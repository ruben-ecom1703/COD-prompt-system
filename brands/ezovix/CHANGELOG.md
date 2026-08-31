# CHANGELOG — journal des mises à jour du repo

> Toute mise à jour du repo s'inscrit ici, datée, la plus récente en haut. Seul le gérant de la brand (Hugo) écrit dans ce repo.

## 2026-08-30 (cod-sync) — Campagnes relancées le 29/08 sur le nouveau BM Abu 3

- `10-operations.md` + `07-relance.md` : compte publicitaire confirmé `CLN_0645-KN-6` (ID `1588269252528563`, owned by CLNG4), désormais rattaché au BM opérationnel **Abu 3** (remplace Lydia Martinez, restreinte le 26/08) — alias « COD 3.0 » sur Kuronet. Campagnes relancées par Hugo le 29/08. ⚠️ Statut du plafond de dépense non reconfirmé (le compte affichait encore $0,00 dépensé au 28/08).
- Filtré (bloquant) : rien — aucune unit economics/COGS/marge, aucun identifiant/secret, aucun lien `[[wiki]]`. Vérif liens/ancres : 0 cassé.

## 2026-08-06 (cod-sync) — Couverture stock estimée à la relance

- `10-operations.md` : nouvelle section couverture stock (06/08) — 3 000 unités arrivant fin août, ~46 j de couverture dès la relance (~01/09), seuil de réassort atteint quasi immédiatement, à décider avant la deadline Q4 mi-septembre.
- Filtré (bloquant) : rien — aucune unit economics/COGS/marge, aucun identifiant, aucun lien `[[wiki]]`.

## 2026-07-15 (cod-sync) — Packaging/stock + anti-rejet Meta

- `10-operations.md` : packaging à refaire avant relance (nouveau design, puis production/livraison) → stock disponible fin août, ralenti par le typhon en Chine.
- `07-relance.md` : nouvelle section anti-rejet Meta (post ID organique, sous-domaine tampon clean, agency ad account) — retour d'un call groupe du 14/07 sur un cas vécu par une autre brand santé.

## 2026-07-14 (v2.1) — Corrections issues du test d'audit

Un agent testeur n'ayant QUE ce repo a passé 7 questions types et audité la cohérence. Corrections appliquées :

- 🔴 **Posologie** : `01-brand.md` donnait encore « 2 cseppentő ×2/jour » + « incohérence jamais tranchée » alors que `09` avait tranché (1 pipette, 1-2×/jour). **Un membre aurait écrit un dosage faux dans une pub santé.** Corrigé + lien canonique posé.
- 🔴 **« ROAS 18,48 » de l'angle objection-prix : supprimé** — ce chiffre venait d'un regroupement du sheet d'audit qui mélangeait une vidéo avec `Krónikus Toroknyák`, qui est en réalité le 4e visuel de l'advertorial winner. Le **tableau des angles a été reconstruit** depuis les exports bruts : chaque ligne est désormais adossée à des copies identifiées (total 281,33 $ / 50 ventes ✅).
- 🔴 **Ad #8 (Barrett) était attribuée à Labor** dans `04` et `05` alors qu'elle tournait sur **Hálózat** (confirmé par l'export brut). Corrigé.
- 🟠 `data/ads.json` : perf manquante sur #8 et #9 (bug d'encodage Unicode sur les accents) → corrigé, schéma désormais uniforme (`null` explicite).
- 🟠 Fichier fantôme `visuels/videos/.mp4` (10 Mo, invisible) et `GLOSSAIRE.md` tronqué/orphelin (doublon du glossaire du README) : supprimés.
- 🟡 Le winner = **4 visuels / 37 ventes / 74 %** (et non 3 / 35 / 70 %) — `#20` en faisait partie. Aligné partout.
- 🟡 Flux COD unifié de bout en bout dans `09` (renvoi depuis `10`). Profil concurrent daté et renvoyé vers la veille.
- 🟡 Chaque fiche d'ad porte désormais une section **« Visuels dans ce repo »** (visuel publié + créas de relance + vidéos) au lieu de renvoyer vers Notion.

## 2026-07-14 (v2) — L'annuaire complet

- **`ads/` : les 20 copies intégrales** rapatriées de Notion (HU + FR + brief visuel + débrief + diagnostic + résultat testing par ad). Index : `ads/README.md`.
- **`06-resultats.md` enrichi** : perf recalculée depuis les exports bruts — spend/ventes/revenue/ROAS **par page** (Labor 236,66 $ → 43 v · Hálózat 44,67 $ → 7 v) + le **tableau des 20 ads** avec le spend réel de chacune (y compris les 0-vente : c'est ce qui prouve « non-testé » ≠ « loser »).
- **`08-brand-system.md`** (nouveau) : code couleur exact du site (teal `#1a8a8f`, or CTA `#e0a52a`…), typos, style codifié des créas, ton de voix HU (tegező), conventions de nommage.
- **`09-site-funnel.md`** (nouveau) : le site section par section, buy box, FAQ verbatim, **posologie tranchée** (1 pipette 1-2×/j), funnel COD. + screenshots dans `assets/site/`.
- **`10-operations.md`** (nouveau) : compte pub, pages, logistique COD (hub Slovaquie, utánvét), stack, qui gère quoi. Sans marges ni accès (décision Hugo).
- **`02-concurrent.md`** : section **Veille datée** — NanoRevive au 14/07 (665 ads actives, 225K visites/mois) + 🆕 leur nouvel angle du 14/04 « The Part Your Acid Blocker Can't Fix » (candidat itération n°1).
- **`data/`** : exports Meta bruts (créas + perf) + **`ads.json`** (data structurée des 20 ads pour les outils/IA).
- **`visuels/videos/`** : les 4 vidéos d'ads compressées (lisibles depuis GitHub).
- **README v2** : carte de routing enrichie (28 entrées), **timeline de la brand**, **glossaire** (LPR, pepsine, utánvét, ROAS…).

## 2026-07-14 (bis) — Visuels des ads réellement publiées + logos pages FB

- Ajout `visuels/ads-testees/` : les 16 visuels de prod du testing (dont les 3 winners blueprint / GERD vs LPR / Nyákcsapda), **mappés sur les ventes/ROAS réels** dans la galerie.
- Ajout `assets/logos-pages-fb/` : logos Labor + Hálózat (transparent + 4 fonds couleur).
- Vidéos Vmake NON incluses (1 fichier > 100 Mo, limite GitHub) — emplacement + résultats documentés dans la galerie.
- Repo renommé `ezovix` → `COD-ezovix` (convention de nommage : préfixe COD).

## 2026-07-14 — Création du repo

- Structure initiale complète : README (sommaire + carte de routing), 01-brand, 02-concurrent, 03-compliance, 04-angles-personas, 05-ads, 06-resultats, 07-relance.
- Données de référence : audit du 13/07/2026 (croisement exports Meta créas × perf, campagne « 03/07/26 - Ezovix - Testing », fenêtre jusqu'au 12/07/2026).
- 47 visuels natives (6 angles Adset 2, générés le 03/07/2026) compressés en JPG.
- Excel `data/Ezovix-DATA-ADS.xlsx` (format 3 onglets : Classement Angles · Créa winneuse · Vue Globale, version corrigée du 13/07).
- Domaine `ezovix.shop` vérifié en ligne le 14/07/2026.
