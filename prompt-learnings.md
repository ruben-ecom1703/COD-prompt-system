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

---

_Ajouter les prochains learnings ci-dessous, toujours avec la date et catégorie (marche / marche pas)._
