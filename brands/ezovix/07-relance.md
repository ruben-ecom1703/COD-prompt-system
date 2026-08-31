# 07 — Plan de relance (actions priorisées)

> 📅 Dernière mise à jour : 2026-08-30 · Statut : 🔁 **campagnes relancées le 29/08** sur le BM Abu 3 (remplace Lydia Martinez restreinte le 26/08) · plafond de dépense non reconfirmé débloqué · Gérant : Hugo

**Ce que contient ce fichier :**
- Le plan d'action exact à la relance des ads, dans l'ordre
- Ce qu'on scale, ce qu'on garde, ce qu'on reteste
- Les idées d'itération créa prêtes à produire

**Ezovix = la priorité absolue du portefeuille à la relance** (ROAS 10,81, 1 ad sur 2 vend — cf. [06-resultats.md](06-resultats.md#comparatif-des-4-brands)).

---

## Étape 0 — Débloquer (bloquant)

- [x] **Lever le plafond de dépense du compte `CLN_0645-KN-6`.** Campagnes relancées le 29/08 sur le nouveau BM opérationnel Abu 3. ⚠️ **Non reconfirmé** : au 28/08 le compte affichait encore $0,00 dépensé sur 30 jours (toutes campagnes Off) — à vérifier après la relance que le plafond n'est plus bloquant.
- [ ] Vérifier le stock (toutes les ads du portefeuille sont en pause pour attente de stock).

## Étape 1 — L'argent le plus facile (zéro création)

- [ ] **Mettre du budget sur « GERD vs LPR »** (`120246113936040014`). Même copy que le winner, **ROAS 15,24 et 3,70 $/vente — le meilleur des trois** — et elle n'a reçu que 33 $, soit 2,5× moins que les autres. Rien à créer, juste ouvrir le robinet.
- [ ] Maintenir le budget du **blueprint « A Torok Amely Nem Ürül Ki »** (`120246113936180014`) — le winner volume (18 ventes, +1 010 $ net).
- [ ] **Garder « A Nyákcsapda »** (ROAS 6,18, +430 $, panier moyen le plus haut : 64 $). Moins efficiente → on l'alimente APRÈS les deux autres, mais **on ne la coupe pas** (le juge = le ROAS, pas le CPA).

## Étape 2 — Donner leur chance aux non-testés (quasi zéro création)

- [ ] **Basculer les récits de l'Adset 2 sur la page Labor** : la chanteuse (#4), les 20 ans d'antiacides (#12), les 3 faux infarctus (#11), le prisonnier de l'IPP (#14), le reflux nocturne (#9), le globus (#10). Ils tournaient sur la page qui convertit 6× moins avec < 3 $ chacun — **ce ne sont pas des losers, ils n'ont jamais été testés** (cf. [06-resultats.md](06-resultats.md#les-pages)).
- [ ] Les visuels de ces 6 angles sont déjà produits (47 créas, 2 variantes par idée) → [visuels/](visuels/README.md).

## Étape 3 — Itérer sur le style gagnant (création légère)

- [ ] **Décliner le style « schéma médical »** sur la copy winner (jamais de produit, jamais de prix, jamais de visage) :
  - la pepsine qui se colle au tissu de la gorge
  - le liquide qui enrobe vs la gélule qui tombe dans l'estomac
  - une coupe avant/après de l'œsophage
- [ ] Explorer les 2 territoires d'angle jamais produits : anxiété alimentaire (repas) et advertorial médecin (cf. [04-angles-personas.md](04-angles-personas.md#plan-dangles-dorigine)).

## Rappels avant de produire

- Relire [03-compliance.md](03-compliance.md) (hedges, cœur, IPP) avant toute copy.
- Offre exacte uniquement : 12 900 / 21 900 (2+1) / 28 900 (3+2) Ft — cf. [01-brand.md](01-brand.md#offre).
- Toute nouvelle ad = fiche complète + diagnostic (règles dans [05-ads.md](05-ads.md#règles-de-production)).
- Nouveau récit « je » → page qui matche le narrateur, et priorité Labor tant que l'écart 6× n'est pas réfuté.

## Avant de scaler — anti-rejet Meta (MAJ 2026-07-15)

Retour d'expérience d'un call groupe (14/07/2026) sur un scénario vécu par une autre brand santé : les ads passent la review au testing petit budget, puis Meta les re-contrôle dès que le spend monte et les rejette. Ce portefeuille (claims santé, récits façon médecin) est exposé au même profil de risque.

Mécanismes de protection à mettre en place, par ordre :

1. **Post ID organique** : publier la créa en post organique sur la page persona (ou la lancer en objectif interactions), puis créer l'ad de conversion en reprenant ce post ID existant. Review plus légère, pas de re-review de créa à chaque duplication au scale, preuve sociale cumulée sur un seul post. → à la relance : publier les winners en organique quelques jours avant de les lancer en ads.
2. **Sous-domaine tampon clean** : créer un sous-domaine 100 % clean (zéro claim santé, zéro mot flaggé) qui redirige vers l'advertorial — le robot Meta classe le domaine à partir de ce qu'il crawle. Rester sur une page tampon réellement clean et cohérente : un cloaking pur (page robot ≠ page utilisateur) aggrave la sanction si détecté.
3. **Agency ad account** : compte agence whitelisted, tolérance et limites plus hautes (piste non détaillée).

Rappel structurel : la data diffère entre comptes pub — ne jamais conclure qu'une ad est morte sur un seul compte ; garder le pixel, tester l'offre dans une nouvelle campagne (même compte), sur au moins une semaine avant de trancher.

---

*Navigation : [← 06 — Résultats](06-resultats.md) · [README (sommaire)](README.md)*
