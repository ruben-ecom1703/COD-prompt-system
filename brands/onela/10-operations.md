# 10-operations — Onela

> 📅 Dernière mise à jour : 2026-08-31 · Gérant : Ruben

**Contenu attendu** : Compte pub (nom + ID), logistique 3PL, stock, stack — SANS unit economics ni identifiants

## Stock (2026-08-21)

**163 commandes écoulées depuis réception du stock** (279 articles, 1,71 article/commande). Rythme observé depuis : ~14 commandes/jour.

- Stock restant estimé : **~1 721 unités** (2 000 − 279)
- **3 000 unités supplémentaires en transit**, arrivée estimée ~2-3 semaines
- Possibilité de repasser commande dès maintenant, délai de production ~2 semaines
- Discussion scaling en cours avec Geoffrey (issue non tranchée à date)
- **Règle de pilotage actée** : repasser commande fournisseur maintenant (avant même de scaler) ; des seuils ROAS de stabilisation/coupure ont aussi été fixés par Ruben (valeurs non reprises ici — filtre coûts, voir CHANGELOG).

## Stock (2026-08-10)

**Stock disponible : 2 000 unités.** Panier moyen : **2,8 unités/commande** → **714 commandes** possibles sur ce stock (reste 0,8 unité).

Rythme d'acquisition max par horizon avant rupture :

| Horizon | Cmd/jour max | Cmd/semaine | Unités/jour |
|---|---|---|---|
| 30 j | 23,8 | 167 | 67 |
| 35 j | 20,4 | 143 | 57 |
| 40 j | 17,9 | 125 | 50 |
| 45 j | 15,9 | 111 | 44 |

**Fenêtre cible retenue : 35-45 jours → rester entre 16 et 20 commandes/jour.**

Lecture inverse (jours de tenue selon le rythme de commandes) : 10 cmd/j = 71 j · 15 cmd/j = 48 j · 20 cmd/j = 36 j · 25 cmd/j = 29 j · 30 cmd/j = 24 j · 40 cmd/j = 18 j.

⚠️ Le seuil de décision n'est pas la rupture mais le **seuil de recommande** = lead time fournisseur × conso quotidienne. Lead time réel fournisseur encore à confirmer.

Repère : à stock égal (2 000 unités), Onela tient 714 commandes contre 1 000 pour Keskia (panier 2,0 unités/commande) — Onela part en rupture en premier si les deux marques tournent au même rythme de commandes/jour.

## Blocage lancement Rapid-Ads (2026-08-07)

Campagne `onela – hu – 07/08/26`, Adset 1 (6 vidéos buccales HU) — erreur Meta au lancement : `Campaign Has Invalid Ad Account: Your campaign must have the same account id as the adgroup you're creating.`

- Cause : le compte pub sélectionné dans Rapid-Ads au moment de la création de l'adset ne correspond pas au compte pub propriétaire de la campagne (mismatch fréquent après un switch de Business Manager, ou session restée sur l'ancien compte).
- Rien à voir avec les créas (les 6 étaient "Ready"), le pixel, ou la policy.
- **Fix** : dans les settings Rapid-Ads, re-sélectionner le compte pub propriétaire de la campagne → hard refresh → re-choisir campagne + adset → relancer. Si persistant : recréer la campagne depuis le compte actuellement connecté.

---
Sources : conversation Ruben 2026-08-10 (calcul stock), session 2026-08-07 (blocage Rapid-Ads)
