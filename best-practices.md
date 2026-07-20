# Best Practices — Prompts B-roll IA

> Règles générales appliquées à TOUS les prompts, quel que soit le format. Injecté systématiquement par le SaaS. Compilé à partir de recherches sur DALL-E 3, GPT-4o, Nano Banana Pro (Gemini 3), Flux, Midjourney.

---

## STRUCTURE D'UN PROMPT — La formule universelle

L'ordre des éléments dans le prompt COMPTE. Les premiers éléments reçoivent plus d'attention du modèle. Structure recommandée :

```
[Cadrage/type de plan] + [Sujet principal] + [Action/pose] + [Environnement/décor] + [Éclairage] + [Caméra/objectif] + [Style/mood] + [Imperfections/grain] + [Négatifs/exclusions]
```

**Longueur optimale** : 1-3 phrases, max 5 adjectifs. Au-delà, le modèle perd le focus et la qualité baisse.

**Écrire en phrases, pas en tags** : les modèles (surtout DALL-E 3) ont été entraînés sur des descriptions en phrases complètes, pas sur des listes de mots-clés séparés par des virgules.
- **Mauvais** : `forest, morning, fog, deer, sunbeams, realistic`
- **Bon** : `A lone deer stands in a misty forest at dawn, with golden sunbeams filtering through the pine trees. Morning fog hangs low between the trunks.`

---

## Règle #1 : UN concept = UNE idée visuelle

Chaque prompt doit décrire UNE SEULE scène, UN SEUL plan. Pas de prompt qui essaie de raconter une histoire en une image.

**Bon** : "Gros plan sur des mains d'homme âgé tenant le filtre Hydra X2 bleu au-dessus d'un ruisseau, lumière naturelle douce"
**Mauvais** : "Un homme au bord d'un ruisseau qui filtre l'eau puis la boit et sourit de satisfaction avec sa famille en arrière-plan"

---

## Règle #2 : Toujours spécifier l'échelle du produit

