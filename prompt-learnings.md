# Prompt Learnings

> Ce qui marche et ce qui ne marche pas — accumulé au fil des tests. Ajouter une entrée datée à chaque apprentissage.

## 2026-07-19

### Ce qui ne marche PAS

- **Mockup 3D sans fiche de référence** : les concepts proposés par l'IA étaient trop génériques, pas assez "blueprint médical". L'IA ne sait pas ce qu'est un "mockup 3D publicitaire" sans description précise du style attendu → ajout de la fiche `formats/mockup-3d.md`.
- **Produit sans dimensions physiques** : l'IA générait le filtre Hydra X2 à la mauvaise taille (trop grand, type pompe à vélo). Fix : ajout de la section "Physique & utilisation" dans `01-brand.md` du repo marque avec dimensions (~20cm × ~3cm) et gestes d'usage corrects.
- **Format "Autre" sans directive** : quand le monteur tape un format libre, l'IA n'a aucune référence et génère du générique.

### Ce qui marche

- **Pattern "sans visage"** : les B-roll cadrant uniquement les mains qui manipulent le produit performent très bien. À systématiser comme option par défaut sur les plans produit.
- **Data marque injectée depuis GitHub** : la qualité des prompts augmente significativement quand la data réelle du produit (usage, contexte, marché) est injectée vs quand l'IA doit deviner.

## 2026-07-20

### Analyse des ads BONJOUR (café foie) — 9 vidéos

**Découverte majeure : "cartoon" ≠ flat 2D.** Le style qui performe dans les ads santé est du **3D Pixar avec organes anthropomorphes** (yeux, bouche, émotions, petits bras). C'est un rendu 3D haute qualité avec subsurface scattering, pas de l'illustration plate. La fiche `formats/cartoon.md` a été entièrement réécrite.

**Deux formats distincts identifiés dans le même corpus d'ads :**
1. **Cartoon 3D Pixar** (6/9 vidéos) : organe = personnage avec émotions, dans son environnement anatomique. Éclairage chaud/ambre (sain) ou vert/sombre (menace). Les bactéries sont des créatures noires hérissées.
2. **Mockup 3D médical** (2/9 vidéos) : coupe anatomique hyperréaliste sur fond blueprint bleu quadrillé. Aucune anthropomorphisation. Lobules hépatiques et vaisseaux sanguins en détail d'atlas médical.

### Patterns visuels capturés

- **Hook "plan contexte humain"** : l'organe cartoon est sorti de son corps et placé dans un décor quotidien (cerveau dans un lit à 01:00 du matin, foie devant une assiette). Mix décor semi-réaliste + personnage cartoon → très bon scroll-stop.
- **Métaphore "usine"** : le foie est montré comme un employé débordé dans une salle de contrôle, submergé de livraisons (cartons de sucre, donuts). La métaphore travail/surmenage est immédiatement lisible.
- **Convention sous-titres** : blanc bold + ombre, avec UN mot-clé en jaune par phrase. Hook en haut dans une bulle blanche arrondie.

## 2026-07-20 — Recherche prompt engineering (Nano Banana Pro, ChatGPT/DALL-E 3, GPT-4o, cross-model)

### Ce qui MARCHE pour le photoréalisme (compilé de toutes les sources)

- **Langage caméra/objectif = technique #1** : spécifier un boîtier et une focale réels (ex : `Sony A7III with 85mm f/1.4`) active le mode photographique du modèle. Les modèles ont appris sur des millions d'images taguées avec leurs données EXIF. Une spec caméra précise bat cinq adjectifs de qualité empilés.
- **Imperfections systématiques** : `visible pores`, `slight film grain`, `off-center cropping`, `slightly overexposed highlights`. La technique de la "photo banale" (prompter pour des snapshots imparfaits) produit le réalisme le plus convaincant.
- **Éclairage directionnel** : toujours spécifier d'où vient la lumière (`from camera left`, `from above and slightly right`). L'éclairage uniforme/flat est un signal IA.
- **Phrases > tags** : écrire des descriptions en phrases complètes, pas des listes de mots-clés. Surtout pour DALL-E 3 (entraîné sur des captions descriptives).
- **Film stocks** : `Kodak Portra 400` (tons chauds crémeux), `Fujifilm Classic Chrome` (muted désaturé) activent des rendus couleur spécifiques.
- **ISO dans le prompt** : `ISO 1600` introduit du grain naturel sans devoir le demander séparément.
- **Catchlights dans les yeux** : le détail qui sépare un portrait réaliste d'un mannequin. `catchlights in both eyes`.

### Ce qui NE MARCHE PAS (pièges à éviter)

- **"Photorealistic" sur DALL-E 3** : paradoxalement, ce mot déclenche un rendu peint/airbrush. Utiliser `photo style` ou `photo image` à la place.
- **Keyword stacking** : `hyper realistic, ultra detailed, 8k, photorealistic, masterpiece` empilés = résultat PIRE. Le modèle perd le focus. 3-5 détails précis > 10 buzzwords.
- **"Golden hour" systématique** : c'est devenu un signal IA tellement c'est utilisé. Varier avec `overcast`, `flat grey light`, `muted cool color`.
- **Négations directes sur DALL-E 3** : "no text", "without shadows" → le modèle génère souvent l'inverse. Décrire ce qu'on VEUT à la place.
- **"Perfect", "flawless", "pristine"** : poussent le générateur vers un idéalisme qui trahit l'IA.
- **Contradictions** : "photorealistic cartoon" crée des résultats confus.
- **Trop de tokens** : DALL-E 3 traite ~256 tokens mais seulement 30-40 se traduisent en graphiques. Au-delà, qualité qui baisse.
- **Nano Banana Pro** : max 5 adjectifs, 1-3 phrases. Plus long = perte de focus.

### Framework SCALD (Nano Banana Pro — utile pour structurer les prompts ads)

- **S**ubject : le sujet principal
- **C**ontext : l'environnement/décor
- **A**esthetics : style visuel, mood
- **L**ayout : composition, angle, format
- **D**irective : contraintes, exclusions

### GPT-4o vs DALL-E 3 — ce qui change

- GPT-4o gère le photoréalisme plus naturellement (87% vs 62% de "convincingness" en test aveugle)
- GPT-4o supporte l'édition itérative dans la même conversation
- GPT-4o est plus lent (60-180s vs 20-45s)
- DALL-E 3 deprecated de l'API depuis mai 2026
- GPT-4o réécrit les prompts automatiquement → ajouter `(don't change the prompt, send it as it is)` pour l'empêcher
- Relancer le chat GPT-4o toutes les 3-5 générations (dégradation de qualité sinon)

### Cohérence de personnage entre plans (learning important pour UGC IA)

- La cohérence parfaite est **impossible** — chaque génération est indépendante. On peut atténuer, pas éliminer.
- **Méthode "anchor image"** : générer UN portrait de référence parfait, puis l'uploader comme référence pour tous les plans suivants.
- **Character DNA** : description détaillée réutilisée mot pour mot dans chaque prompt (traits physiques, tenue, accessoires).
- **Preserve lists** : `Do not change face, facial features, skin tone, body shape. Preserve exact likeness.`
- **Style lock** : créer un snippet de style fixe appendé à chaque prompt pour la cohérence visuelle.

---

_Ajouter les prochains learnings ci-dessous, toujours avec la date et catégorie (marche / marche pas)._
