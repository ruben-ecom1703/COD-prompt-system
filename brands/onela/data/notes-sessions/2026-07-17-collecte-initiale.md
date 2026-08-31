# ONELA — Notes de collecte initiale (session Claude du 2026-07-17)

**Contexte donné par Ruben (verbatim/paraphrasé) :**

- Format qui a le mieux performé sur le testing : le **format cartoon** (créas avec personnages illustrés — grenouille/crapaud/gecko visibles dans les vignettes Ads Manager). Réadapté "très rapidement" pour Onela — pas un format pensé from scratch pour la marque.
- Résultat du testing : **rentable, mais pas énormément**.
- Point d'optimisation identifié par Ruben : Onela est un produit **mass market**, qui touche une **grosse pain** (mauvaise odeur intime/corporelle) — donc marge de manœuvre importante en diversifiant les angles/créas pour baisser le coût d'acquisition.
- Type de produit : **complément alimentaire → brand à récurrence** (potentiel d'abonnement/reachat, contrairement à Nomad Labs qui est un achat unique de matériel).

**Site produit :** https://onela.shop/products/onela-szagsemlegesito-etrend-kiegeszito
(marché Hongrie — "szagsemlegesítő étrend-kiegészítő" = complément alimentaire neutralisant les odeurs)

**Concurrent identifié par Ruben :** https://lyveli.com/products/complement-anti-odeur (marché FR)

## Export PERF CSV — vérifié

Fichier : `CLN_0428-KN-3---Nomadsla-s-Ads-1-Jun-2026-30-Jun-2026.csv` (période 01–30 juin 2026, 20 lignes d'ads).

- Le préfixe **"Nomadsla-s"** dans le nom de fichier est normal : **le testing Onela et Nomad Labs s'est fait sur le même ad compte partagé** (confirmé par Ruben le 2026-07-17). Aucun chevauchement d'Ad ID entre les deux exports (plage 943xxxxxxx438 pour Onela vs 941xxxxxxx438 pour Nomad Labs) — deux campagnes bien distinctes au sein du même compte.
- ~~Amount spent à 0~~ **Corrigé** : erreur de parsing initiale (split naïf sur virgules, cassé par le champ "Attribution setting" qui contient une virgule entre guillemets). Re-parsé avec un lecteur CSV correct — les montants matchent exactement la capture d'écran de Ruben (Ads 4 = \$120.54, Ads 2 = \$67.70, Ads 1 = \$62.75, etc.). **Total spend juin 2026 : \$346.40 sur 20 ads, ~20 achats (purchases) au total.**
- Top spend / top résultats (triés par dépense) :

| Ad | Ad ID | Spend | Résultats (purchases) | Reach | Coût/résultat |
|---|---|---|---|---|---|
| Ads 4 | 120245943369860438 | $120.54 | 6 | 6 399 | $20.09 |
| Ads 2 | 120245943369900438 | $67.70 | 6 | 4 436 | $11.28 |
| Ads 1 | 120245943163170438 | $62.75 | 2 | 2 784 | $31.38 |
| Ads 13 | 120245943531530438 | $22.77 | — | 1 058 | — |
| Ads 6 | 120245943369880438 | $22.06 | — | 1 212 | — |
| Ads 9 | 120245943473240438 | $6.12 | 3 | 223 | $2.04 |

- Fenêtre du CSV = juin uniquement. À confirmer avec Ruben : le testing s'est-il arrêté fin juin, ou y a-t-il de la donnée de juillet non incluse ?

## Veille concurrent Lyveli (via TrendTrack, 2026-07-17)

3 pages Facebook actives liées à lyveli.com : **Lyveli+** (136 ads actives), **Claire Delattre** (110 ads actives — page au nom de particulier, pattern "advertorial"), **Lyveli +** (53 ads actives). ~300 ads actives cumulées, marché FR.

**Top angle (le plus fort, rank #1-2, 40-44 jours actifs, reach 237k-294k)** — angle "caséum" (tonsil stones), POV confession 1ère personne :
> "Si vous retirez du caséum de votre gorge chaque semaine — parfois chaque jour — il faut absolument que vous lisiez ceci. Parce qu'on vous a probablement expliqué le problème complètement à l'envers..."
→ Landing page dédiée : `lyveli.com/pages/comparatif-solutions-haleine-lyveli`

**2e angle** — origine digestive (pas buccale) de la mauvaise haleine, POV plus direct/vendeur :
> "Tu te brosses les dents… mais ton haleine pue toujours ? C'est peut-être pas ta bouche. Dans la majorité des cas, la mauvaise haleine vient de ton système digestif..."
→ `lyveli.com/pages/try-deos`

**3e angle** — lancement produit Gummies (chlorophylle/menthe/persil), reach 157k, 19j actif, CTA -20% code GUMMIES20 :
→ `lyveli.com/pages/gummies-anti-odeur`

Catalogue Lyveli identifié : Gummies anti-odeur, Gel buccal anti-odeur, Complément anti-odeur (gélules) — plusieurs formats testés en parallèle sur la même pain.

⚠️ Copy complète non reproduite ici au-delà des extraits ci-dessus (droits du concurrent) — pattern uniquement.

---
Source : conversation Claude du 2026-07-17, notes de session Ruben + scan TrendTrack (brief_competitor, search_advertisers, search_ads sur lyveli.com)
