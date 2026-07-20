# Format : UGC IA (User Generated Content simulé par IA)

> Simule du contenu filmé par un vrai utilisateur avec son téléphone — selfie, POV, face caméra. Le spectateur doit croire que c'est une vraie personne qui filme.

---

## 1. STYLE VISUEL

### Rendu
- **Ultra-réaliste, qualité caméra frontale de smartphone** — pas une caméra pro
- Le résultat doit ressembler à une vidéo envoyée par messagerie, légèrement compressée
- **Pas trop clean** — la perfection technique trahit le faux UGC

### Cadrage
- **Selfie** : bras tendu ou trépied bas, angle légèrement en dessous du visage
- **POV** : ce que la personne voit (ses mains qui déballent, le produit devant elle)
- **Face caméra** : plan moyen, la personne regarde l'objectif
- Léger tremblement naturel (`handheld`), pas de steadicam parfait
- Sujet pas parfaitement centré

### Éclairage
- Lumière naturelle imparfaite : fenêtre, extérieur, lampe de bureau
- Légères ombres, zones inégalement éclairées
- `natural daylight from window`, `slightly uneven exposure`
- Acceptable : `harsh flash` pour un look story/snap brut
- **JAMAIS** : studio lighting, ring light, softbox, professional setup

### Décor
- Intérieur domestique réel : chambre, cuisine, salle de bain, voiture
- Extérieur quotidien : trottoir, parc, café
- **Du clutter visible** : `coffee mug`, `phone charger on table`, `slightly messy background`
- Adapté au marché cible (pas de décor américain pour marché européen)

---

## 2. RÈGLE CRITIQUE : COHÉRENCE DU PERSONA

**Un seul persona par vidéo.** C'est le défaut #1 des UGC IA.

Tous les plans d'une même vidéo doivent montrer :
- Le même visage, la même morphologie
- La même tenue vestimentaire
- Le même environnement (ou logiquement connecté)
- Le même type de peau, couleur de cheveux, accessoires

### Comment maintenir la cohérence dans les prompts
- Créer un "character DNA" réutilisé dans chaque prompt :
  > "30-year-old woman with shoulder-length brown hair, light freckles, wearing an oversized grey t-shirt"
- Reprendre cette description **mot pour mot** dans chaque prompt de la série
- Ajouter explicitement : `Do not change face, facial features, skin tone, body shape. Preserve exact likeness. Change only [pose/action/angle].`
- Si possible, uploader une image de référence et demander "same person as in the reference image"

### Persona adapté au marché
- **Hongrie** : traits d'Europe centrale, 30-55 ans pour produit santé, vêtements casual de tous les jours
- Ne jamais utiliser un persona qui ne correspond pas à la cible (ex : jeune mannequin sportive pour un produit 55+)

---

## 3. TYPES DE PLANS

### Face caméra
- La personne regarde l'objectif et "parle" (bouche fermée OK si voix off)
- Expression naturelle, pas de sourire forcé
- `front camera selfie angle, eye contact with camera, natural expression`

### POV mains
- Les mains de la personne manipulent le produit (on ne voit pas le visage)
- `POV shot, hands holding [product], first-person perspective`
- Les mains doivent être cohérentes avec le persona (même teint, même type)

### Selfie avec produit
- La personne se filme en tenant/montrant le produit
- Un bras tient le téléphone, l'autre tient le produit
- `selfie with product, one arm extended holding phone, casual pose`

### Plan de réaction
- Expression faciale : surprise, satisfaction, dégoût face au problème
- `candid reaction shot, genuine expression of [emotion]`

### Plan "preuve"
- Gros plan sur le produit, l'emballage, le résultat
- Filmé de près comme pour montrer à un ami
- `close-up proof shot, showing [detail] to camera, shaky handheld`

---

## 4. TEMPLATES DE PROMPTS

### Template selfie face caméra
```
Ultra-realistic front camera selfie of [character DNA], looking directly at camera with [expression]. [Décor domestique du marché cible]. [Éclairage naturel imparfait]. Shot on iPhone Pro front camera. [Imperfections : grain, angle, peau]. Raw unfiltered UGC style. No beauty retouching, no studio, no model. Vertical 9:16.
```

**Exemple :**
"Ultra-realistic front camera selfie of a 35-year-old woman with shoulder-length brown hair and light freckles, wearing a grey oversized t-shirt, looking at camera with a slightly surprised excited expression. Standing in a small European kitchen, morning light from a window on the left, slightly uneven exposure. Shot on iPhone Pro front camera. Slight digital noise, visible skin pores, no makeup, faint under-eye circles. Raw unfiltered UGC style. Not a professional photo. Vertical 9:16."

### Template POV mains avec produit
```
POV first-person shot of [mains cohérentes avec le persona] holding [produit avec dimensions/couleur] in [environnement]. [Action]. [Éclairage]. Shot on iPhone. Handheld slight wobble. [Imperfections]. Authentic UGC feel.
```

### Template unboxing
```
[Cadrage] of [persona] opening a package on [surface domestique]. [Produit visible dans l'emballage]. [Éclairage naturel]. Shot on smartphone, slightly shaky. Genuine excitement/curiosity on face. [Clutter domestique visible]. Not a professional unboxing, not a studio.
```

---

## 5. MOTS-CLÉS

### Obligatoires
`selfie`, `front camera`, `handheld`, `natural lighting`, `authentic`, `user generated content`, `smartphone quality`, `casual`, `everyday person`, `no makeup`, `home setting`

### Fortement recommandés
`shot on iPhone`, `slight digital noise`, `visible skin pores`, `slightly off-center`, `raw unfiltered`, `not a professional photo`, `slightly uneven exposure`, `natural skin texture`

### Négatifs spécifiques UGC (à inclure)
`No studio lighting, no professional photography, no stock photo, no model, no perfect skin, no heavy makeup, no perfect composition, no centered framing, no staged, no commercial, no advertisement`

### Interdits
`professional photography`, `studio`, `model`, `advertisement`, `perfect lighting`, `3D`, `illustration`, `polished`, `commercial`, `cinematic`, `glossy`, `flawless`

---

## 6. ERREURS FRÉQUENTES À ÉVITER

1. **Persona qui change** entre les plans → character DNA identique partout
2. **Qualité trop haute** (trop net, trop bien éclairé) → ajouter grain, compression, angle imparfait
3. **Mains avec anomalies** → négatifs mains + `realistic hand grip, anatomically correct hands`
4. **Décor trop luxueux/parfait** → ajouter du clutter, objets du quotidien
5. **Personne qui ressemble à un mannequin** → `everyday person`, `no makeup`, `natural imperfections`, `visible pores`
6. **Persona incohérent avec le marché** → adapter âge, ethnie, style vestimentaire au marché cible
7. **Peau plastique/lisse** → `visible pores`, `faint skin texture`, `skin blemishes`, `no retouching`
8. **Sourire trop parfait** → `natural expression`, `casual smile`, `mid-conversation expression`
9. **Éclairage uniforme sans ombre** → spécifier la direction de la lumière et les zones d'ombre
10. **Arrière-plan trop propre** → `slightly messy background`, `everyday clutter visible`
