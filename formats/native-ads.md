# Format : Native Ads — B-roll photoréalistes pour publicités natives

> B-roll réalistes pour publicités natives — le spectateur ne doit PAS identifier le contenu comme une pub ni comme de l'IA. **C'est notre format principal.** On cherche le réalisme avant tout, pas la perfection.

---

## 1. STYLE VISUEL — Le photoréalisme natif

### Le principe cardinal
Une native ad réussie doit avoir l'air d'un **snapshot banal pris par un vrai humain**, pas d'une photo de studio. Plus le prompt est "ordinaire", plus le résultat a l'air authentique.

### Rendu
- **Photoréaliste absolu** — qualité photo iPhone/Samsung haut de gamme
- Le résultat doit passer pour une vraie photo quand il défile dans un feed
- Pas trop parfait, pas trop composé — c'est la clé

### Éclairage
- **Lumière naturelle uniquement** : soleil, fenêtre, lampe domestique, overcast daylight
- Accepter les imperfections d'éclairage : zones légèrement surexposées, ombres inégales
- `soft window light`, `overcast daylight`, `warm afternoon light`, `practical lighting`
- Pour un look plus brut/amateur : `harsh flash`, `single overhead bulb`, `fluorescent`
- **JAMAIS** : studio lighting, ring light, dramatic HDR, neon glow, "golden hour" (trop utilisé, devenu une signature IA)

### Cadrage
- Plans serrés et moyens, angles **légèrement imparfaits**
- Sujet légèrement décentré (`slightly off-center cropping`)
- Léger tremblement naturel sur les plans "mains" (`handheld camera with tiny wobble`)
- Horizon pas parfaitement droit (`horizon slightly off level`)
- **Le cadrage "parfait" trahit l'IA** — l'asymétrie est réaliste

### Fond/décor
- Environnements réels du quotidien : cuisine, jardin, rue, bureau, nature, salle de bain
- **Toujours cohérent avec le marché cible** (intérieur hongrois pour Nomad Labs, pas américain)
- Ajouter du clutter subtil : `half-finished drink`, `coffee mug`, `books`, `fruit bowl`, `slightly messy counter`
- Le décor se lit en 0,5 seconde — un frigo américain ou un pavillon US crée une dissonance immédiate

### Couleurs
- Palette naturelle, PAS saturée, PAS filtrée
- Tons chauds pour les moments positifs/produit
- Tons froids/désaturés pour les moments problème/tension
- `natural colour grading`, `muted tones`, `earthy palette`
- Film stock pour rendu spécifique : `Kodak Portra 400` (chaud crémeux), `Fujifilm Classic Chrome` (désaturé muted)

---

## 2. LA CLÉ DU RÉALISME — Imperfections obligatoires

Les vraies photos sont imparfaites. L'IA génère de la perfection par défaut — c'est ce qui la trahit. Chaque prompt native ad doit inclure AU MOINS 2-3 imperfections.

### Imperfections textures (choisir 1-2)
- `visible pores`, `faint skin texture`, `fine baby hairs visible`
- `skin blemishes`, `fabric wrinkles`, `wear marks`
- `dust and scratches`, `fingerprints on surfaces`
- `no retouching`, `zero artificial beauty retouching`
- `catchlights in both eyes` (détail critique pour les portraits)

### Imperfections caméra (choisir 1-2)
- `slight film grain`, `digital noise`, `subtle sensor noise`
- `soft focus areas`, `slight motion blur`
- `overexposed highlights`, `gentle vignette darkening corners`
- `slight chromatic aberration at high-contrast edges`
- `bokeh fringing`

### Imperfections environnement (choisir 1)
- `subtle background clutter`, `slightly imperfect table arrangement`
- `crumbs on counter`, `dishes drying by sink`
- `dust particles in light beam`
- `condensation on cold glass`, `water ring stain on table`

### Imperfections composition (implicite via le cadrage)
- `candid moment`, `unstaged composition`
- `subject slightly off-center`, `awkward angle`
- `mid-laugh turning toward camera`

---

## 3. LANGAGE CAMÉRA — L'outil #1 du photoréalisme

Spécifier une caméra/objectif réel active le mode photographique du modèle IA (les modèles ont appris sur des images taguées avec leurs données EXIF).

