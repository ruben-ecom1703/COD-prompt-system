# Onela — contexte marque

Une des 4 marques COD (ecom Cash-On-Delivery, marché Hongrie) sous [[1 Terrains/COD Empire/_context|COD Empire]]. Repo Data Hub GitHub : `COD-Agency-Data-brand/COD-onela`.

**Produit :** Capsule de chlorophylle anti-odeurs (haleine + corporel). Complément alimentaire, brand à récurrence. Mass market, grosse pain.
**Site :** onela.shop/products/onela-szagsemlegesito-etrend-kiegeszito
**Concurrent cloné :** Lyveli (lyveli.com, marché FR)

## 2026-07-16
- Marque identifiée lors du setup du système Data Hub GitHub (voir [[1 Terrains/COD Empire/_context|COD Empire]] § Système Data Hub GitHub). Repo à remplir — build pas encore démarré (priorité donnée à Nomad Labs en premier).

## 2026-07-17
- Collecte initiale : export CSV perf juin 2026 (20 ads, $346.40 spend, 20 achats), fetch site live complet (offre, formule, FAQ, témoignages), veille concurrent Lyveli (3 angles identifiés : caséum, digestif, gummies).
- Format gagnant du testing : cartoon (personnages illustrés — grenouille/gecko), réadapté très rapidement depuis Lyveli. Rentable mais pas énormément.

## 2026-07-23
- **Ingestion complète des scripts top ads + analyse** dans le repo GitHub (01-brand, 04-angles-personas, 05-ads, 06-resultats, 09-site-funnel — tous remplis).
- **Scripts des top ads récupérés :**
  - Ads 4 ($120.54, 6 achats) : cartoon dialogue amis, "ton pote pue 24h/24"
  - Ads 2 ($67.70, 6 achats, $11.28/achat) : cartoon personnages personnifiés (bactérie vs chlorophylle) — **meilleur CPR des gros budgets**
  - Ads 1 ($62.75, 2 achats) : variante cartoon
  - Ads 9 + Ads 4 bis ($9.69, 5 achats, $1.79-2.04/achat) : static + texte emoji — **meilleur CPR absolu** (signal fort, budget faible)
- **Problème critique identifié :** tous les scripts contiennent des noms du concurrent (Livelli Plusz, Jelveli formula, Deos) au lieu d'Onela — copie brute non adaptée.
- **5 pistes d'angles non testés identifiées :** caséum (P1), odeur corporelle (P2), social/couple/intimité (P3), confession insider type dentiste (P4), digestif pur développé (P5).
- **Analyse site complète** : page produit solide (2147 avis 4.8/5, expert endorsement, comparatif, FAQ, COD). Incohérence social proof (15 000 dans les ads vs 2 147 sur le site).
- Brand identifiée comme **gros potentiel d'optimisation** : pain mass market + un seul angle testé + scripts rushés avec noms du concurrent → marge énorme sur le CPR.

## 2026-07-24
- **Angle 4 "déodorant interne" rejeté** par Ruben — le produit n'a pas de preuve suffisante pour les odeurs de transpiration/peau. Remplacé par **angle 4 "Fumeur"** (haleine sous la fumée).
- **Recherche scientifique complète** sur chlorophylle + fumeur : Desulfovibrio 17x plus chez fumeurs (Kato/Antinozzi 2022), Fusobacterium 5x (Al Bataineh 2020), salive -24% (Christy 2025), VSCs = 90% halitose (Zanetti 2021). Mécanisme défendable : chlorophylline cuivrique se lie au H2S + méthyl mercaptan dans le GI tract. FDA reconnaît chlorophylline comme déodorant interne (OTC M026, 2020).
- **Data Hongrie** : 28.1% fumeurs adultes = 2.3M personnes, 4e en Europe. Paradoxe social : 57% d'acceptation du tabac MAIS 89% des célibataires refusent de sortir avec un fumeur.
- **3 scripts native ads Angle 4 Fumeur écrits** : F2 gaslighting (confession homme fumeur 34 ans), F1 test à jeun (femme fumeuse 29 ans + test 24h), F4 insider dissident (pharmacien fumeur 42 ans). Sauvés dans `COD-onela/ads/scripts-native-ads.md`.
- Scripts angles 1-3 écrits dans la session précédente. ~~pas sauvés en fichier~~ → **CORRECTION 2026-08-07 : ils SONT bien dans `COD-onela/ads/scripts-native-ads.md`. Les 16 scripts y sont complets et indexés.**
- **Angle futur identifié : MÉNOPAUSE** — la ménopause cause des changements hormonaux qui perturbent la flore intestinale et la production d'odeurs. Angle à développer plus tard avec data scientifique. Cible : femmes 45-60.
- **2 scripts Angle 5 Confession dating écrits** : F2 gaslighting (femme 28 ans, célibataire, "c'est dans ta tête"), F5 cycle échec-espoir (femme 31 ans, en couple, pattern 2 semaines sur 3 relations). 
- **2 scripts Angle 7 Haleine du matin écrits** : F1 test à jeun (homme 36 ans, marié, "test de la brosse du soir"), F4 insider dissident (dentiste 48 ans qui se lève 15 min avant sa femme, concept "2 couches"). Tous sauvés dans `COD-onela/ads/scripts-native-ads.md`.

