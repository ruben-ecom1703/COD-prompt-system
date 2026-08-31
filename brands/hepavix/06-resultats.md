# 06 — Résultats réels du testing (vérifiés)

> 📅 Dernière mise à jour : 2026-07-14 · Campagne « **26/06/26 Hepavix** » (compte `CLN_0428-KN-5`) · Fenêtre mesurée : 14/06 → 13/07/2026 · Statut : campagne en pause

**Ce que contient ce fichier :**
- La méthode de vérification (zéro donnée inventée)
- Le comparatif des 4 brands — **Hepavix = 🥈 2e**
- **Les 17 ads, une par une** : spend, ventes, coût/vente, ROAS
- La perf **par page Facebook** et **par angle**
- Les learnings et les pièges de lecture

**Sommaire** : [Méthode de vérification](#méthode-de-vérification) · [Comparatif des 4 brands](#comparatif-des-4-brands) · [Les 17 ads](#les-17-ads) · [Par page Facebook](#par-page-facebook) · [Par angle](#par-angle) · [Learnings](#learnings) · [Pièges de lecture](#pièges-de-lecture)

---

## Méthode de vérification

Tous les chiffres viennent du croisement de **deux exports Meta bruts** (fournis le 14/07), archivés dans [data/exports-meta/](data/exports-meta/) :
- **Export de performances** `CLN_0428-KN-5-Ads-14-Jun-2026-13-Jul-2026.csv` — 17 ads : `Purchases`, `Amount spent`, `Purchase ROAS`.
- **Export de créatives** `export-creas-20260713.xlsx` — la copy réellement diffusée, l'`Ad ID`, le fichier image/vidéo, et surtout le **`Link Object ID` = la page Facebook** de chaque ad.

Le croisement se fait sur le **nom d'ad**. **Contrôle réussi** : la somme des 17 ads = **306,95 $ · 41 ventes · 2 710,99 $ de revenue · ROAS 8,83** — exactement les totaux de la campagne. Zéro écart, zéro donnée inventée.

**Les pages Facebook de ce fichier sont lues depuis l'export**, jamais depuis une note. (Sur Ezovix, une ad avait été attribuée à la mauvaise page pendant des semaines faute de ce contrôle.)

## Comparatif des 4 brands

| | Ezovix | **Hepavix** | Aurivo | Nuvalis |
|---|---|---|---|---|
| **ROAS global** | 10,81 🥇 | **8,83** 🥈 | 6,07 | 5,14 |
| Ventes | 50 | **41** | 37 | 25 |
| Dépensé | 281,33 $ | **306,95 $** | 325,59 $ | 324,12 $ |
| Revenue | 3 040,11 $ | **2 710,99 $** | 1 974,79 $ | 1 667,32 $ |
| Taux de winner | 10/20 = 50 % | **4/17 = 24 %** | 8/26 = 31 % | 6/26 = 23 % |

**La particularité d'Hepavix** : la brand tient sur **une seule ad**. Ads 2 fait **36 ventes sur 41 (88 %)** — c'est la concentration la plus extrême du portefeuille. C'est une force (on sait exactement quoi scaler) et un risque (tout repose sur une copy, une page, un visuel).

## Les 17 ads

| Ad | Angle | Page FB | Spend | Ventes | Coût/vente | ROAS |
|---|---|---|---|---|---|---|
| 🏆 [**Ads 2**](ads/cortisol-winner.md) | Cortisol / foie — le ventre qui ne part pas | Dr. Tóth Petra | **250,09 $** | **36** | 6,95 $ | **9,33** |
| [Ads 12](ads/statines-airbnb.md) | Statines / foie — l'hôtesse Airbnb | Varga Nóra | 24,56 $ | 2 | 12,28 $ | 6,35 |
| [Ads 5](ads/offre-ldl-directe.md) | Cholestérol — offre directe | Hepavix (marque) | 2,33 $ | 2 | **1,17 $** | **66,95** ⚠️ |
| [Ads 6](ads/alcool-detox.md) | Alcool / detox | Hepavix (marque) | 3,22 $ | 1 | 3,22 $ | 20,75 |
| [Ads 10](ads/cardiologie-ce-quon-ne-dit-pas.md) | Cholestérol — « ce que la cardiologie ne dit pas » | Dr. Tóth Petra | 13,09 $ | 0 | — | ❌ |
| [Ads 9](ads/offre-ldl-206.md) | Cholestérol — offre (visuel « 206 LDL ») | Hepavix (marque) | 5,96 $ | 0 | — | ❌ |
| [Ads 14](ads/eszter-pere.md) | Eszter — « j'ai regardé mon père disparaître » | Varga Nóra | 2,64 $ | 0 | — | ⚪ |
| [Ads 11](ads/alcool-8-semaines.md) | Alcool — le foie d'un buveur en 8 semaines | Hepavix (marque) | 1,89 $ | 0 | — | ⚪ |
| [Ads 7](ads/offre-ldl-sztatin.md) | Cholestérol — offre (visuel « plus de statine ») | Dr. Tóth Petra | 1,45 $ | 0 | — | ⚪ |
| [Ads 1](ads/ingredient-mariatovis.md) | Ingrédient — le chardon-Marie européen | Hepavix (marque) | 1,18 $ | 0 | — | ⚪ |
| [Ads 15](ads/zsuzsa-fatigue.md) | Zsuzsa — « pendant 2 ans j'ai cru que c'était l'âge » | Varga Nóra | 0,45 $ | 0 | — | ⚪ |
| [Ads 16 (vidéo)](ads/video-cholesterol-statine.md) | Vidéo — cholestérol sous statine | Dr. Tóth Petra | 0,03 $ | 0 | — | ⚪ |
| [Ads 3](ads/alcool-detox-dynamique.md) | Alcool / detox (variante dynamique) | Hepavix (marque) | 0,03 $ | 0 | — | ⚪ |
| [Ads 4](ads/infirmiere-statines.md) | L'infirmière — « sauvez votre cœur » (20 423 car.) | Varga Nóra | 0,03 $ | 0 | — | ⚪ |
| [Ads 8](ads/cortisol-variante.md) | Cortisol — variante dynamique du winner | Dr. Tóth Petra | 0,00 $ | 0 | — | ⚪ jamais diffusée |
| [Ads 17 (vidéo)](ads/video-mariatovis-dilue.md) | Vidéo — chardon-Marie dilué | Dr. Tóth Petra | 0,00 $ | 0 | — | ⚪ jamais diffusée |
| [Ads 15 – Copy 2](ads/zsuzsa-fatigue-copy2.md) | Zsuzsa (duplicata) | — | 0,00 $ | 0 | — | ⚪ jamais diffusée |

**Total : 306,95 $ · 41 ventes** ✅

⚠️ **Ads 5 : ROAS 66,95 sur 2,33 $ de dépense.** C'est le meilleur ROAS affiché, mais sur **deux ventes et deux dollars** — statistiquement, ça ne prouve rien. À reconfirmer avec du budget avant d'en faire une conclusion.

**Lecture des verdicts** :
- ❌ **Testée, n'a pas vendu** = a reçu ≥ 3 $ et n'a rien donné (Ads 10 avec 13,09 $, Ads 9 avec 5,96 $).
  - 💡 **Piste sur l'échec d'Ads 10** (le seul vrai échec financé) : son titre annonce « Comment le LDL de **Katalin** est passé de 5,4 à 4,0 » — mais **Katalin n'apparaît nulle part dans le texte**. Le lecteur clique pour une histoire qu'on ne lui raconte pas. Le même titre orphelin traîne sur Ads 12 ([03-compliance.md](03-compliance.md#défauts-à-corriger-avant-réutilisation)).
- ⚪ **Jamais réellement testée** = moins de 3 $ de budget. **Ce ne sont pas des losers** — elles n'ont jamais eu leur chance. **Elles sont 11**, dont l'infirmière (la plus longue copy de la brand, **3 centimes**) et **Ads 8, la variante du winner, jamais diffusée (0 $)**.

## Par page Facebook

| Page FB | ID | Ads | Spend | Ventes | Revenue | ROAS |
|---|---|---|---|---|---|---|
| **Dr. Tóth Petra Menopauza szakértő** 🏆 | `1082894771584939` | 6 | **264,66 $** | **36** | 2 332,20 $ | 8,81 |
| Hepavix (page marque) | `1188936560969417` | 6 | 14,61 $ | 3 | 222,80 $ | **15,25** |
| Varga Nóra Szexológus | `1276839362173620` | 4 | 27,68 $ | 2 | 155,99 $ | 5,64 |

**Ce que ça dit vraiment — attention à la lecture facile :**
- La page **Dr. Tóth Petra** porte 88 % des ventes. Mais elle a aussi reçu **86 % du budget** : c'est le winner qui a été financé, pas la page. Le mérite revient d'abord à la copy.
- La **page marque a le meilleur ROAS (15,25)** — sur 14,61 $ seulement. C'est contre-intuitif par rapport à la loi du portefeuille (« la page de marque ne vend pas »), et ça a une explication simple : **les ads de la page marque sont des ads d'offre courtes, sans narrateur** — c'est le bon usage d'une page de marque. La loi reste vraie pour les **advertorials** (un récit à la première personne sur une page de marque ne marche pas).
- La page **Varga Nóra (sexologue)** porte l'advertorial d'une **hôtesse Airbnb** : le narrateur ne colle pas à la page. C'est la cause la plus probable de sa sous-performance (2 ventes pour 24,56 $).

## Par angle

Chaque ligne est adossée aux ads qui la composent — pas d'agrégat non traçable :

| Angle | Ads | Spend | Ventes | Verdict |
|---|---|---|---|---|
| **Cortisol / foie — le ventre qui ne part pas** | Ads 2 · Ads 8 | 250,09 $ | **36** | 🏆 WINNER — 88 % des ventes |
| Statines / foie — l'hôtesse Airbnb | Ads 12 | 24,56 $ | 2 | ✅ rentable (ROAS 6,35) |
| Cholestérol — offre directe | Ads 5 · Ads 7 · Ads 9 | 9,74 $ | 2 | ✅ rentable |
| Alcool / detox | Ads 3 · Ads 6 · Ads 11 | 5,14 $ | 1 | ✅ rentable (ROAS 20,75 sur Ads 6) |
| Cholestérol — « ce que la cardiologie ne dit pas » | Ads 10 | 13,09 $ | 0 | ❌ testé, n'a pas vendu |
| Eszter — « j'ai regardé mon père disparaître » | Ads 14 · Ads 17 * | 2,64 $ | 0 | ⚪ jamais testé |
| Ingrédient — le chardon-Marie européen | Ads 1 | 1,18 $ | 0 | ⚪ jamais testé |
| Zsuzsa — la fatigue chronique | Ads 15 (×2) | 0,45 $ | 0 | ⚪ jamais testé |
| Vidéo — cholestérol sous statine | Ads 16 | 0,03 $ | 0 | ⚪ jamais testé |
| L'infirmière — « sauvez votre cœur » | Ads 4 | 0,03 $ | 0 | ⚪ jamais testé |

**Total : 306,95 $ · 41 ventes** ✅

`*` **Ads 17 est classée ici par son TITRE** (celui de l'angle Eszter) — mais **son texte parle du chardon-Marie dilué**. C'est une ad qui mélange deux angles ; elle n'a jamais été diffusée. À trancher avant de la lancer ([03-compliance.md](03-compliance.md#défauts-à-corriger-avant-réutilisation)).

## Learnings

- **L'angle qui gagne, c'est « on t'a menti sur la cause »** : ton ventre ne part pas à cause du cortisol — mais le cortisol reste élevé **parce que ton foie ne l'évacue plus**. C'est le même pattern que les 3 autres brands (la pepsine chez Ezovix, l'inflammation chez Aurivo, les mitochondries chez Nuvalis). **C'est le pattern d'angle le plus rentable du portefeuille.**
- **Le format qui gagne** = l'advertorial long à la première personne, narré par une **autorité médicale**, sur une **page d'autorité médicale**.
- **Le visuel du winner ne montre pas le produit** : c'est un **dessin simple, deux silhouettes de ventre** (un gros qui pend, un plus plat) sur fond blanc. Pas une photo, pas un packshot, pas de prix. Learning #1 de la brand : **le visuel fait la moitié de la performance**.
- **La page doit coller au narrateur.** L'hôtesse Airbnb sur une page de sexologue, c'est une incohérence que le lecteur ressent.
- **Une ad d'offre courte sur la page marque, ça marche** (Ads 5, Ads 6) — c'est le bon usage de la page de marque.
- **Un budget de 3 centimes ne teste rien.** **11 ads** (dont la plus travaillée de la brand, et la variante du winner) sont mortes sans avoir jamais été vues.

## Pièges de lecture

1. **« Ads 5 a un ROAS de 66,95 »** → sur 2,33 $. Ça ne prouve rien encore.
2. **« La page marque est meilleure que la page médecin »** → non : elle a eu 18× moins de budget, et elle porte un autre type d'ad.
3. **« 13 ads sur 17 sont des losers »** → non : 5 n'ont jamais été financées. Seules Ads 10 et Ads 9 ont vraiment échoué avec du budget.
4. **« Le winner dit silymarine 80 %, donc c'est 80 % »** → **NON.** C'est 90 % ([01-brand.md](01-brand.md#ingrédients)). La copy est historique.

---

*Navigation : [← 05 — Inventaire des ads](05-ads.md) · [07 — Plan de relance →](07-relance.md)*
