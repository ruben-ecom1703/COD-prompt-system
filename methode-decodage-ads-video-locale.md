# Méthode — décoder une ad vidéo (.mp4) en local

Ressource transverse. Applicable à **tous les terrains COD Empire** (Marco Moretti, Nomad Labs, et toute marque dont on veut analyser les ads vidéo winners ou celles d'un concurrent).

Créée le 2026-08-04, à partir du décodage des 3 top spend Marco Moretti.

---

## Le problème

Les ads winners existent souvent uniquement en **fichier vidéo** (Drive, export monteur, capture concurrent). Or :
- Un lien Google Drive public ne suffit pas — un `.mp4` ne se lit pas par simple fetch.
- **Aucun modèle Claude ne peut visionner une vidéo**, quelle que soit la version. Les images (PNG/JPG) et PDF, oui. La vidéo, non.

Sans méthode, on perd l'accès à la donnée la plus riche qu'on possède : ce que disent et montrent réellement nos propres winners.

---

## La méthode (validée en production le 2026-08-04)

Deux passes complémentaires, entièrement **en local sur la machine**, sans ffmpeg ni service externe.

### 1. Structure visuelle — extraction de frames

- Extraction des images clés via **AVFoundation** (Swift), natif macOS.
- Composition d'une **planche-contact** par vidéo (grille de frames horodatées) → lisible d'un coup comme une image simple.
- Pour un détail précis (texte incrusté, commentaire, packaging), **regrab de la frame ciblée en pleine résolution**.

Ce que ça donne : le persona, les décors, les transitions, le rythme, l'end card — et surtout **tout texte incrusté** (hooks, sous-titres, commentaires screenshotés).

### 2. Voix off — transcription on-device

- Transcription via le framework **Speech** d'Apple, en local (rien n'est envoyé à un service tiers).

⚠️ **Deux pièges rencontrés, à anticiper :**
- **TCC / autorisation micro-speech** : un binaire CLI nu ne peut pas demander l'autorisation → le process meurt en `exit 134 (SIGABRT)`. Il faut **packager en `.app`** avec la description d'usage dans l'`Info.plist`, et le lancer via LaunchServices pour qu'il porte sa propre identité.
- **Blocage sur sémaphore** : les callbacks de reconnaissance sont livrés sur la **run loop principale**. Attendre sur un sémaphore qui bloque le main thread fige tout. Ne pas bloquer le main thread.

---

## Quand l'utiliser

- Avant toute réadaptation d'un format winner en un autre format (vidéo → native/statique).
- Avant d'écrire des concepts « ancrés dans la data » : sans les mots exacts de la voix off, on écrit par analogie — et l'analogie produit des erreurs factuelles.
- Sur les ads concurrentes récupérées en vidéo.

## Alternative rapide (si pas le temps)

Demander les éléments en **texte brut** : l'ad copy copiée-collée + le script / la voix off. C'est plus exploitable que la vidéo pour l'analyse de structure. À défaut, **quelques screenshots des moments clés** (hook, plans importants, fin) suffisent à reconstituer la structure.

## Raccourci Trendtrack (ajouté le 2026-09-02)

Pour une ad concurrente disponible sur Trendtrack : la page de partage publique (`app.trendtrack.io/share/ads/…`) contient dans son HTML l'ID Meta (`platform_ad_id`), l'URL du mp4 et l'ad copy. L'outil MCP `scan_ad` avec cet ID renvoie le **transcript complet** quand Trendtrack l'a déjà généré (26 ads sur 30 lors du test). Le mp4 se télécharge avec un User-Agent + Referer `app.trendtrack.io`, puis extraction de frames AVFoundation comme ci-dessus. Application : `1 Terrains/COD Empire/Nomad Labs/analyse-32-concepts-trendtrack.md`.

---

## Enseignement méta

Les angles qu'on « pressent » sont souvent **déjà validés dans nos propres winners** sans qu'on le sache — parce que la donnée dort dans des fichiers qu'on ne relit jamais. Décoder ses propres ads avant d'en inventer de nouvelles est plus rentable que de chercher un nouvel angle.

Voir application concrète : `1 Terrains/COD Empire/Marco Moretti/_context.md` (section 2026-08-04).