## 2026-07-25
- **Premier stock en cours de réception : 2 000 pièces** attendues dans la semaine.
- **Délai de réapprovisionnement complet : 30 jours** (2 sem. production + 2 sem. envoi).
- **Calcul de capacité stock** : bundle best-seller = 2+1 (3 unités/commande) → 666 commandes possibles → max 16 cmd/jour pour tenir 40 jours (reorder à J+10). Si reorder à J+5, marge monte à 19 cmd/jour.
- **Stratégie stock** : lancer les ads, observer le rythme réel sur 5-10 jours, puis reorder immédiatement pour tenir sans rupture.

## 2026-08-07
- **Audit des 16 scripts native ads confirmé** : tous présents et complets dans `COD-onela/ads/scripts-native-ads.md` (96 Ko, index en tête). Structure = 7 angles × 5 frameworks (F1 test à jeun, F2 gaslighting, F3 autorité pédago, F4 insider dissident, F5 cycle échec-espoir). Répartition : Caséum 3, Reflux 3, Langue blanche 3, Fumeur 3, Dating 2, Haleine du matin 2. Angles 6 (insider pur) et 8 (odeurs alimentaires) dans la matrice mais non scriptés. Fil rouge commun aux 16 : les VSC viennent du tractus GI, la bouche n'est que le lieu où on les constate.
- **Headline + sub-headline du link preview définis** (modèle décortiqué : Lynae / lynae.co, "C'est pas dans votre tête." + sub descriptive plate). Recette : headline ≤5 mots, négation + déplacement du problème, sans nom de produit / chiffre / exclamation ; sub-headline 100 % descriptive ton notice, écrite pour que la troncature Facebook tombe sur un mot ouvert.
  - **Pick universel compatible avec les 16** : `Ce n'est pas votre bouche.` — jumeau structurel du headline Lynae et thèse littérale des 16 scripts.
  - **Sub** : « Complément naturel à base de chlorophylle pour neutraliser les composés soufrés dans le système digestif, là où l'odeur se forme. Premiers résultats… »
  - HU : `Nem a szája a probléma.` + sub HU — **à faire relire par un natif avant launch** (plusieurs tournures de négation possibles).
  - Règle de test : même headline sur les 16 au premier round, sinon deux variables en même temps.
  - Interdit : réutiliser « C'est pas dans votre tête » tel quel (headline actif de Lynae, même plateforme).
  - Détail sauvé dans `COD-onela/ads/headlines-native-ads.md`.
