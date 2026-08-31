# resultats — Nomad Labs

> 📅 Dernière mise à jour : 2026-08-31 · Gérant : Ruben

## Scaling par pays (21/08 — 7 jours glissants)

| Marché | ROAS 7j | ROAS veille |
|---|---|---|
| Hongrie | 4,89x | 4,27x |
| Slovaquie | 7,06x | **2,80x** ⚠️ signal faible, à surveiller |
| Tchéquie | 6,82x | 5,01x |
| **Global** | **5,52x** | **4,16x** |

**Constat** : le stock n'est plus le facteur limitant (réappro alimente ~3x plus vite que la conso actuelle, voir [10-operations.md](10-operations.md)) — le vrai frein au scaling est le ROAS, pas le stock. Décision détaillée dans [07-relance.md](07-relance.md).

## Performance Meta Ads (11 juillet – 9 août 2026)

Audit croisant l'export Meta interne, la bibliothèque publicitaire (7 screenshots) et le corpus de scripts du vault.

| Métrique | Valeur |
|---|---|
| Spend (29 j) | **$14 814,77** |
| Achats | **1 745** |
| CPA moyen | **$8,49** |
| ROAS reporté | **11,66x** (revenu commandé ~$172 700) |
| ROAS net réel estimé | **7,5-8x** (taux de livraison COD 65-70 %) |
| Ads à 0 achat | 110 sur 168 — mais seulement $271 de spend cumulé (test large + kill rapide, sain) |

**Progression vs l'audit du 20/07** : ~$218/jour (1-20 juillet) → **~$510/jour**, rythme plus que doublé en dégradant le CPA seulement de $6,59 à $8,49.

### Où part l'argent

| Bloc | Spend | Part | CPA | ROAS |
|---|---|---|---|---|
| Adsets de scale legacy (2 scripts : László + Bolt) | $8 559 | 58 % | $8,57 | 11,65x |
| Batchs de test datés (16/07 → 08/08) | $5 747 | 39 % | $8,43 | 11,65x |
| Vidéo | $769 | 5,2 % | $8,95 | 10,38x |

**Constat central : 58 % du budget tourne encore sur 2 native ads écrites le 12 juin** (László/Voisine et Chauffeur Bolt). Meilleur ratio du compte : Adset 5 BOF/ads 4 — CPA $5,71, ROAS 16,81x, budget sous-financé.

**Signal de fatigue** : le CPA des nouveaux tests est passé de $6,89 (16-25/07) à $17,03 (07-08/08) — x2,5. Cause probable : les batchs récents sont surtout des rips supplémentaires du même concurrent (Primitive Labs) sur le même mécanisme, déjà exposé à l'audience depuis 2 mois.

### Répartition des 13 native ads actives — origine et framework

**13 scripts natives uniques tournent, 12 sur 13 utilisent la même framework narrative** (récit 3 actes : mystère → insider → cascade géopolitique → eau → ancrage Texas 2021 → démo → CTA rareté), reprise du concurrent Primitive Labs.

| Origine | Scripts | Part du spend |
|---|---|---|
| Rip concurrent (Primitive Labs Ad 1→21) | 9 | ~85 % |
| Itération interne (batch 2) | 3 | ~10 % |
| Création interne hors batch | 1 | ~5 % |

Top performers : **László/Voisine** (€1 977 EU · $7 590 interne · 885 achats — pilier n°1, mais un seul POV testé en native sur les 4 écrits en vidéo) · **Chauffeur Bolt** (€1 170 EU · $1 476 · 178 achats) · **Húgom Szerbiából** (€270, meilleure nouvelle entrée du batch récent — preuve par témoignage familial plutôt que par insider).

**Goulot identifié** : sur ~35 scripts long-form rédigés, seuls 16 tournent. Le script noté **9,5/10 "le meilleur pour la Hongrie"** ([[script-lista-kertesz]], mécanisme liste de priorité plutôt que révélation insider) n'a jamais été lancé. 13 briefs vidéo produits, une seule vidéo (framework 7 blocs maison) dépense réellement (€188, mieux classée du format vidéo).

**Frictions actives à corriger** : ~€425 de spend estimé sur des créas HU qui citent encore "HYDRA-X1" (nom réservé aux marchés SK/CZ) au lieu de "HYDRA-X2" (nom HU) ; claim "militaire" toujours en ligne sur 2 créas malgré la règle compliance du 18/07 qui l'interdit ; nommage des ads ("ads 1"→"ads 13") qui empêche d'attribuer 39% du spend à un script précis.

Détail complet (mapping ad par ad, batchs, recommandations) : `perf-audit-2026-08-10.md` et `native-ads-repartition-2026-08-10.md` (vault Obsidian, pas encore copiés dans ce repo).

## Performance Meta Ads (1–20 juillet 2026)

| Groupe | Achats | Spend | CPA | Adsets | Note |
|--------|--------|-------|-----|--------|------|
| ads 1 | 194 | $1 313 | $6.77 | 13 | |
| ads 2 | 185 | $1 355 | $7.32 | 10 | |
| ads 3 | 184 | $1 100 | **$5.98** | 10 | Meilleur CPA |
| ads 4 | 86 | $534 | $6.21 | 11 | |
| ads 5 | 11 | $48 | **$4.35** | 3 | ⭐ Early winner — correspond au script Éva/Infirmière (diffusion 16 juil) |
| ads 6 | 0 | $2 | — | test | |
| **Total** | **660** | **$4 352** | **$6.59** | | |

### Signaux forts (mi-juillet)

- **ads 3** : 7 achats à ROAS 52x sur une itération récente — à scaler
- **ads 5** : 5 achats à ROAS 28x, CPA $4.35 — early winner script Éva, à scaler en priorité

### Angle dominant

100% des top ads tournent sur l'**Angle #1 (Insider géopolitique / crise eau)**. Les angles #2 (contamination) et #3 (gaslighting) n'ont pas encore de native ads en circulation — testés uniquement en statiques.

## Commentaires (208 total — 110 visibles / 98 hidden)

### Frictions majeures identifiées

1. **"1500L" vs "400L"** — incohérence entre scripts et page produit (repérée par commentateurs). Erreur historique, pas corrigée vu les stats. Règle future : 400L max.
2. **Détection AI/GPT** — "Ha már íratsz egy cyberpunk típusú novellát a gptvel"
3. **Pattern fatigue** — "Ezt már olvastam taxissal is" (même histoire recyclée avec taxi)
4. **Langue traduite** — "Nagyon furcsa magyarsággal íródott ez a szöveg"
5. **"Où filtrer si pas d'eau ?"** — objection logique sur les sources alternatives
6. **Friction paiement** — demande d'option virement (COD insuffisant pour certains)

### Signaux positifs

- Intentions d'achat directes dans les commentaires
- Croyance dans le scénario de crise
- Social proof organique (partages, tags de proches)
- Marketing reconnu et admiré par certains commentateurs

## Classement natifs par spend (24/08) — priorité passage vidéo

Ranking complet (spend décroissant, sans chiffres exacts) et détail du pipeline de conversion natif → vidéo (ElevenLabs EN + doublage HU) dans [05-ads.md](05-ads.md). Résumé : les piliers vidéo restent László/Voisine et Chauffeur Bolt ; les scripts natifs Éva/Infirmière, Húgom Szerbiából et Colonel László 62 sont les prochains en tête de file pour le même traitement.

---
Sources : export Meta Ads + analyse commentaires session 2026-07-20, confirmé par Ruben 2026-07-22 ; conversations Claude du 2026-08-24 au 25 (classement spend natifs, pipeline vidéo)