Le produit doit TOUJOURS être décrit avec une référence de taille dans le prompt (dans une main, à côté d'une bouteille, dans une poche). Sans ça, l'IA invente la taille et se trompe systématiquement.

---

## Règle #3 : Le langage caméra/objectif transforme le réalisme

**C'est la technique qui a le plus d'impact sur le photoréalisme.** Spécifier des métadonnées de caméra réelles active le rendu photographique dans le modèle (les modèles ont appris sur des images étiquetées avec les données EXIF).

### Focales et leur effet :
- **24mm** — grand angle, contexte environnemental, légère distorsion sur les bords
- **35mm** — le plus naturel/réaliste, style street photography
- **50mm** — perspective la plus proche de l'œil humain, polyvalent
- **85mm f/1.4** — gold standard portrait, beau bokeh, isolation nette du sujet
- **100-300mm** — compression téléphoto, sujets isolés

### Exemples de chaînes caméra qui marchent :
- `shot on iPhone Pro front camera` — style UGC/casual
- `Nikon D810, ISO 64, focal length 20mm, f/9` — paysage net
- `Sony A7III with 50mm lens, shallow depth of field` — portrait lifestyle
- `Sigma 85mm f/1.4` — sujet net + bokeh crémeux
- `disposable camera, harsh flash` — style nostalgique/brut

---

## Règle #4 : L'éclairage fait la différence réel/IA

### Éclairage réaliste (utiliser) :
- `natural light`, `soft window light`, `golden hour sunlight`
- `overcast daylight`, `warm afternoon window light`
- `practical lighting` (lumières qui existent dans la scène)
- `harsh flash` (pour look casual/amateur)
- `single overhead bulb`, `fluorescent lighting` (pour réalisme banal)

### Éclairage qui TUE le réalisme (éviter) :
- `neon glow`, `magical lighting`, `fantasy lighting`
- `dramatic HDR`, `ethereal light`, `dreamlike`
- `studio lighting` (sauf si c'est explicitement voulu)

---

## Règle #5 : Les imperfections = la clé du réalisme

**Le concept le plus important pour du natif.** Les vraies photos sont imparfaites. L'IA par défaut génère de la perfection, ce qui se repère immédiatement comme artificiel.

### Imperfections à demander :
**Textures** : `visible pores`, `skin blemishes`, `fabric wrinkles`, `wear marks`, `dust and scratches`, `fingerprints on surfaces`, `faint skin texture`, `fine baby hairs visible`

**Caméra** : `slight film grain`, `digital noise`, `soft focus areas`, `slight motion blur`, `overexposed highlights`, `awkward angle`, `slightly off-center cropping`

**Environnement** : `subtle background clutter`, `half-finished drink`, `rumpled bedding`, `slightly imperfect table arrangement`

### La technique "photo banale" (très efficace)
Pour le réalisme maximum, ne PAS viser la perfection. Prompter pour des snapshots imparfaits, banals, quotidiens. Plus le prompt est "ordinaire", plus le résultat a l'air authentique.

---

## Règle #6 : Inclure les négatifs/exclusions

Toujours préciser ce qu'on NE veut PAS. L'IA a des biais par défaut qu'il faut contrer explicitement.

### Négatifs standards de qualité :
`low quality, blurry, watermark, text, logo, bad anatomy, extra fingers, deformed hands, cluttered composition`

### Négatifs pour le réalisme natif :
`studio lighting, professional photography, stock photo, model, perfect skin, heavy makeup, perfect composition, centered framing, staged, commercial, advertisement`

### Négatifs pour les mains (problème récurrent) :
`deformed hands, extra fingers, fused fingers, blurry hands, missing thumbs, warped joints, melted details, overlapping hands`

**Note DALL-E 3** : les négations directes ("no text", "without shadows") fonctionnent mal. Préférer décrire ce qu'on VEUT au lieu de ce qu'on ne veut pas.

---

## Règle #7 : Cohérence entre les plans d'une même vidéo

Tous les prompts d'une même vidéo doivent partager :
- Le même style visuel (pas de mix réaliste + cartoon)
- La même palette de couleurs dominante
- Le même niveau de qualité/grain
- Le même type de cadrage général
- Le même persona si un personnage apparaît (visage, tenue, environnement identiques)

Pour maintenir l'identité d'un personnage entre plans : `Do not change face, facial features, skin tone, body shape. Preserve exact likeness. Change only [ce qui change].`

---

## Règle #8 : Le marché cible dicte le décor

Toujours adapter l'environnement au marché :
- **Hongrie** → intérieurs d'Europe de l'Est, petites villes hongroises, jardins, campagne. JAMAIS de décor américain
- **France** → intérieurs français typiques, pas de McMansion américaine
- Le décor se lit en 0,5 seconde — un frigo américain ou un pavillon US crée une dissonance immédiate

---

## Règle #9 : Produit fidèle au réel

Ne JAMAIS inventer le design du produit. Toujours décrire le produit tel qu'il est réellement (couleur, forme, taille, marquages). Si l'info physique n'est pas dans la data marque, ne pas deviner — demander.

Spécifier la matérialité précise — pas "veste" mais "veste en tweed bleu marine". Pas "filtre" mais "paille filtrante cylindrique bleue, ~20cm, inscription 'NOMAD LABS' en blanc".

---

## Règle #10 : Pas de texte dans l'image

Sauf indication contraire explicite, ne pas demander de texte/mots/chiffres dans l'image. Les modèles génèrent du texte déformé dans 90% des cas. Le texte sera ajouté en post-production.

**Exception Nano Banana Pro/GPT-4o** : si du texte est nécessaire, le mettre entre guillemets, max 5 mots, en début de prompt. Décrire la typo : `"NOMAD LABS" in bold white sans-serif font`.

---

## Règle #11 : Laisser de l'espace pour le texte overlay

Pour les plans destinés à avoir du texte en post-production (hook, CTA), spécifier : `clean negative space in upper left for headline text` ou `empty area in lower third for subtitle`.

---

## Règle #12 : Aspect ratio selon la plateforme

Toujours spécifier le format dans le prompt :
- **TikTok / Reels / Stories** : 9:16 vertical
- **Instagram feed** : 1:1 ou 4:5
- **YouTube** : 16:9
- **Facebook feed** : 1:1 ou 4:5

---

## TEMPLATES DE PROMPTS RÉUTILISABLES

### Template natif/réaliste (le plus fréquent pour nous)
```
[Cadrage] of [sujet] in [environnement du marché cible]. [Action/pose]. [Éclairage naturel]. Shot on [caméra/objectif], [profondeur de champ]. [Imperfections]. [Style]. [Négatifs].
```

**Exemple** :
"Close-up of weathered hands of a 60-year-old man holding a small blue water filter straw (~20cm) over a stream. Natural overcast daylight, soft shadows. Shot on iPhone Pro, slight digital noise, candid documentary style. Slight motion blur on the water. No studio lighting, no perfect composition, no advertisement look. 9:16 vertical format."

### Template UGC/selfie
```
Ultra-realistic [cadrage] selfie of [persona], captured as if on iPhone Pro front camera. [Environnement]. [Éclairage]. [Imperfections : grain, flou, angle]. Raw unfiltered UGC style. No beauty retouching, no studio, no model.
```

### Template produit B-roll
```
[Cadrage] of [produit avec description physique précise] [action/position] in [contexte d'usage réel]. [Éclairage]. [Caméra]. [Détails texture]. [Imperfections]. No text, no logo overlay.
```
