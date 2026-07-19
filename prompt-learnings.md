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

---

_Ajouter les prochains learnings ci-dessous, toujours avec la date et catégorie (marche / marche pas)._