### Par type de plan natif

| Plan | Caméra/objectif | Effet |
|---|---|---|
| Mains qui manipulent le produit | `shot on iPhone Pro`, `35mm f/2` | Casual, quotidien |
| Portrait/personne avec produit | `Sony A7III with 85mm f/1.4, shallow depth of field` | Sujet isolé, beau bokeh |
| Produit dans son contexte | `50mm lens, natural depth of field` | Proche de l'œil humain |
| Scène large (nature, camping) | `24mm wide angle` | Contexte environnemental |
| Macro produit/texture | `100mm macro f/2.8` | Détails intimes |
| Look amateur/authentique | `shot on iPhone`, `disposable camera, harsh flash` | UGC feel |

### Chaînes caméra qui marchent bien
- `shot on iPhone Pro front camera` — le plus casual/UGC
- `Fujifilm X-T4 with 35mm f/1.4 at ISO 1600` — street/documentary
- `Sony A7III with 50mm lens, shallow depth of field` — lifestyle
- `Canon EOS R5, 85mm f/1.4, ISO 200` — portrait premium
- `Sigma 85mm f/1.4` — sujet net + bokeh crémeux

### ISO pour le grain naturel
- ISO 100-200 : image propre, lumière abondante
- ISO 800-1600 : grain subtil, look naturel intérieur
- ISO 3200+ : grain visible, look low-light/nocturne

---

## 4. CE QU'ON VOIT

- Des **mains qui manipulent le produit** (pattern winner : sans visage, cadrage mains uniquement)
- Des situations du **quotidien crédibles**
- Le produit dans son **contexte d'usage réel**
- Des **détails texturés** (gouttes d'eau, surface du produit, matériaux de l'environnement)
- Des **personnes normales** (pas des mannequins, pas de maquillage pro, pas de tenue de shooting)

---

## 5. CE QU'ON NE VOIT PAS

- Pas de fond studio / fond uni
- Pas de texte superposé sur l'image
- Pas de mise en scène publicitaire évidente
- Pas de visage parfait / mannequin / peau plastique
- Pas d'éclairage artificiel visible
- Pas de composition parfaitement centrée
- Pas de symétrie parfaite (les vrais visages et scènes sont asymétriques)

---

## 6. TEMPLATES DE PROMPTS

### Template principal (le plus utilisé)
```
[Cadrage] of [sujet avec détails physiques] in [environnement du marché cible]. [Action naturelle/pose]. [Éclairage naturel spécifique]. Shot on [caméra/objectif], [ISO si pertinent]. [2-3 imperfections]. [Style]. Not a professional photo, not an advertisement.
```

**Exemple Hydra X2 :**
"Close-up of weathered hands of a 60-year-old man holding a small blue cylindrical water filter straw (~20cm, 'NOMAD LABS' inscription) over a rocky stream. Natural overcast daylight, soft shadows falling unevenly. Shot on iPhone 15 Pro, slight digital noise, visible skin texture on knuckles. Candid documentary style. Subject slightly off-center, water motion slightly blurred. 9:16 vertical format. Not a professional photo, no studio lighting, no perfect composition."

### Template produit dans contexte
```
[Cadrage] of [produit avec description physique précise] [position/action] in [décor quotidien du marché cible]. [Éclairage]. Shot on [caméra]. [Détails texture environnement]. [Imperfections]. No text, no logo overlay. Not a studio photo.
```

**Exemple :**
"Medium shot of a small blue water filter straw resting on a worn wooden kitchen table next to a half-empty glass of water and a set of car keys. Warm afternoon window light from camera left, soft shadows. Shot on 35mm f/2, slight film grain. Slightly messy table surface with crumbs. Condensation droplets on the glass. 9:16 vertical. No advertisement look."

### Template "mains qui tiennent" (le pattern winner)
```
Close-up of [type de mains] holding [produit avec taille et couleur] [geste d'usage]. [Environnement visible en arrière-plan flou]. [Éclairage naturel]. Shot on [caméra], [profondeur de champ]. [Texture peau]. [Imperfection caméra]. Candid, not posed.
```

