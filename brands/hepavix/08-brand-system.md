# 08 — Brand system : code couleur & identité visuelle

> 📅 Dernière mise à jour : 2026-08-09 · Source : CSS live de hepavix.com + créas de production · Gérant : Hugo

**Ce que contient ce fichier :**
- Le code couleur exact du site (hex)
- Les typographies
- Le packshot de référence et la règle du flacon
- Le style visuel qui vend (et celui qui ne vend pas)
- Les conventions de nommage

**Sommaire** : [Code couleur](#code-couleur) · [Typographies](#typographies) · [Le flacon](#le-flacon) · [Style visuel des créas](#style-visuel-des-créas) · [Les 3 pages Facebook](#les-3-pages-facebook) · [Logo](#logo--exploration-en-cours-0808) · [Nommage des fichiers](#nommage-des-fichiers)

---

## Code couleur

Extrait du CSS live de hepavix.com le 14/07/2026 :

| Rôle | Hex | Usage |
|---|---|---|
| **Bleu marine (couleur de marque)** | `#16344f` | Wordmark HEPAVIX, titres, bandeau promo, bandeaux des statics |
| **Bleu médian (CTA)** | `#2d6da3` | Bouton « Megrendelem », liens, éléments actifs |
| Bleu très foncé | `#1c2b38` | Texte principal |
| Gris-bleu | `#6f8090` | Texte secondaire |
| **Bleu pâle (fonds)** | `#eaf2f8` · `#e2ebf1` · `#e7eef3` | Cartes, blocs, fonds de sections |
| Blanc cassé | `#f6f9fb` | Fond général |
| Cyan accent | `#38bdf8` | Accents ponctuels |

**Logique** : univers **bleu clinique / pharmaceutique** (sérieux, médical, propre) — cohérent avec le positionnement « qualité pharmaceutique ». Le produit lui-même est **blanc**, ce qui renforce le côté clinique.

## Typographies

| Usage | Police |
|---|---|
| Principale | **Inter** |
| Fallback | -apple-system, BlinkMacSystemFont |

## Le flacon

- **Flacon BLANC**, wordmark **HEPAVIX** en bleu marine, « Pharmaceutical Grade Liver Protection & Recovery », **« 60 CAPSULES »**, petit logo feuille/foie.
- Packshot officiel de référence : [`hepavix-flacon-officiel.jpg`](assets/hepavix-flacon-officiel.jpg) · rendu du site : [`hepavix-hero-site-1024.jpg`](assets/hepavix-hero-site-1024.jpg)
- ⚠️ **Toujours compositer le packshot réel.** Ne jamais laisser un générateur d'image « inventer » le flacon (il dérive systématiquement : mauvaise étiquette, mauvaise couleur, mauvais nombre de gélules).
- ⚠️ **Ne pas confondre avec Keskia** (flacon orange, gouttes, produit pour chien).

## Style visuel des créas

**✅ CE QUI VEND — le dessin simple, pas la photo**

Le winner ([Ads 2](ads/cortisol-winner.md), 36 ventes) tourne avec un visuel qui est **un dessin, pas une photo** : fond blanc, **deux silhouettes de ventre vues de côté** — à gauche un ventre qui pend (« Kötényhas »), à droite un ventre plus plat (« Alhasi zsírpárna »). Effet avant/après en douceur. **Aucun produit visible.**

C'est le **learning n°1 de la brand** : *le visuel fait la moitié de la performance*, et le visuel qui gagne **montre le problème du lecteur**, il ne montre pas le produit.

Autres visuels qui ont vendu :
- [Ads 12](ads/statines-airbnb.md) : une **fausse capture de caméra de surveillance** (noir et blanc, fisheye, horodatage `2026-05-17 05:22:09`) qui reconstitue littéralement la scène du texte. Ultra-natif, ne ressemble à aucune pub.
- [Ads 5](ads/offre-ldl-directe.md) / [Ads 6](ads/alcool-detox.md) : statics de marque (flacon + bandeau bleu marine) — mais ce sont des **ads d'offre**, pas des natives.

**❌ CE QUI NE VEND PAS** : les statics produit sur les angles éditoriaux. Constat identique sur les 4 brands du portefeuille : quand on montre le produit dans une native ad, on ne vend pas.

**⚠️ Règle Meta** : sur les angles alcool, **jamais de verre d'alcool visible** (cause de refus documentée — [03-compliance.md](03-compliance.md#refus-meta-déjà-encaissés)).

**Décrire un visuel** : toujours en mots simples et concrets (« un ventre gros et un ventre plat, dessinés, sur fond blanc »), jamais en jargon (« infographie diagnostique comparative »).

## Les 3 pages Facebook

| Page | Rôle | Ce qu'on y publie |
|---|---|---|
| **Dr. Tóth Petra Menopauza szakértő** | Autorité médicale | Advertorials « le médecin qui raconte ses patientes » |
| Varga Nóra Szexológus | Persona femme | Témoignages à la première personne ⚠️ *mais le narrateur doit coller à la page — voir le cas Ads 12* |
| Hepavix (page marque) | Marque | Statics et ads d'offre, sans narrateur |

**À créer à la relance** : 2-3 pages « médecin / expert santé » supplémentaires pour diluer le risque (aujourd'hui tout repose sur Dr. Tóth Petra), et une vraie page « femme 55-65 » pour les récits pair-à-pair.

## Logo — exploration en cours (08/08)

Un nouveau logo est en exploration : **7 directions** briefées (raffinement de l'actuel · monogramme H hexagonal · foie stylisé en feuilles · bouclier · typographie pure avec un V en forme de feuille · sceau pharmacie · goutte-foie style biotech dégradé marine→cyan). **4 des 7 seulement ont été générées** — le batch a été interrompu par une panne du connecteur de génération en cours de route. **Aucun choix fait par Hugo à ce stade.** Rien à intégrer dans ce repo tant que la direction n'est pas tranchée et le fichier final produit.

## Nommage des fichiers

- Ads : `ads/<slug-descriptif>.md` (le nom Meta `Ads N` est rappelé en titre — c'est la clé de croisement avec les exports)
- Visuels publiés : `visuels/ads-testees/<nom-du-fichier-source>.jpg`
- Jamais d'espaces, d'accents ni de parenthèses dans les noms de fichiers (ça casse les liens markdown).
- Repos GitHub : préfixe `COD-`.

---

*Navigation : [← 07 — Relance](07-relance.md) · [09 — Site & funnel →](09-site-funnel.md)*
