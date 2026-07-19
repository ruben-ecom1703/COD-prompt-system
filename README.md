# COD-prompt-system

Système de référence pour la génération de prompts B-roll par le SaaS interne.

**Lu en live par le SaaS** — chaque modification ici est prise en compte automatiquement (cache 15 min).

## Structure

```
formats/           → une fiche par format vidéo (style visuel, mots-clés, erreurs interdites)
  native-ads.md
  mockup-3d.md
  cartoon.md
  ugc-ia.md
  vsl.md
best-practices.md  → règles générales de prompt engineering (injecté systématiquement)
prompt-learnings.md → learnings accumulés au fil du temps (ce qui marche / ce qui ne marche pas)
```

## Comment mettre à jour

1. Éditer le fichier directement sur GitHub (bouton crayon)
2. Commit
3. Le SaaS utilise la nouvelle version à la prochaine génération (max 15 min de délai)

Pas besoin de redéployer le SaaS.