- **Stratégie de test des headlines arrêtée (2 rounds)** : Meta accepte 5 titres/pub via "plusieurs versions de texte", mais **pas au round 1** — 16 scripts × 4 headlines = 64 combinaisons pour ~20 achats de data, reporting par combinaison inexploitable. Round 1 = 1 seule headline sur les 16 (isoler le script). Round 2 = les 2-3 scripts gagnants dupliqués en pubs séparées, 1 headline par pub. Multi-titres réservé au scaling.
- **⚠ Règle policy Meta apprise — Attributs personnels** : ne jamais écrire `Votre mauvaise haleine…`. Le possessif = affirmation directe sur l'état de santé du lecteur → motif de refus classique sur les compléments, et à répétition ça tape le compte pub. Reformuler en général : `La mauvaise haleine n'est pas normale.` Les headlines en négation pure (`Ce n'est pas votre bouche.`) passent car elles n'affirment rien sur le lecteur.
- **Limite d'usage repérée** : `Vous nettoyez au mauvais endroit.` ne colle pas aux scripts #10-12 (Fumeur) ni #13-14 (Dating) — le lecteur n'y "nettoie" pas. Réservée aux 12 autres.
- **Sub-headline v2 retenue** : « Complément alimentaire naturel qui neutralise les composés soufrés dans le système digestif. Là d'où l'odeur vient vraiment. Résultats… » — calibrée sur la longueur Lynae pour que la troncature FB tombe après le payoff.
- **PACK DE DÉPLOIEMENT HU figé** (prêt à copier-coller, dans `headlines-native-ads.md`) : sub unique `Természetes étrend-kiegészítő, amely az emésztőrendszerben semlegesíti a kénvegyületeket. Onnan, ahonnan a szag valójában ered. Eredmények…` + 3 headlines → **H1** `Nem a szájában kezdődik.` / **H2** `Rossz helyet tisztít.` / **H3** `A szájszag nem normális.` CTA `Vásárlás`.
- **Affectation headline × script décidée** : H1 sur #2,4,6,8,11,12,16 (scripts d'autorité/insider, 7) · H2 sur #1,5,7,9,15 (scripts avec geste de nettoyage inutile, 5) · H3 sur #3,10,13,14 (scripts F2 gaslighting / F5 cycle, 4). Règle : **jamais H2 sur Fumeur ni Dating**.
- **Arbitrages HU en attente du natif** : H2 `Rossz helyen keresi.` (plus idiomatique, perd le verbe "nettoyer") vs `tisztít` · H3 `szájszag` (courant, mass market) vs `rossz lehelet` (propre).
- **Matrice de compatibilité headline × script établie** (fallbacks par script, pas seulement le pick) : **H1 passe sur les 16, sans contre-indication** — c'est la valeur par défaut, y compris pour les angles futurs (Ménopause, Odeurs alimentaires). Les 5 scripts où les 3 headlines passent : #4, #6, #7, #15, #16. **H2 interdite sur #10-12 (Fumeur) et #13-14 (Dating)** — le lecteur n'y nettoie rien, la headline promet un contenu absent → clic payé, vente perdue. **H3 faible (mais pas fausse) sur #1, #2, #5, #8, #9** — pas de moment "on m'a dit que c'était normal" dans ces scripts.
- **Workflow de saisie "3 copier-coller"** défini pour ne pas retaper 16 fois : H2 → 1/5/7/8/9/15 · H3 → 3/10/13/14 · H1 → 2/4/6/11/12/16 · sub identique sur les 16.
- **⚠ Blocage launch Rapid-Ads (campagne `onela – hu – 07/08/26`, Adset 1, 6 vidéos buccales HU)** : erreur Meta `Campaign Has Invalid Ad Account: Your campaign must have the same account id as the adgroup you're creating.` → la campagne existe dans un compte pub A, mais Rapid-Ads envoie la création de l'adset avec l'account id d'un compte pub B. Rien à voir avec les créas (les 6 sont "Ready"), ni avec le pixel, ni avec la policy. Cause la plus fréquente : compte pub sélectionné dans Rapid-Ads ≠ compte où la campagne a été créée (ou session cachée sur l'ancien compte après un switch de BM). Fix : Settings Rapid-Ads → re-sélectionner le compte pub propriétaire de la campagne, hard refresh, re-choisir campagne + adset, relancer. Si ça persiste : recréer la campagne depuis le compte actuellement connecté.

## 2026-08-10

### Autonomie de stock — 2 000 unités
- **Panier moyen : 2,8 unités/commande** → **714 commandes** disponibles sur le stock (reste 0,8 unité).
- Rythme d'acquisition max par horizon :

| Horizon | Cmd/jour | Cmd/semaine | Unités/jour |
|---|---|---|---|
| 30 j | 23,8 | 167 | 67 |
| 35 j | 20,4 | 143 | 57 |
| 40 j | 17,9 | 125 | 50 |
| 45 j | 15,9 | 111 | 44 |

- **Fenêtre cible 35-45 jours → rester entre 16 et 20 commandes/jour.**
- Lecture inverse : 10 cmd/j = 71 j · 15 cmd/j = 48 j · 20 cmd/j = 36 j · 25 cmd/j = 29 j · 30 cmd/j = 24 j · 40 cmd/j = 18 j.
- ⚠ Le chiffre de décision n'est pas la rupture mais le **seuil de recommande** = lead time fournisseur × conso quotidienne. Exemple : à 18 cmd/j avec 25 j de délai fournisseur, repasser commande à **1 260 unités restantes** (≈ J+15). **Lead time réel à confirmer.**
- Comparatif : à stock égal, Onela sort **714 commandes** contre 1 000 pour Keskia (panier 2,0 u/cmd) → Onela part en rupture en premier si les deux tournent au même nombre de commandes/jour.

## 2026-08-21

### Stats campagne Hongrie (depuis réception stock)
- **163 commandes** écoulées, **279 articles**, **1,71 art./cmd**
- **CA : 6 579 €**, AOV : 40,36 €, **98 % COD**
- **Dépense pub : 1 005 €** → **ROAS 6.55x** (profit estimé ~2 891 €)
- **ROAS break-even : 1.69x** → marge confortable
- **Stock restant estimé : ~1 721 unités** (2 000 – 279)
- **3 000 unités supplémentaires en transit** (arrivée ~2-3 semaines)
- Possibilité de repasser commande dès maintenant (délai production ~2 semaines)
- Discussion scaling en cours avec Geoffrey
