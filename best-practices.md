# Best Practices — Prompts B-roll IA

> Règles générales appliquées à TOUS les prompts, quel que soit le format. Injecté systématiquement par le SaaS.

## Règle #1 : UN concept = UNE idée visuelle

Chaque prompt doit décrire UNE SEULE scène, UN SEUL plan. Pas de prompt qui essaie de raconter une histoire en une image. Si le concept a plusieurs éléments, les séparer en plusieurs prompts distincts.

**Bon** : "Gros plan sur des mains d'homme âgé tenant le filtre Hydra X2 bleu au-dessus d'un ruisseau, lumière naturelle"
**Mauvais** : "Un homme au bord d'un ruisseau qui filtre l'eau puis la boit et sourit de satisfaction avec sa famille en arrière-plan"

## Règle #2 : Toujours spécifier l'échelle du produit

Le produit doit TOUJOURS être décrit avec une référence de taille dans le prompt (dans une main, à côté d'une bouteille, dans une poche). Sans ça, l'IA invente la taille et se trompe presque toujours.

## Règle #3 : Commencer par le cadrage, finir par l'ambiance

Structure d'un bon prompt :
1. **Type de plan** (gros plan, plan moyen, POV...)
2. **Sujet principal** (quoi/qui est dans l'image)
3. **Action/pose** (ce que le sujet fait)
4. **Environnement** (où ça se passe)
5. **Éclairage** (type de lumière)
6. **Style/mood** (ambiance, grain, qualité)

## Règle #4 : Inclure les "négatifs"

Toujours préciser ce qu'on NE veut PAS en plus de ce qu'on veut. L'IA a des biais par défaut (fond blanc, éclairage studio, visages parfaits) — les contrer explicitement.

## Règle #5 : Cohérence entre les plans d'une même vidéo

Tous les prompts d'une même vidéo doivent partager :
- Le même style visuel (pas de mix réaliste + cartoon)
- La même palette de couleurs dominante
- Le même niveau de qualité/grain
- Le même type de cadrage général
- Le même persona si un personnage apparaît

## Règle #6 : Le marché cible dicte le décor

Toujours adapter l'environnement au marché :
- Hongrie → intérieurs d'Europe de l'Est, petites villes hongroises, jardins, campagne. JAMAIS de décor américain
- France → intérieurs français typiques, pas de McMansion américaine
- Le décor se lit en 0,5 seconde — un frigo américain ou un pavillon US crée une dissonance immédiate

## Règle #7 : Produit fidèle au réel

Ne JAMAIS inventer le design du produit. Toujours décrire le produit tel qu'il est réellement (couleur, forme, taille, marquages). Si l'info physique n'est pas dans la data marque, ne pas deviner — demander.

## Règle #8 : Pas de texte dans l'image

Sauf indication contraire explicite dans le concept, ne pas demander de texte/mots/chiffres dans l'image générée. Les modèles d'image IA génèrent du texte illisible ou déformé dans 90% des cas. Le texte sera ajouté en post-production par le monteur.
