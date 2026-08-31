# CHANGELOG

## 2026-08-31 — sync : règle de pilotage stock/ROAS (10-operations.md)

- Source : conversation Claude du 2026-08-21 (même session déjà partiellement synchronisée le 22/08).
- `10-operations.md` : rythme observé ~14 commandes/jour depuis réception stock + règle de pilotage actée par Ruben (repasser commande fournisseur maintenant, avant tout scaling).
- **Non ajouté / détecté mais ignoré** : ROAS post-réception (6,55x puis 6,57x) et les deux seuils ROAS de la règle de pilotage (stabiliser entre 2-3x, couper vers 1,69x) — même filtre bloquant coûts/marges/unit economics déjà appliqué au sync du 22/08 pour cette marque. **À noter pour Ruben** : le repo Nomad Labs documente régulièrement le ROAS comme métrique de perf (06-resultats.md) — incohérence entre marques à trancher si le filtre doit s'appliquer uniformément ou pas.

## 2026-08-22 — sync : mise à jour stock post-réception (10-operations.md)

- Source : vault Obsidian `_context.md` (section 2026-08-21)
- `10-operations.md` : 163 commandes écoulées depuis réception du stock (279 articles, 1,71 art./cmd), stock restant estimé ~1 721 unités, 3 000 unités supplémentaires en transit (arrivée ~2-3 semaines), possibilité de repasser commande (délai production ~2 semaines), discussion scaling en cours avec Geoffrey (non tranchée)
- **Non ajouté / détecté mais ignoré** : chiffres de CA, dépense pub, AOV, ROAS et profit estimé de la même section — filtre bloquant coûts/marges/unit economics
- **Non ajouté** : configs CommentGuard Onela (modération commentaires) — déjà stockées séparément dans le vault, pas de section dédiée dans la structure du repo (même remarque que les syncs précédents)

## 2026-08-12 — sync : stock + blocage Rapid-Ads (10-operations.md), index headlines dans 05-ads.md

- Source : vault Obsidian `_context.md` (sections 2026-08-07 et 2026-08-10)
- `10-operations.md` : premier remplissage du template — stock 2 000 unités / 714 commandes possibles, fenêtre cible 35-45j = 16-20 cmd/j, comparatif Keskia ; note du blocage lancement Rapid-Ads du 07/08 (mismatch compte pub) et son fix
- `05-ads.md` : ajout d'un pointeur vers `ads/headlines-native-ads.md` (pack déjà pushé en direct le 2026-08-07, commits `a216e08`→`f24f298` — non re-documenté ici, seulement indexé)
- **Non ajouté** : configs CommentGuard (rédigées 2026-08-06) — pas de section dédiée dans la structure du repo, à trancher avec Ruben avant d'en créer une (même remarque que pour Keskia/Nomad Labs)

## 2026-07-30 — sync : rattrapage 07-23/24 (brand/concurrent/angles/ads/résultats/funnel) + nouveau lot scripts

- Rattrapage : contenu rédigé les 2026-07-23/24 mais resté non commité jusqu'ici — `01-brand.md`, `02-concurrent.md`, `04-angles-personas.md`, `05-ads.md`, `06-resultats.md`, `09-site-funnel.md` (commit 835a32d)
- `05-ads.md` : ajout de l'index vers [ads/scripts-native-ads.md](ads/scripts-native-ads.md) — 16 nouveaux scripts native ads long-form (rédigés 2026-07-24, jamais commités), 5 angles × 5 frameworks (Test à jeun, Gaslighting, Autorité pédago, Insider dissident, Cycle échec-espoir), répondant directement aux gaps notés dans les Learnings créatives (diversification angle, POV insider/confession)
- ⚠️ Traduction hongroise et diffusion réelle encore à faire — notes /10 sont des auto-évaluations rédactionnelles, pas de perf confirmée

## 2026-07-18 — sync : angles, perf, plan de relance (04/06/07)

- Sources archivées : `data/exports-meta/CLN_0428-KN-3---Nomadsla-s-Ads-1-Jun-2026-30-Jun-2026.csv` + `data/notes-sessions/2026-07-17-collecte-initiale.md` + `data/notes-sessions/2026-07-17-site-live-fetch.md`
- `04-angles-personas.md` : contexte du format cartoon testé (rentable mais peu), pas de mapping ad-par-ad disponible (export créatives différé par Ruben) ; 3 angles concurrents (Lyveli) identifiés comme pistes à tester
- `06-resultats.md` : perf complète des 20 ads (total $346.40, 20 achats), désambiguïsation par Ad ID (plusieurs noms dupliqués)
- `07-relance.md` : plan priorisé (scaler Ads 4/Ads 2, diversifier les angles, tester les angles Lyveli)
- ⏳ **Hors scope de ce sync** : `01-brand.md`, `02-concurrent.md`, `03-compliance.md`, `05-ads.md`, `08-brand-system.md`, `09-site-funnel.md`, `README.md` restent en template — remplis par le prompt de build dédié, pas par cette routine. Le site live (offre 3 paliers, FAQ 6 Q/R, preuve sociale) et le concurrent Lyveli sont déjà collectés dans les notes de session archivées, prêts pour ce build.

## {DATE} — Création du repo (build initial)

- {résumé du build}
