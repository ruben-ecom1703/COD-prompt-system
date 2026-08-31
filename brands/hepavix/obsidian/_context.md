# Hepavix — Gyógyszerészeti Minőségű Májvédelem és Regeneráció

Complément alimentaire de protection et régénération hépatique, marché hongrois.

- **Site / PDP** : https://hepavix.com/products/hepavix-gyogyszereszeti-minosegu-majvedelem-es-regeneracio
- **Nom produit** : Hepavix – Gyógyszerészeti Minőségű Májvédelem és Regeneráció
- **Tagline** : « A májformula, amiről mindenki beszél »
- **Note** : la marque est parfois appelée « Epavix » à l'oral — le nom réel et le domaine sont **Hepavix** / hepavix.com.

## Produit

- **Actifs** : Máriatövis (90% szilimarin) · N-Acetil-Cisztein (NAC) · Kolin (bitartarát)
- **Positionnement** : doses cliniques, « no filler », testé en labo indépendant, 32+ études citées
- **Posologie** : napi 2 kapszula étkezéshez (2 gélules/jour au repas) — 1 flacon = 30 jours
- **Bénéfices mis en avant** : protection + régénération du foie, énergie & clarté mentale, inflammation, métabolisme des graisses, détox alcool, moins de ballonnements et de brouillard mental

## Pricing & Offre (Hongrie, HUF)

| Palier | Prix | Barré | Coût/jour | Inclus |
|---|---|---|---|---|
| 1 üveg | 12 400 Ft | 18 500 Ft | ~413 Ft/nap | — |
| **2+1 INGYEN** ⭐ | 20 900 Ft | 37 200 Ft | ~232 Ft/nap | Ingyenes szállítás + **2 e-könyv** |
| 3+2 INGYEN | 27 900 Ft | 62 000 Ft | ~186 Ft/nap | Ingyenes szállítás + **2 e-könyv** |

- **Garantie** : 60 napos pénzvisszafizetési garancia — « Ha nem érzed a különbséget, küldd vissza teljes árvisszatérítésért. Még üres üvegekkel is. Kérdés nélkül. »
- **Social proof** : 4,8/5 — 2 184 avis vérifiés (Trustpilot). Répartition : 1 878 × 5★, 218 × 4★, 52 × 3★, 22 × 2★, 14 × 1★.

## E-books (cadeaux post-achat)

2 e-books offerts à partir de **2 flacons** (donc paliers 2+1 et 3+2 uniquement — jamais le palier 1 üveg). PDF reçus et lus le 2026-08-06, source : `~/Downloads/hepavix ebook hu/`.

**1. « A májdetox útmutató »** — 25 pages · 7 chapitres · valeur affichée **9 990 Ft**
1. Hogyan méregtelenít a máj — 500+ tâches quotidiennes, les 2 phases de détox, le glutathion
2. Mi terheli a májat — **alcool en tête**, puis sucre/fructose (NAFLD), aliments transformés, médicaments, environnement, stress, manque de sommeil ; les 4 stades du foie gras
3. A túlterhelt máj jelei — 6 signes (fatigue, digestion, peau, réveil, appétit, irritabilité) + les symptômes qui relèvent du médecin
4. Étrend a májért — crucifères, ail/oignon, verts, betterave, poisson gras, noix, thé vert ; assiette 50/25/25
5. Életmód és szokások — 30 min/jour, 7-8 h de sommeil, eau, stress, alcool
6. A kulcstápanyagok — szilimarin / NAC / kolin, et « a dózis számít »
7. **A 14 napos terv** — 6 paliers (folyadék → tányér → mozgás → alkohol → alvás → összegzés)

**2. « Energia és emésztés természetesen »** — 25 pages · 7 chapitres · valeur affichée **6 990 Ft**
1. Honnan jön az energia — le trajet en 5 étapes, mitochondries, glycémie
2. Mi rabolja el az energiát — glycémie, déshydratation, caféine (pas de café après 14 h), sommeil, stress, foie surchargé
3. Az emésztés alapjai — bouche → estomac → grêle → côlon, rôle du foie et de la bile, 4 causes de ballonnements
4. Étrend a stabil energiáért — fehérje + rost + jó zsír, **l'ordre des aliments compte**, le petit-déjeuner
5. A bélrendszer és a bélflóra — ~70% de l'immunité, axe intestin-cerveau, pré/probiotiques
6. Napi ritmus és alvás — horloge interne, 10 min de marche après le repas
7. **A 7 napos energiaterv** — 1 étape par jour (víz → reggeli → tányér → séta → koffein → bélflóra → alvás)

Les deux se terminent par un disclaimer légal (complément alimentaire, pas un médicament) et la mention « 60 napos garancia · Magyar nyelvű ügyfélszolgálat ».

Promesse affichée sur la PDP : *« E-mailben küldjük a rendelés után, azonnali letöltéssel »* → **l'e-mail doit partir immédiatement après la commande**.

## 2026-08-06

- Récupération de toute la data PDP (produit, pricing 3 paliers, e-books, garantie 60j, social proof) → fiche ci-dessus.
- **Flow e-mails de livraison des e-books rédigé** → `flow-emails-ebooks.md` dans ce dossier. 2 e-mails (J+0 / J+1), HU + FR, avec la config de flow et le filtre bundle en amont.
- Filtre décidé par Ruben : ne déclencher le flow que sur les commandes contenant un bundle (2+1 ou 3+2), le palier 1 flacon n'ouvrant pas droit aux e-books.
- Les PDF ne sont pas encore hébergés — Ruben reçoit les liens par mail et va les télécharger. Placeholders `{{ LIEN_EBOOK_1 }}` / `{{ LIEN_EBOOK_2 }}` dans les e-mails en attendant.
- Modèle de référence : le flow e-books **Aurivo** (2 e-books, J+0 science / J+1 pratique, ton éducatif-marque, hongrois tegező) — voir `1 Terrains/COD Empire/Aurivo/_context.md`. Nomad Labs a 3 e-books dans son offre mais **aucun flow d'envoi documenté** à ce jour.
