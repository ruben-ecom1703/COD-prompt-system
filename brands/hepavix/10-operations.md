# 10 — Opérations & fonctionnement

> 📅 Dernière mise à jour : 2026-08-30 · Gérant : Hugo
> ⚠️ **Documentation descriptive uniquement.** Ce fichier explique le setup et où chaque chose est gérée. Il ne contient **aucun identifiant, aucun secret, aucune donnée financière** (COGS et marges volontairement exclus).

**Sommaire** : [Qui gère quoi](#qui-gère-quoi) · [Setup publicitaire](#setup-publicitaire) · [Logistique COD](#logistique-cod) · [Stack](#stack) · [Ce qui nest pas dans ce repo](#ce-qui-nest-pas-dans-ce-repo)

---

## Qui gère quoi

| | |
|---|---|
| **Gérant de la brand** (ads, site, data, ce repo) | **Hugo** |
| Contexte | Hepavix = brand du projet COD (Ruben × Hugo × Danila), 4e site testé, semaine du 22/06 → 28/06 |
| Relation partenaire logistique | Danila (pilote), avec Ruben et Hugo |
| Copies des ads | Miroir complet dans [ads/](ads/README.md) — briefs d'origine dans Notion |

## Setup publicitaire

- **Compte publicitaire** : `CLN_0428-KN-5`
- **Campagne** : « **26/06/26 Hepavix** » — objectif Outcome Sales, budget quotidien 150 $, **17 ads dans un seul ad set** (`Adset 1 - Static/Native`)
- **Statut au 13/07/2026** : campagne éteinte (PAUSED) — une mise en pause, pas un blocage de compte. (À la différence d'Ezovix, qui a atteint un plafond de dépense.)
- **🔴 Statut au 07/08/2026** : **relancée sur ce même compte de base** (`CLN_0428-KN-5`), campagne « 26/06/26 Hepavix », **150 $/j**, avec les **16 ads d'origine**. Le projet de migration vers un nouveau compte (`ReStart 07/08/26`, ci-dessous) a été **abandonné** → détail [ci-dessous](#-maj-2026-08-07-suite--import-abandonné-relance-sur-le-compte-de-base).
- **🚩 Statut au 08/08/2026** : le pixel de ce compte est **flaggé par Meta** (« Some website data blocked ») → détail [ci-dessous](#-maj-2026-08-08--pixel-hepavix-flaggé--some-website-data-blocked-).
- **3 pages Facebook** utilisées (IDs vérifiés dans l'export de créatives) → [01-brand.md](01-brand.md#pages-facebook)
- **Méthode de suivi de la perf** : exporter (1) l'export de créatives `.xlsx` (contient `Link Object ID` = la page FB) et (2) l'export de performances `.csv`, puis croiser sur le nom d'ad. Les deux exports bruts sont archivés dans [data/exports-meta/](data/exports-meta/) — n'importe qui peut refaire le calcul.

## Logistique COD

Partenaire 3PL officiel du portefeuille (contact : Teodor ; onboarding piloté par Danila) :

- **Hub : Slovaquie** → livraison rapide sur SK / PL / CZ / **HU**. Les compléments alimentaires sont stockés en Slovaquie.
- **Flux client (utánvét)** : commande en ligne sans carte → expédition → **le client paie en liquide au livreur à la réception** → le cash est reversé. Détail du parcours : [09-site-funnel.md](09-site-funnel.md#funnel-cod).
- Le réseau du partenaire couvre la CEE (entrepôts BG / RO / HR / IT / ES) → utile pour l'expansion après validation du marché hongrois.
- ⚠️ Les ads du portefeuille sont en pause en attente de stock → **vérifier le stock avant toute relance**.

### MAJ 2026-07-15 — écart packaging site vs colis réel

Le colis réellement expédié n'est **pas** la boîte « premium » visible sur le site — c'est le même packaging que Nuvalis avec un nouveau label (choix de rapidité). En COD, le client ouvre le colis à la livraison : un écart trop visible entre le site et le colis reçu est un risque de refus. À date, décision = ne pas montrer le packaging de base sur le site et retoucher le mock-up si besoin.

### 🟢 MAJ 2026-08-06 — stock confirmé 10 000 unités, couverture large

Approximation construite depuis le tableau transverse stock/couverture des 4 brands du portefeuille (méthode : couverture en unités, jamais en commandes) :

| Stock | Conso estimée | Couverture | Rupture estimée |
|---|---|---|---|
| **10 000 unités** (confirmé 06/08) | ~65 u/j à 150 $/j (winner ≈ 7 $/achat) | **~154 j** | **~janvier 2027** |

| Budget | Conso | Couverture | Rupture |
|---|---|---|---|
| 150 $/j | ~65 u/j | ~154 j | ~janvier 2027 |
| 300 $/j | ~130 u/j | ~77 j | ~fin octobre |
| 600 $/j (scale Q4) | ~260 u/j | ~38 j | ~mi-septembre ⚠️ |

**Verdict : c'est la brand qui peut encaisser le scale Q4** sans risque de rupture à budget modéré — mais si elle confirme son statut de meilleure brand du portefeuille et scale fort (300-600 $/j), le réassort doit être commandé avant mi-septembre malgré les 10k en stock (lead time ~45 j Chine → Slovaquie, deadline dure Q4 = commande avant mi-septembre).

### 🟢 MAJ 2026-08-24 — Chiffres réels confirmés par Hugo : cadence 2× l'estimation, lead time réel bien plus court, réassort ~20 000 u recommandé

Les hypothèses du 06/08 sont remplacées par des chiffres réels donnés par Hugo :

| Cadence réelle | Couverture (10 000 u au 24/08) | Rupture estimée |
|---|---|---|
| 100 articles/j | ~100 j | ~début décembre |
| 125 articles/j | ~80 j | ~mi-novembre |
| 150 articles/j | ~67 j | ~fin octobre |

- **Cadence réelle = 100-150 articles/j** (40-50 commandes/j, parfois 60) — **~2× l'estimation initiale de 65 u/j** du 06/08.
- **Lead time réel = 2-3 semaines** (pas les ~45 j génériques du portefeuille) — vraisemblablement du stock pré-produit chez le fournisseur. Point de commande recalculé : **~3 100 unités restantes** (3 sem × 150 u/j, marge incluse).
- **Scénario scale 5 000 €/day** (objectif affiché pour la brand de tête) : ~230-270 articles/jour → les 10 000 unités ne couvrent plus que **~40 jours**, point de commande remonté à **~5 300 unités**.
- **Recommandation actée : commander ~20 000 unités maintenant.** Besoin d'ici fin décembre estimé entre ~16 000 u (cadence actuelle) et ~25-30 000 u (si le scale 5k/day démarre en sept-oct). Contrainte Q4 : le gros stock doit être à l'entrepôt fin octobre, pas en transit pendant le rush transporteurs de nov-déc. Version cash-light évoquée : négocier le stockage gratuit chez le fournisseur (produire 20-30k, payer à l'expédition, tirer par tranches de ~10k).
- **Minimum vital sans confirmation du scale : 10 000 u** — mais ce plancher remet un point de commande en plein rush Q4 (novembre), déconseillé si l'objectif 5k/day tient.
- Détail du calcul (stock transverse 4 brands) → data master vault, section stock & couverture.

### MAJ 2026-08-06 — rattachement au BM opérationnel partagé du portefeuille

Le compte pub Hepavix est désormais rattaché au BM opérationnel partagé du portefeuille (le même qui héberge les 8 ad accounts des brands Hugo/Ruben) — partage de page finalisé le 06/08. ⚠️ **Ambiguïté non résolue** : le compte pub exact (`CLN_0428-KN-5`) est aussi cité comme celui de Nuvalis dans son propre repo — à confirmer lequel des deux brands le détient réellement (ou s'il a été partagé/réassigné entre les deux à un moment).

### 🔵 MAJ 2026-08-07 — Fichier d'import RESTART livré (migration vers nouvel ad account)

Migration de la campagne testing vers un nouveau départ, format `More → Import ads in bulk` :

- **Base** : export `export_20260806_1712.xlsx` (campagne « 26/06/26 Hepavix », 17 ads) → **16 ads** reprises (1 coquille vide supprimée, body vide + lien google.com + page inconnue).
- **Nouvelle structure** : campagne `CBO - HEPAVIX HU - ReStart 07/08/26` — **3 ad sets, un par page** (`Dr Toth Petra` ×6 · `Page Hepavix` ×6 · `Varga Nora` ×4). ⚠️ Une v1 à ad set unique a été **rejetée à l'import** par Meta (« Link Object ID — Data doesn't match ») : un ad set créé ne peut porter qu'une seule page.
- **Paramètres** : IDs vidés (campaign/adset/ad/story), Image Hash + Video ID vidés (visuels à réattacher aux brouillons), budget **50 $/j warm-up** (CBO, contre 150 $/j en source), tout **PAUSED**, UTM posés (template Aurivo du 24/07), **pixel conservé** `1369068885114854` (non bloqué — à la différence du cas Aurivo).
- **Corrections copy appliquées** : silymarine **80 → 90 %** sur les 3 ads qui citaient encore l'ancien taux (les mentions « 80 % » restantes ailleurs = claims biologiques LDL/choline d'autres marques, non touchées) · 10 mots hongrois cassés réparés sur l'ad de l'hôtesse Airbnb (`üvegcse`, `Edények`, `befőttesüveg`, `esküvőjéről`, `fotel`, `Harmincegy`, `Én is sírtam`, `vizeskancsó`, `csíkokról`).
- **Laissé verbatim (flags connus, non corrigés à cet import)** : dosage « 3 kapszula » sur 4 ads, titres orphelins « Katalin » sur 2 ads, disclaimer absent des 16.
- **Reste à faire à l'import** : ajouter le visuel de chaque ad dans les brouillons, partager les 3 pages au BM de destination si pas déjà fait, relecture native recommandée avant scale sur l'ad de l'hôtesse.

### 🔴 MAJ 2026-08-07 (suite) — Import abandonné, relance sur le compte de base

L'import bulk ci-dessus a finalement été **abandonné**. Hugo a préféré relancer la campagne **« 26/06/26 Hepavix » directement sur le compte de base**, à **150 $/j**, avec les **16 ads d'origine** (verbatim : *« ça clc de faire ça, laisse tomber je vais tout relancer à la main »*). Raison : l'historique du compte (41 ventes, pixel qui a appris, visuels déjà en place) vaut mieux qu'un compte neuf, et évite un import bulk complet.

**Conséquence : la campagne repart avec ses défauts d'origine, pas la version corrigée.** Checklist de relance :

- **Ads 10** (« Katalin LDL », page Dr. Tóth Petra) : à couper — seul vrai échec financé du testing (13,09 $, 0 vente), titre orphelin, visuel jugé à risque « shock content » Meta → [ads/cardiologie-ce-quon-ne-dit-pas.md](ads/cardiologie-ce-quon-ne-dit-pas.md).
- **Ads 12** (l'hôtesse Airbnb) : à couper — rentable, mais la **copy réellement diffusée** contient toujours les mots hongrois cassés (`üvegtutty`, `Harmincégy`…). La version corrigée (10 mots réparés le 06/08) existe et sera relancée séparément plus tard → [ads/statines-airbnb.md](ads/statines-airbnb.md).
- **Ads 1, 2, 3** (encore à 80 % de silymarine) : **ne pas les éditer maintenant** — une édition renvoie l'ad en review et casse le momentum du compte qui vient de repartir. Toute **nouvelle** itération part directement à 90 %.
- **🔴 UTM manquants** : les 17 ads live ont les URL Tags **vides** — le même trou qui a rendu les ventes Aurivo non attribuables. À poser pendant une pause, jamais en pleine diffusion.
- **Visuels** : 12 fichiers renommés par ad préparés (source : dossier de production Hepavix + fichiers retrouvés, tous vérifiés à l'œil). **3 ads sans visuel documenté nulle part** : Ads 3 (alcool), Ads 4 (infirmière), Ads 8 (pour Ads 8 — variante du winner, même angle/titre — la reco est de remettre le même dessin « kötényhas » que le winner).

### 🚩 MAJ 2026-08-08 — Pixel Hepavix flaggé « Some website data blocked »

**Constat (Events Manager, BM opérationnel partagé)** : le dataset **Pixel Hepavix `1369068885114854`** est en erreur active « Some website data blocked ». Domaine concerné : **hepavix.com**. Motif Meta : « associated with medical conditions, specific health statuses… » → catégorie assignée **« Health & wellness conditions »**. C'est le **même mécanisme** que celui déjà documenté sur try-aurivo.shop (cf. le repo Aurivo, MAJ 24/07) : classification automatique du **domaine** par le crawler Meta à partir du contenu du site (foie, ALT/AST, « gyógyszerészeti minőségű májvédelem »…), sans lien avec l'ad account ni avec une erreur de manipulation.

- **Review de catégorisation déjà demandée le 07/08 à 12:19** (statut « Pending review », décision attendue par email). ⚠️ Une nouvelle demande n'est possible qu'à **+30 jours** (fenêtre ~06/09) — ne pas re-soumettre en boucle.
- **Timing notable** : le flag a été détecté le 07/08, soit le jour même de la relance de la campagne sur le compte de base. Pendant le testing de fin juin, le pixel trackait normalement (les 41 ventes du testing sont attribuées).
- **Conséquence probable** : les events mid/lower funnel (dont Purchase) sont partiellement ou totalement bloqués pour les visiteurs situés en UE — et la Hongrie est en UE. L'algorithme Meta optimise donc à l'aveugle et l'Ads Manager sous-compte les ventes réelles. Retour d'expérience Aurivo : un nouveau pixel sur le même domaine se fait bloquer dès le jour 1, et **la CAPI ne contourne pas un blocage domain-level**.
- **Plan d'action (aligné sur le playbook Aurivo)** :
  1. Poser les UTM sur les 17 ads live (trou critique documenté ci-dessus).
  2. Vérifier chaque jour si des Purchase remontent encore côté Meta.
  3. Nettoyer le vocabulaire le plus médical de hepavix.com avant le passage du reviewer.
  4. Si la review est refusée → Plan B domaine : nouveau domaine primaire + redirection 301, sur le modèle déjà utilisé pour Aurivo.
  5. Mesure tierce indépendante du pixel (ex. ClickFlare) mutualisable avec les autres brands du portefeuille en cas de blocage confirmé.

**Repères marché (recherche du 08/08, sources externes citées en conversation — à traiter comme des pistes, pas des garanties)** : l'enforcement Meta sur le vertical santé est incohérent et progressif — beaucoup de sites tournent encore parce qu'ils n'ont pas été crawlés, ou tournent en restriction partielle silencieuse. Piste la plus citée par les media buyers (communautés Shopify, CustomerLabs, Zappush) : des **custom events aux noms neutres** envoyés en CAPI avec un payload nettoyé (aucun nom de produit santé, aucune URL sensible) — mais cette piste est **non garantie** : Meta peut exiger une certification que la donnée n'est pas liée à la santé, et peut aussi filtrer les events server-side d'un domaine déjà classé restreint. Ce qui est documenté comme **ne marchant pas** : renommer seulement les events standards, la CAPI seule, la migration en sous-domaine (la classification porte sur le domaine racine), et la demande de review pour un site réellement médical dans son contenu. Citation retenue : *« The category does not need to change. The data architecture does. »*

### 🔧 MAJ 2026-08-17 — Test pixel "Hepavix V2" + review Meta relancée + identifiants précisés

- **Nouveau pixel "Hepavix V2" créé et connecté à EasySell**, en sachant qu'un nouveau pixel ne débloque PAS le flag de catégorisation (mécanisme domain-level, cf. MAJ 08/08 ci-dessus — contrairement à Nuvalis, dont le Shopify indépendant permet de voir les commandes normalement même flaggé). Test réversible et sans coût. Fenêtre de lecture : 48-96h (Events Manager → Pixel Hepavix V2 → Purchase events).
- **Review de catégorisation relancée avec le support Meta** : asset fourni (pixel `1369068885114854`, hepavix.com), réponse générique de 1er niveau reçue, relance en cours pour obtenir une **review humaine** avec argumentaire que hepavix.com n'est ni portail patient, ni pharmacie, ni app de télémédecine.
- **Identifiants techniques précisés** : ad account Hepavix = **`CLN_0428-Hepavik`** (ID `1570993443911452`) · store Shopify = **`k1kbc9-mw`** (hepavix.com). ⚠️ Nom différent de `CLN_0428-KN-5` utilisé plus haut (MAJ 08/08) — même préfixe `CLN_0428`, à vérifier si c'est le même compte renommé ou un compte distinct avant la prochaine relance.
- **Confirmé (18/08)** : Hepavix tourne sur le BM opérationnel partagé du portefeuille (celui des 8 ad accounts, cf. plus haut), avec désormais **2 ad accounts actifs** dessus pour Hepavix. Reste à trancher : lequel des deux est `CLN_0428-Hepavik`, et quel est le second — probablement lié à l'ambiguïté `CLN_0428-KN-5` déjà notée ci-dessus.

### 💰 MAJ 2026-08-19 — Top-up confirmé : Hepavix = Kuronet, compte "DRENIA"

- **Confirmé par ID matching** : l'ad account Hepavix `CLN_0428-Hepavik` (ID `1570993443911452`) correspond exactement au compte **« DRENIA »** sur la plateforme de top-up **Kuronet**. Solde vu le 18/08 : **$58,12** (941,88 $ déjà spent). Le top-up Hepavix se fait donc là.
- **Solde actualisé au 21/08 : $293,80** (contre $58,12 le 18/08) — un top-up a été effectué entre les deux relevés.
- **Piège à retenir** : les alias affichés sur Kuronet ne matchent jamais le nom de la brand (Hepavix = « Drenia ») → toujours croiser par **Meta Ad Account ID**, jamais par le nom.
- 🔴 **MAJ 2026-08-24 — solde quasi à sec, recharge nécessaire sous ~4 jours.** Alerte Meta reçue sur le compte (« account spending limit » — pas un ban, juste le plafond = solde rechargé). Solde Drenia ≈ **293 $**, déjà spent ≈ **280 $**. Action : Kuronet → Request Top-up → compte DRENIA (`1570993443911452`) → recharger → l'agence relève le plafond, les ads repartent automatiquement. Rappel : Hepavix est la **seule brand du portefeuille Hugo en compte à top-up** (Aurivo/Nuvalis sont en Clikim auto, jamais de plafond de ce type).

### ✅ MAJ 2026-08-19 — Tracking V2 monté (Rapi CAPI + EasySell), architecture fermée

- **Nouveau pixel « Hepavix V2 »** connecté au compte pub, partagé sur le BM opérationnel début 08/2026 : vivant, réception d'événements confirmée (courbe de PageView active).
- **Architecture retenue (répliquée du setup Aurivo)** : **Rapi Tracking** porte le pixel navigateur sur tout le site, avec la **CAPI Meta activée côté Rapi** — c'est le seul émetteur server-side. **EasySell** reste branché sur les 2 pixels (V1 + V2) pour les events de formulaire COD, **sans CAPI de son côté** (un seul émetteur server-side, sinon doublon de Purchase).
- **Contrôles restants avant scale** : ① vérifier qu'une vraie commande ne génère **qu'un seul** Purchase dans Events Manager (2 = doublon Rapi/EasySell à couper, 0 = CAPI à revoir) ; ② ne jamais activer le canal « Facebook & Instagram » dans Events Manager (pousse du catalogue non voulu) ; ③ désactiver « Automatic page and product detail » dans les settings du dataset.
- **⚠️ Le nettoyage du vocabulaire médical du site (pare-feu domaine) reste à faire** — tant que ce n'est pas fait, le pixel V2 reste exposé à la même catégorisation santé que le V1 (cf. [section pixel flaggé](#-maj-2026-08-08--pixel-hepavix-flaggé--some-website-data-blocked-) ci-dessus). Diagnostics à vérifier chaque matin.

### 🚫 MAJ 2026-08-20 — Confirmation : un pixel neuf + Rapi CAPI ne débloque pas la catégorisation du domaine

- Meta a notifié une restriction sur le `.myshopify.com` du shop — ce n'est **pas** un domaine tiers, c'est l'identifiant technique interne de la même boutique Hepavix (au même titre que `hepavix.com`, `www`, le sous-domaine SK).
- **Conclusion actée** : la cause est le contenu du site, jamais le pixel ni la CAPI — un pixel neuf ne débloque jamais une catégorisation de domaine. Le `.myshopify.com` n'est pas renommable (attribué par Shopify) : seul un rebuild complet de boutique en génère un vierge.
- **Confirme la doctrine déjà posée le 08/08** (cf. ci-dessus) : nettoyer le vocabulaire médical du site AVANT de redemander une review Meta (fenêtre ~06/09), sinon repartir sur une boutique neuve. En attendant, pilotage en UTM/Shopify, pas de coupure des ads live.

### ⭐ MAJ 2026-08-30 — Nouveau pixel de backup « Pixel Hepavix V4 - BM5 backup » sur un nouveau BM (proxy 5)

Suite à un call Ruben × Danila × Hugo du 29-30/08 : identification que le **BM central historique (proxy 4, TVBB Bm3) pouvait lui-même être une cause de flag pixel**, distincte de la catégorisation santé du domaine (les deux mécanismes restent indépendants et cumulatifs — cf. section pixel flaggé du 08/08 ci-dessus).

- **Nouveau BM de backup « BM5 Pay HP 272425 »** (Business portfolio, Business ID `203325125096679`), sur le **proxy 5** (SunBrowser, remplace le proxy 4 pour la création de nouveaux pixels).
- **Pixel « Hepavix V4 - BM5 backup » créé le 30/08, Pixel ID `905536555611383`.** Category vide, CAPI activée à la création. (⚠️ Un ID `1073218318685436` noté d'abord depuis l'URL du popup Meta était faux — toujours confirmer l'ID via Events Manager, à côté du nom du pixel.)
- **Rapi Tracking** : pixel V4 ajouté le 30/08 en config manuelle + jeton CAPI généré (Set up without Dataset Quality API). Pixels V2 et V3 restent présents dans Rapi mais désactivés (toggle OFF).
- **Assign Partner effectué le 30/08** : pixel partagé depuis BM5 vers le BM opérationnel **Abu 3** (Business ID `2097685157511807`, où vivent les ad accounts Hepavix). Reste à faire : Connected Assets côté Abu 3 pour relier le pixel au bon ad account, puis coller le Pixel ID dans EasySell.
- ⚠️ **Choix Hugo (30/08)** : dans le même Assign Partner, les 9 Facebook Pages de BM5 ont aussi été partagées vers Abu 3 (pas juste le pixel) — 2 correspondent aux pages Ezovix déjà documentées, 7 autres d'origine inconnue à date.
- ⚠️ **Rappel doctrine inchangé** : un nouveau BM/pixel règle un éventuel problème de BM restreint, mais **ne règle PAS** la catégorisation santé du domaine si le contenu du site n'est pas nettoyé.

## Stack

| Brique | Outil |
|---|---|
| Boutique | Shopify — hepavix.com |
| Ads | Meta (compte `CLN_0428-KN-5`, 3 pages) |
| Briefs & copies | Notion (semaine « 22/06 → 28/06 ») + ce repo (miroir) |
| Data & décisions | Ce repo + les exports Meta bruts dans [data/](data/) |
| Data Hub historique | Un Google Doc « Hepavix Data Hub » existe (Drive COD EMPIRE) — ⚠️ il contient des doublons créés le 11/07. **Ce repo le remplace comme référence.** |

## Ce qui n'est PAS dans ce repo

Volontairement absent — à demander à Hugo si besoin légitime :

- **Unit economics** : COGS, marges, coûts logistiques chiffrés
- **Accès** : identifiants Business Manager, compte pub, Shopify, Notion
- **Les 2 e-books** offerts (fichiers non archivés)
- **Vidéos HD originales** (versions compressées dans [visuels/videos/](visuels/videos/))
- **Les screenshots du site du concurrent** (24 fichiers, sur le disque d'Hugo)

---

*Navigation : [← 09 — Site & funnel](09-site-funnel.md) · [README (sommaire)](README.md)*