**Exemple :**
"Close-up of tanned female hands holding a small blue water filter straw (~20cm) up to a clear mountain stream, about to dip it in. Blurred green forest background. Natural overcast light, soft shadows. Shot on Sony A7III 50mm f/1.8. Visible skin texture, faint sun spots on forearms. Slight motion blur on the water surface. Candid, not posed. 9:16."

### Template scène problème (avant le produit)
```
[Cadrage] of [visualisation du problème] in [environnement quotidien]. [Éclairage cool/muted]. [Caméra]. [Tons froids/désaturés]. [Imperfections]. Documentary style. Subtle tension in the frame.
```

---

## 7. MOTS-CLÉS

### Obligatoires (inclure dans chaque prompt)
`realistic`, `natural lighting`, `candid`, `everyday setting`, `authentic`, `not a professional photo`

### Fortement recommandés (inclure 2-3)
`shot on [caméra spécifique]`, `slight film grain`, `visible skin texture`, `off-center composition`, `handheld`, `documentary style`, `subtle background clutter`

### Interdits (ne JAMAIS inclure)
`studio lighting`, `professional photography`, `advertisement`, `commercial`, `perfect`, `glossy`, `flawless`, `pristine`, `3D render`, `illustration`, `cartoon`, `cinematic` (trop stylisé), `hyper-realistic` (paradoxalement déclenche un rendu peint), `magical`, `ethereal`, `dreamlike`, `stock photo`, `model`

### Note DALL-E 3 spécifique
- Utiliser `photo style` au lieu de `photorealistic` (ce dernier déclenche un rendu airbrush/peint)
- Écrire en phrases complètes, pas en liste de tags
- Les négations directes ("no text") fonctionnent mal — décrire ce qu'on VEUT à la place
- Max 30-40 tokens graphiques efficaces (au-delà, perte de qualité)

### Note GPT-4o / GPT Image
- Plus naturel pour le photoréalisme que DALL-E 3
- Supporte l'édition itérative ("change only the background to...")
- Ajouter `(don't change the prompt, send it as it is)` pour empêcher la réécriture automatique
- Relancer le chat toutes les 3-5 générations pour éviter la dégradation de qualité

---

## 8. ERREURS FRÉQUENTES À ÉVITER

1. **Produit trop centré/posé** comme une photo de catalogue → décentrer, angle imparfait
2. **Éclairage trop parfait/uniforme** → ajouter des zones d'ombre, surexpositions naturelles
3. **Mains avec 6 doigts** ou proportions étranges → ajouter `realistic hand grip, anatomically correct hands` + négatifs mains
4. **Décor américain pour un marché européen** → toujours spécifier le style de décor du marché cible
5. **Produit à la mauvaise échelle** → toujours donner les dimensions et un objet de comparaison
6. **Peau plastique/waxy** → toujours inclure `visible pores`, `natural skin texture`, `no retouching`
7. **Trop de mots-clés "qualité"** → `hyper realistic, ultra detailed, 8k, masterpiece` empilés = résultat pire, pas meilleur
8. **Couleurs trop saturées** → spécifier `natural colour grading`, `muted tones`
9. **Symétrie parfaite** → les vraies scènes sont asymétriques, toujours demander de l'imperfection
10. **"Golden hour" systématique** → c'est devenu un signal IA. Varier : `overcast`, `flat grey light`, `muted cool color`

---

## 9. GUIDE PAR SURFACE/DÉCOR

| Surface/environnement | Quand l'utiliser | Mots-clés |
|---|---|---|
| Cuisine domestique | Produit alimentaire/santé, usage quotidien | `home kitchen counter`, `worn wooden table`, `morning light through window` |
| Nature/extérieur | Produit outdoor, aventure, survie | `rocky stream`, `forest trail`, `campsite`, `overcast natural light` |
| Salle de bain | Produit santé/hygiène | `bathroom shelf`, `slightly messy counter`, `morning natural light` |
| Bureau/travail | Productivité, bien-être | `cluttered desk`, `laptop in background`, `office window light` |
| Voiture/transport | Mobilité, voyage | `car dashboard`, `backseat`, `travel context` |
| Marché/rue | Quotidien, authenticité locale | `local market`, `street vendor`, `urban setting` |
