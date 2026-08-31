# 06 — Résultats réels du testing (vérifiés)

> 📅 Dernière mise à jour : 2026-07-14 · Statut : ads à l'arrêt (plafond compte `CLN_0645 - KN - 6`) · Gérant : Hugo
> Campagne : « 03/07/26 - Ezovix - Testing » (lancée le 04/07/2026) · Fenêtre mesurée : jusqu'au 12/07/2026 · Vérifié le 13/07/2026

**Ce que contient ce fichier :**
- La méthode de vérification (zéro donnée inventée)
- Le comparatif des 4 brands testées — **Ezovix = n°1**
- Les 10 ads qui ont vendu (IDs, ventes, coût/vente, ROAS)
- **Le test le plus instructif** : 3 winners = la même copy, seul le visuel change
- Les learnings et les 3 lois prouvées sur les 4 brands

**Sommaire** : [Méthode de vérification](#méthode-de-vérification) · [Comparatif des 4 brands](#comparatif-des-4-brands) · [Les ads qui ont vendu](#les-ads-qui-ont-vendu) · [Le test le plus instructif](#le-test-le-plus-instructif) · [Les pages](#les-pages) · [Learnings](#learnings) · [Les 3 lois du portefeuille](#les-3-lois-du-portefeuille) · [État du compte](#état-du-compte)

---

## Méthode de vérification

Tous les chiffres de ce fichier viennent du croisement de **deux exports Meta bruts** (13/07/2026) :
- **Export créas** `export_20260713_0840.xlsx` — contient la copy, les Ad IDs et la colonne `Link Object ID` (= la page FB qui diffuse l'ad).
- **Export perf** `CLN_0645---KN---6-Ads-13-Jun-2026-12-Jul-2026.csv` — `Purchases`, `Amount spent`, `Purchase ROAS`.

⚠️ **Croisement toujours sur le couple nom d'ad + ad set** (plusieurs ads portent le même nom dans des ad sets différents — croiser sur le nom seul fait perdre des ventes). Le détail par angle est aussi dans l'Excel [data/Ezovix-DATA-ADS.xlsx](data/Ezovix-DATA-ADS.xlsx) (3 onglets : Classement Angles · Créa winneuse · Vue Globale).

## Comparatif des 4 brands

**EZOVIX EST LA MEILLEURE DES 4 BRANDS TESTÉES.**

| | **Ezovix** | Hepavix | Aurivo | Nuvalis |
|---|---|---|---|---|
| **ROAS global** | **10,81** 🥇 | 8,83 | 6,07 | 5,14 |
| Ventes | 50 | 41 | 37 | 25 |
| Dépensé | 281,33 $ | 306,95 $ | 325,59 $ | 324,12 $ |
| Revenue | 3 040,11 $ | 2 710,99 $ | 1 974,79 $ | 1 667,32 $ |
| **Taux de winner** | **10/20 = 50 %** 🥇 | 4/17 = 24 % | 8/26 = 31 % | 6/26 = 23 % |

**1 ad sur 2 a vendu.** Aucune autre brand n'approche ça. À la relance, Ezovix passe en premier.

## Les ads qui ont vendu

10 ads sur 20 ont fait au moins 1 vente :

| Rang | Ad | Ad ID | Page | Ventes | Coût/vente | ROAS |
|---|---|---|---|---|---|---|
| 🏆 1 | Static - A Torok Amely Nem Ürül Ki *(blueprint)* | `120246113936180014` | Labor | **18** | 4,54 $ | 13,36 |
| 🥈 2 | Static - GERD vs LPR (v1) | `120246113936040014` | Labor | 9 | **3,70 $** | **15,24** |
| 🥉 3 | Static - A Nyákcsapda | `120246113936150014` | Labor | 8 | 10,37 $ | 6,18 |
| 4 | Photo IA Réaliste Graduation | `120246114383960014` | Hálózat | 5 | 4,41 $ | 13,69 |
| 5 | Vmake AI Vidéo Hongroise (2) | `120246113937620014` | Labor | 4 | 3,08 $ | 18,78 |
| 6 | Static - Krónikus Toroknyák | — | Labor | 2 | 4,52 $ | 18,08 |
| 7 | Static - Miért Köhögtem 200x | — | Labor | 1 | 4,42 $ | 10,25 |
| 7 | Vmake AI Vidéo Hongroise (1) | — | Labor | 1 | 3,65 $ | 12,41 |
| 7 | Vidé 2 | — | Hálózat | 1 | 2,80 $ | **25,14** |
| 7 | hf_20260703_095722… *(globus)* | — | Hálózat | 1 | 10,40 $ | 6,77 |

## Le test le plus instructif

**Quatre ads (18 + 9 + 8 + 2 = 37 ventes, soit 74 % du total) ont EXACTEMENT le même texte** — mot pour mot, les 8 048 caractères de l'advertorial LPR d'Ágnes K. ([copy intégrale](ads/05-lpr-image-c-blueprint.md)) — sur la même page (Labor). **Seul le VISUEL change** :

| Visuel | Copy | Spend | Ventes | Coût/vente | ROAS | Panier moyen |
|---|---|---|---|---|---|---|
| **Blueprint** (plan d'architecte bleu, coupe gorge + mucus) | [#5](ads/05-lpr-image-c-blueprint.md) | 81,69 $ | **18** | 4,54 $ | 13,36 | 60,65 $ |
| **GERD vs LPR** (infographie « la flamme vs le brouillard ») | [#2](ads/02-lpr-image-b-gerd-vs-lpr.md) | 33,33 $ | 9 | **3,70 $** | **15,24** | 56,39 $ |
| **A Nyákcsapda** (gravure anatomique ancienne, parchemin) | [#1](ads/01-lpr-flagship.md) | 82,98 $ | 8 | 10,37 $ | 6,18 | **64,09 $** |
| **Krónikus Toroknyák** (mucus chronique) | [#20](ads/20-advertorial-image-c-kronikus.md) | 9,03 $ | 2 | 4,52 $ | 18,08 | — |

Le coût/vente va **du simple au triple (3,70 $ → 10,37 $) à copy strictement identique**. Conclusion : **sur une bonne copy, le visuel décide de tout le reste.**

⚖️ **Les 4 sont rentables — on n'en coupe AUCUNE.** C'est une question d'allocation de budget, pas de coupe. Règle validée par Hugo : **le juge d'une ad = le ROAS (+ profit net), jamais le coût/vente isolé** — A Nyákcsapda a le pire CPA mais le panier moyen le plus haut (64 $) et reste profitable.

## Les pages

Data complète par page, recalculée depuis les exports bruts le 14/07 (les sommes tombent juste : 236,66 + 44,67 = 281,33 $ · 43 + 7 = 50 ventes) :

| Page FB | ID | Ads | **Spend** | Ventes | Revenue | ROAS | Coût/vente |
|---|---|---|---|---|---|---|---|
| **Emésztési Egészség Labor** (autorité) 🏆 | `1155025737700054` | 10 | **236,66 $** | **43** | 2 597,59 $ | **10,98** | 5,50 $ |
| Természetes Emésztési Egészség Hálózat (communauté) | `1212951778564210` | 10 | **44,67 $** | 7 | 442,52 $ | 9,91 | 6,38 $ |

**Lecture honnête** : Labor a fait **6× plus de ventes** (43 vs 7) — mais elle a aussi reçu **5,3× plus de budget**. Au ROAS, les deux pages sont rentables (10,98 vs 9,91 — Hálózat sauvée par Graduation et Vidé 2). La vraie conclusion : **Labor est prouvée à l'échelle, Hálózat est sous-testée** — et les récits de l'Adset 2 n'ont jamais eu leur chance (< 3 $ chacun). Le signal « la page persona autorité vend plus » reste vrai au niveau du portefeuille (preuve nette chez Aurivo : même copy, 28 ventes page médecin vs 1 page marque).

### Détail Labor — 10 ads (236,66 $ · 43 ventes)

| Ad Meta | Copy ([fiche](ads/README.md)) | Spend | Ventes | Coût/vente | ROAS |
|---|---|---|---|---|---|
| Static - A Torok Amely Nem Ürül Ki *(blueprint)* 🏆 | #5 (flagship Ágnes K.) | 81,69 $ | **18** | 4,54 $ | 13,36 |
| Static - A Nyákcsapda | #1 (flagship, img Phlegm Trap) | 82,98 $ | 8 | 10,37 $ | 6,18 |
| Static - GERD vs LPR (v1) | #2 (flagship, img B) | 33,33 $ | 9 | **3,70 $** | **15,24** |
| Vmake AI Vidéo Hongroise (2) | famille STOP BURNING (#15/16/18*) | 12,32 $ | 4 | 3,08 $ | 18,78 |
| Static - Krónikus Toroknyák | #20 (flagship, img C) | 9,03 $ | 2 | 4,52 $ | 18,08 |
| Static - Az Év Legnagyobb Akciója (promo 2+1) | #7 | 5,83 $ | 0 | — | ❌ static produit |
| Static - Miért Köhögtem 200x | #6 | 4,42 $ | 1 | 4,42 $ | 10,25 |
| Vmake AI Vidéo Hongroise (1) (1) | famille STOP BURNING* | 3,65 $ | 1 | 3,65 $ | 12,41 |
| Vmake AI Vidéo Suppresseur Hongrois (2) | famille STOP BURNING* | 2,29 $ | 0 | — | ⚪ |
| Static - 11 összetevő (aloe vera) | #3 | 1,12 $ | 0 | — | ❌ static produit |

### Détail Hálózat — 10 ads (44,67 $ · 7 ventes)

| Ad Meta | Copy ([fiche](ads/README.md)) | Spend | Ventes | Coût/vente | ROAS |
|---|---|---|---|---|---|
| Photo IA Réaliste Graduation | #8 (Barrett/gastroscopie) | 22,05 $ | **5** | 4,41 $ | 13,69 |
| hf_20260703_095722… | #10 (globus) | 10,40 $ | 1 | 10,40 $ | 6,77 |
| Vidé 2 | UGC (#17 ou #19*) | 2,80 $ | 1 | 2,80 $ | **25,14** |
| AI Images from Text & Photo (9) | #13 (contagieux) | 2,76 $ | 0 | — | ⚪ jamais testé |
| hf_20260703_101950… | #12 (antiacides, TAM #1) | 2,35 $ | 0 | — | ⚪ jamais testé |
| Static - A Rejtett Enzim | #4 (chanteuse) | 1,76 $ | 0 | — | ⚪ jamais testé |
| Homme Hongrois Réaliste en Pleurs (1) | #9 (nocturne) | 1,04 $ | 0 | — | ⚪ jamais testé |
| Vidé 1 | UGC (#17 ou #19*) | 0,78 $ | 0 | — | ⚪ jamais testé |
| Higgsfield AI Images 2026-07-03 | #14 (prisonnier IPP) | 0,70 $ | 0 | — | ⚪ jamais testé |
| AI Images from Text & Photo (8) | #11 (faux infarctus) | 0,03 $ | 0 | — | ⚪ jamais diffusé |

> Mapping copy ↔ ad Meta : par titre du visuel ou par spend exact croisé avec le tableau des angles (détail par copy dans [data/ads.json](data/ads.json)). Les lignes marquées `*` (vidéos) = correspondance exacte au numéro de copy **à confirmer par Hugo**.

⚠️ **Conséquence directe** : tous les récits de l'Adset 2 (la chanteuse, les 20 ans d'antiacides, les 3 faux infarctus, la boule dans la gorge, le prisonnier de la pilule, les 2 ans sans dormir) tournaient **uniquement sur la page la moins financée**, avec **moins de 3 $ de budget chacun**. Ce ne sont **pas des losers — ce sont des non-testés** (plan de rattrapage dans [07-relance.md](07-relance.md)).

## Learnings

- **Le format « odyssée du mauvais diagnostic » est LE format gagnant** : 70 % des ventes (advertorial 15 temps, cf. [02-concurrent.md](02-concurrent.md#squelette-advertorial-15-temps)).
- **L'angle « on t'a menti sur la cause »** : ce n'est pas une allergie, ni de l'asthme — c'est ton œsophage. Et ce n'est pas l'acide, **c'est la pepsine**.
- **Le « cimetière de solutions » est le pivot de la copy** : elle a tout essayé, et chaque solution a échoué à cause du FORMAT. Le produit ne fait pas mieux, **il fait autrement** (liquide qui reste sur le tissu vs gélule qui tombe dans l'estomac).
- **Le visuel gagnant = un SCHÉMA MÉDICAL, pas une pub** : blueprint, infographie, gravure anatomique. Aucun produit, aucun prix, aucun visage.
- **Les statics produit : 0 vente** (angles 13-14). Quand on montre le produit, on ne vend pas.

## Les 3 lois du portefeuille

Prouvées 4 fois (Ezovix, Hepavix, Aurivo, Nuvalis) :

1. **L'angle qui gagne = « on t'a menti sur la cause. »** Le vrai coupable est ailleurs et personne ne te l'a dit : la pepsine (Ezovix) · le foie (Hepavix) · l'inflammation (Aurivo) · les mitochondries (Nuvalis). Ne jamais partir d'un symptôme vague — viser quelqu'un qui a une opération programmée, un antiacide dans chaque poche, ou 5 médecins qui n'ont rien trouvé.
2. **La page persona vend, la page de marque ne vend pas.** Ezovix : Labor 43 vs Hálózat 7. Preuve la plus nette (Aurivo) : la même copy fait 28 ventes sur la page médecin et 1 sur la page marque.
3. **À copy identique, le visuel décide de tout.** Le visuel doit montrer L'INSTANT ou PROUVER, jamais décorer. Pour Ezovix : le schéma médical.

## État du compte

- ⚠️ Business Manager (13/07/2026) : **« Your ads have stopped running — you've reached your ad account spending limit for CLN_0645 - KN - 6 »**. Les ads sont à l'arrêt **sur un plafond de dépense du compte, pas sur une décision**. À débloquer avant toute relance.
- Contexte portefeuille : toutes les ads COD sont en pause en attente du nouveau stock (état au 13/07/2026).

---

*Navigation : [← 05 — Inventaire des ads](05-ads.md) · [07 — Plan de relance →](07-relance.md)*
