# 10-operations — Nomad Labs

> 📅 Dernière mise à jour : 2026-08-26 · Gérant : Ruben

> ⚠️ Compte pub / logistique 3PL / stack encore en attente de la capture Business Manager (voir [07-relance.md](07-relance.md), item bloquant #2). Cette page ne couvre pour l'instant que le stock, seul point communiqué à date.

## Ads Manager — incident restriction Business Manager (2026-08-26)

Meta a restreint 2 Business Managers de l'agence ("HP 664", "Abu 2") le 26/08 pour suspicion d'automatisation/détection anti-bot. **Le compte pub dédié Nomad Labs ("CLK_0428-KN-3 - Nomadslabs") a été vérifié sain et non affecté.** À surveiller au prochain sync.

## Workflow créa — retours monteur (2026-08-26)

La reviewer de contenu "Sylvio" produit des révisions d'ads/B-roll jugées positives (bon rendu réalisme, cohérence avec la marque). Demande faite de passer la livraison des B-roll par Google Drive plutôt que par fichier zip (zip non accessible côté Ruben).

## Stock (mise à jour 2026-08-21)

- **Réception fournisseur** : ~10 000 unités tous les 5 jours en moyenne (rythme de réappro confirmé, cohérent avec le "+10 000 unités/semaine" annoncé le 17/07)
- **Stock estimé en main** : ~30 000 unités
- **Pipeline de réappro continu** — pas de risque de rupture identifié à court terme au rythme actuel de scaling

## Stock (au 2026-07-17) — historique



- **Vélocité de vente observée** : 645 commandes / 14 jours = **~46 commandes/jour**, 1 964 items vendus / 14 jours = **~140 items/jour** (~3,05 items/commande en moyenne)
- **Stock disponible aujourd'hui (17/07)** : ~2 000 unités
- **Réassort en douane** : +4 000 unités, dédouanement attendu "d'ici quelques jours" (~22/07 en hypothèse basse)
- **Gros arrivage suivant** : +10 000 unités attendu vers le **5 août 2026** (donné en fourchette par Ruben, pas une date ferme)
- **Rythme annoncé après le 5 août** : **+10 000 unités/semaine** en continu, le temps de laisser les monteurs vidéo produire davantage de créatives avant d'accélérer le scaling

## Lecture pacing stock vs scaling (calcul du 17/07)

| Étape | Stock disponible | Conso cumulée (@140/j) | Solde |
|---|---|---|---|
| Aujourd'hui (17/07) | 2 000 | — | 2 000 |
| Sans réassort | — | rupture théorique ~31/07 (14,3j de marge) | — |
| Douane arrivée (~22/07, +5j) | +4 000 | 5j × 140 = 700 | 1 300 + 4 000 = 5 300 |
| Jusqu'au 5 août (14j restants) | — | 14j × 140 = 1 960 | **5 300 − 1 960 = 3 340 unités d'avance** |

→ **Pas de risque de rupture avant le 5 août au rythme actuel** — marge d'environ 3 340 unités (~24 jours de plus) même si le gros arrivage prend du retard. De la marge existe pour accélérer le scaling avant cette date, mais pas au point de viser le plafond théorique (~316 items/jour, 2,25x le rythme actuel) sans garde-fou.

## Modération commentaires — audit CommentGuard (2026-07-29)

Audit de l'outil CommentGuard.io (page Felkészült Magyar Családok, langues HU/SK/CZ/parfois FR) — settings actuels : profanity/negativity/custom topics/URLs/emails-phones/images tous ON, appliqué posts + ads, **impersonators OFF**.

**Problème trouvé** : un des 4 custom topics existants est un doublon exact d'un autre ("produit inutile / ne marche pas" en double).

**4 nouveaux topics recommandés** (types de commentaires qui passent actuellement à travers) :
1. Doute sur l'authenticité de la démo/vidéo ("il fait semblant de boire")
2. Accusation de contenu généré par IA
3. Meta-commentaire "c'est juste de la pub"
4. Hors-sujet religieux/politique

**Autres recommandations** : activer **Hide impersonators** (actuellement OFF) ; configurer les auto-réponses (onglet Automation, non utilisé à date) pour les questions d'achat (→ lien site) et les questions produit (→ data Hydra X2) ; renforcer le texte des règles de modération personnalisées ; tester le tout dans le Playground avant activation.

---
Source : conversation Claude du 2026-07-17 (chiffres stock donnés directement par Ruben, pas d'export système) — aucune donnée de coût/marge incluse, uniquement des unités et des dates. Audit CommentGuard : session vault du 2026-07-29. Mise à jour stock 21/08 : `_context.md` (vault), section "Scaling massif & stats live" — uniquement les unités reprises, aucune donnée de spend/CPA/marge. Incident BM et note workflow monteur : conversation Claude du 2026-08-26.
