# CHANGELOG — journal des mises à jour du repo

> Toute mise à jour s'inscrit ici, datée, la plus récente en haut. Seul le gérant de la brand (Hugo) écrit dans ce repo.

## 2026-08-30 (cod-sync) — Nouveau pixel de backup « Hepavix V4 - BM5 » sur un nouveau BM (proxy 5)

- `10-operations.md` : suite à un call Ruben × Danila × Hugo du 29-30/08, identification que le BM central historique (proxy 4, TVBB Bm3) pouvait lui-même être une cause de flag pixel (mécanisme distinct de la catégorisation santé du domaine). Nouveau BM de backup « BM5 Pay HP 272425 » créé sur le proxy 5, nouveau pixel « Hepavix V4 - BM5 backup » (Pixel ID `905536555611383`), branché sur Rapi Tracking, partagé vers le BM opérationnel Abu 3 avec les 9 pages FB du BM5 (2 identifiées comme pages Ezovix, 7 d'origine inconnue).
- Filtré (bloquant) : rien — aucune unit economics/COGS/marge, aucun mot de passe/token/secret (seuls des IDs d'assets Meta, déjà le format utilisé partout ailleurs dans ce fichier), aucun lien `[[wiki]]`. Vérif liens/ancres : 0 cassé.

## 2026-08-28 (cod-sync) — Les 35 prompts d'images du batch Ritual Labs écrits et posés sur Notion

- `07-relance.md` : nouvelle section en tête — PHASE 2 débloquée (30 briefs visuels du 22/08 n'avaient jamais eu de prompt prêt à coller dans ChatGPT). 7 fiches natives traitées, 35 prompts au format trame validée par Hugo, exception de bloc réalisme pour les 2 illustrations médicales (R1-1/R1-2), contraintes hongrois/produit/scans intégrées, angle alcool documenté.
- Filtré (bloquant) : rien — aucune unit economics/COGS/marge, aucun identifiant/secret, aucun lien `[[wiki]]`.
- Non routé : le contenu intégral des 35 prompts (texte à coller dans ChatGPT) reste sur Notion — ce repo garde le résumé traçable (structure, exceptions, contraintes), pas le verbatim.

## 2026-08-25 (cod-sync) — Audit pré-lancement V3 (25/08) : 4 rouges avant le 26/08 00h00

- `07-relance.md` : nouvelle section en tête — audit de la relance « 26/08/2026 - V3 Campagne Hepavix HU » (17 ads, pixel V3 `2133570580843947`). 4 bloquants non corrigés au moment du sync (liens `.com` dans 13 copies, « 80 % » silymarine sur 3 copies testing, 7 mots hongrois cassés sur Ads 12, Advantage+ enrollé) + points à trancher (handle produit avec claims, page « Varga Nóra Szexológus » incohérente avec le narrateur) + décision actée (domaine primaire Shopify reste `.com`, CAPI Rapi+EasySell gardé, UTM en cours de pose).
- Filtré (bloquant) : rien — aucune unit economics/COGS/marge, aucun identifiant/secret, aucun lien `[[wiki]]`. Statut des 4 rouges non confirmé corrigé au moment du sync — à revérifier au prochain run.

## 2026-08-24 (cod-sync) — PHASE 3 faite (pages persona créées) + chiffres stock réels + alerte top-up

- `01-brand.md` : section Pages Facebook — **PHASE 3 faite**, les 2 pages (Nagy István, Kovács Éva) sont créées avec leurs bios (bio neutre sans métier — leçon actée après un premier essai « Ápolónő » contredisant 3 des 4 copies routées dessus), mapping final audité et figé (Dr. Tóth Petra garde ses 2 natives, pas de 3e page femme médicale créée).
- `02-concurrent.md` : « PHASE 3 (à venir) » → « PHASE 3 FAITE (24/08) ».
- `07-relance.md` : bandeau de statut + section Production natives mises à jour (PHASE 3 faite) + alerte top-up ajoutée au bandeau.
- `10-operations.md` : nouvelle section stock (MAJ 24/08) — cadence réelle confirmée par Hugo 100-150 articles/j (2× l'estimation du 06/08), lead time réel 2-3 semaines (pas 45 j), point de commande recalculé (~3 100 u), scénario scale 5k€/day, **recommandation : commander ~20 000 unités maintenant**. Nouvelle section top-up (MAJ 24/08) — solde Drenia/Kuronet quasi à sec (~293 $ solde, ~280 $ spent), alerte Meta « account spending limit » sous ~4 jours, action = recharger Drenia sur Kuronet.
- `README.md` : timeline complétée (24/08).
- Filtré (bloquant) : **le coût unitaire (~3,2 €/u) et le montant cash du réassort (~64 K€) présents dans la source vault n'ont volontairement PAS été recopiés** (unit economics/COGS) — seules les quantités en unités et les dates sont reprises. Aucun identifiant/secret nouveau, aucun lien `[[wiki]]`.
- Non routé : rien d'autre cette fenêtre pour Hepavix.

## 2026-08-22 (cod-sync, suite) — Décision scaling agressif pendant le préavis pixel

- `07-relance.md` : nouvelle section **Décision 22/08 : scaler AGRESSIVEMENT pendant les 30 jours de préavis pixel** — plutôt que freiner, doublement du budget acté avec les associés dès le 22/08 au soir puis hausse quasi quotidienne, ~50 natives produites pour alimenter le scaling, stock jugé large (~10 000 unités, 25-30j). Risque de retour à zéro (re-phase d'apprentissage) assumé si la review échoue. Piste de cloaking évoquée mais explicitement non retenue, gardée pour mémoire.
- Filtré (bloquant) : rien de nouveau — pas de COGS/marge/P&L, pas d'identifiant/token/secret, pas de lien `[[wiki]]`.

## 2026-08-22 (cod-sync) — Tracking V2 fermé, batch natives (Ads 2 + Ads 12 + concurrent Ritual Labs), pages persona actées, recherche personas Reddit/HU

- `10-operations.md` : solde Kuronet DRENIA actualisé ($293,80 au 21/08, contre $58,12 le 18/08) ; nouvelle section **Tracking V2 monté** (Rapi Tracking = pixel navigateur + CAPI, EasySell = events formulaire sans CAPI, contrôles restants avant scale) ; nouvelle section **test tranché 20/08** confirmant qu'un pixel neuf + Rapi CAPI ne débloque jamais une catégorisation de domaine (le `.myshopify.com` du shop se refait flag comme `hepavix.com`).
- `07-relance.md` : nouvelle section **Production natives en cours (19-22/08)** — statut du batch « 19/08/2026 — Ads » (7 copies itérées du winner Ads 2, hooks refaits le 21/08, visuels natives 3/4/5 livrés, native 6 partielle) ; batch Ads 12 « Anna, l'hôtesse Airbnb » clos à 3 fiches (2 ventes = pas un winner) ; itérations concurrent Ritual Labs PHASE 1 terminée (6 ads clonées, 7 fiches) et PHASE 2 (30 briefs visuels) validée ; nouveau format de fiche Notion (en-tête 5 éléments, changements en rouge, FR du concurrent en vis-à-vis).
- `01-brand.md` : nouvelle section — noms et photos des 2 pages persona actés (Kovács Éva / Nagy István), pas encore créées, plan de chauffe avant mise en ads.
- `02-concurrent.md` : nouvelle section **Itérations clonées — batch natives concurrent** — tableau des 6 ads Ritual Labs sources (IDs Meta), classification, adaptations HU, page Hepavix de routage ; état des phases 2 et 3.
- `04-angles-personas.md` : nouvelle section **Recherche personas Reddit + marché hongrois** — 8 nouveaux angles (A8-A15), mécanisme nommé « capsule de Glisson », TAM hongrois (~3M personnes), trous concurrentiels (GymBeam/Hepadex/Legalon), nouvelles objections FAQ (diarrhée, interactions antihypertenseurs, acheteur-proxy).
- Filtré (bloquant) : les identifiants pixel/ad account/IDs Meta d'ads concurrentes = identifiants techniques déjà admis dans ce repo (pas des secrets) ; le solde de top-up n'est pas une unit economics (pas de COGS/marge) ; les verbatims Reddit/HU ont été résumés en conclusions actionnables plutôt que recopiés intégralement ; tous les liens `[[wiki]]` du fichier de recherche source ont été retirés au profit de texte descriptif ; aucun token/mot de passe/2FA mentionné.
- Non routé (signalé, pas tranché) : le solde de top-up mis à jour concerne un compte publicitaire dont l'identité exacte reste ambiguë depuis le 17/08 (`CLN_0428-Hepavik` vs `CLN_0428-KN-5`, cf. `10-operations.md`) — non résolu par ce run, signalé à Hugo.

## 2026-08-19 (cod-sync) — Top-up confirmé : compte Kuronet "DRENIA"

- `10-operations.md` : nouvelle section MAJ 19/08 — l'ad account Hepavix `CLN_0428-Hepavik` (ID `1570993443911452`) identifié par matching d'ID comme le compte **« DRENIA »** sur la plateforme de top-up Kuronet, solde $58,12 (941,88 $ spent) au 18/08. Règle ajoutée : toujours croiser par Meta Ad Account ID, jamais par le nom affiché sur Kuronet.
- Filtré (bloquant) : rien — donnée de solde de top-up (pas une unit economics COGS/marge), aucun identifiant de connexion, aucun lien `[[wiki]]`.
- Non routé : rien d'autre cette fenêtre pour Hepavix.

## 2026-08-18 (cod-sync) — Clarification : 2 ad accounts actifs sur le BM opérationnel partagé

- `10-operations.md` : le signal faible non confirmé du 17/08 (mention tronquée d'un possible 2e ad account) est confirmé — la phrase source n'était pas coupée. Hepavix tourne bien sur le BM opérationnel partagé du portefeuille avec **2 ad accounts actifs**. Reste ouvert : lequel des deux est `CLN_0428-Hepavik`, quel est le second.
- Filtré (bloquant) : rien — pas d'unit economics, pas de secret/token. Le nom nominatif de l'admin du BM (cité dans le vault) est volontairement omis ici, conformément à la convention déjà en place dans ce repo (le BM est désigné "opérationnel partagé", jamais nommé).
- Non routé : aucun autre item cette fenêtre — audit complet des 6 autres brands du portefeuille (Aurivo, Nuvalis, Ezovix, Khloris, Nomad Labs, Keskia, Onela, Pulmavi Labs, Vitora, Sonira, Leurovix, Nixela) n'a rien remonté de nouveau.

## 2026-08-17 (cod-sync) — Test pixel V2 + review Meta relancée + identifiants ad account/store précisés

- `10-operations.md` : nouvelle section MAJ 17/08 — nouveau pixel "Hepavix V2" créé et connecté à EasySell (test réversible, ne débloque pas le flag domain-level, fenêtre de lecture 48-96h) ; échange support Meta en cours pour obtenir une review humaine de la catégorisation ; ad account précisé (`CLN_0428-Hepavik`, ID `1570993443911452`) avec flag de vérification vs le nom `CLN_0428-KN-5` déjà documenté ; store Shopify précisé (`k1kbc9-mw`).
- Filtré (bloquant) : rien — aucune unit economics/COGS/marge, aucun secret (IDs pixel/ad account/store = identifiants d'exploitation, pas des tokens ni des mots de passe), aucun lien `[[wiki]]`.
- Non routé : un signal faible et non confirmé (mention tronquée d'un possible 2e ad account sous le même BM) — laissé côté vault uniquement, à vérifier auprès d'Hugo avant toute documentation repo.

## 2026-08-09 (cod-sync) — Migration abandonnée, relance sur le compte de base, pixel flaggé, itérations en attente

- `10-operations.md` : mise à jour du statut de campagne — le projet de migration vers un nouveau compte (`ReStart 07/08/26`) a été **abandonné** ; la campagne « 26/06/26 Hepavix » a été **relancée sur le compte de base** (`CLN_0428-KN-5`, 150 $/j, 16 ads d'origine). Nouvelle checklist de relance (couper Ads 10 et Ads 12, ne pas éditer les copies à 80 % en pleine diffusion, UTM manquants sur les 17 ads, 3 ads sans visuel documenté). Nouvelle section — **pixel Hepavix flaggé « Some website data blocked »** (08/08) : domaine catégorisé « Health & wellness conditions » par Meta, review en attente, plan d'action aligné sur le playbook déjà documenté pour Aurivo, et repères marché sur les workarounds du vertical santé (non garantis).
- `07-relance.md` : statut mis à jour (relance sur compte de base, pixel flaggé), nouveaux items bloquants en Étape 0 (pixel, coupe Ads 10/12), nouvelle section Étape 4 — **3 itérations rédigées du winner** (hook visage, hook ashwagandha, preuve sociale en hook), en attente du GO d'Hugo, rien posé sur Notion.
- `01-brand.md` : statut de campagne mis à jour (relance 07/08 + pixel flaggé 08/08).
- `04-angles-personas.md` : mise à jour de l'idée « preuve sociale en hook » — désormais rédigée comme itération 3, renvoi vers 07-relance.md.
- `08-brand-system.md` : nouvelle section Logo — exploration en cours (7 directions briefées, 4 générées, batch interrompu par une panne du connecteur, aucun choix fait).
- `README.md` : statut, timeline (06/08 → 08/08) et liste « À savoir » mis à jour avec l'alerte pixel.
- `ads/cardiologie-ce-quon-ne-dit-pas.md` (Ads 10) et `ads/statines-airbnb.md` (Ads 12) : flag « coupée à la relance du 07/08 ».
- Filtré (bloquant) : rien — aucune unit economics/COGS/marge, aucun identifiant/token/secret (le pixel et l'ad account sont des identifiants techniques déjà documentés ailleurs dans ce repo), aucune donnée Marco Moretti/perso, aucun lien `[[wiki]]` (remplacés par du texte descriptif, y compris le pointeur croisé vers le repo Aurivo qui reste en langage naturel, pas un lien).

## 2026-08-07 (cod-sync) — Import RESTART livré, arbitrage 3 pages tranché, idée d'angle hook

- `10-operations.md` : nouvelle section — fichier d'import RESTART (16 ads, 3 ad sets un par page, budget 50 $/j warm-up CBO, pixel conservé, corrections copy silymarine 90 % + 10 mots hongrois réparés sur l'ad Airbnb, flags dosage/titre/disclaimer laissés verbatim).
- `07-relance.md` : arbitrage tranché — non à la page unique, répartition des 3 pages confirmée et affinée (Dr. Tóth Petra = médecin Hepavix only, page marque = statics/offres, nouvelle page femme lambda pour récits pair-à-pair), lecture croisée avec la veille Ritual Labs.
- `01-brand.md` : section Pages Facebook complétée avec l'arbitrage et le plan de dilution (2-3 nouvelles pages médecin).
- `04-angles-personas.md` : nouvelle idée non qualifiée dans « Territoires jamais explorés » — preuve sociale (2 184 avis/4,8) en hook, angle inspiré de Ritual Labs.
- Filtré (bloquant) : rien — aucune unit economics/COGS/marge, aucun identifiant/token/secret (le pixel et l'ad account sont des identifiants techniques déjà documentés ailleurs dans ce repo, pas des accès), aucun lien `[[wiki]]`.

## 2026-08-06 (cod-sync) — Stock confirmé 10k, veille concurrent Ritual Labs, rattachement BM

- `10-operations.md` : nouvelle section couverture stock (06/08) — 10 000 unités confirmées, ~154 j de couverture à 150 $/j (scénarios à 300/600 $/j inclus), c'est la brand qui peut le plus encaisser le scale Q4. Nouvelle section rattachement au BM opérationnel partagé du portefeuille (06/08), avec flag d'ambiguïté sur le compte pub exact (conflit avec Nuvalis, non résolu).
- `02-concurrent.md` : nouveau relevé de veille daté 06/08 (Brandsearch) — Ritual Labs Happy Liver passé à 219 ads/147 actives, stratégie confirmée sur une seule page marque (test page persona abandonné côté concurrent).
- Filtré (bloquant) : rien — aucune unit economics/COGS/marge, aucun identifiant/token/secret, aucun lien `[[wiki]]`.

## 2026-07-15 (cod-sync) — Packaging, SAV IA, anti-rejet Meta, page partagée

- `10-operations.md` : écart entre le packaging du site et le colis réellement expédié (même packaging que Nuvalis, nouveau label) — risque de refus de colis en COD.
- `10-operations.md` (via note ci-dessus) : upsell croisé confirmé en prod sur le bot SAV IA quand la question dérive vers un humain.
- `07-relance.md` : nouvelle section anti-rejet Meta (post ID organique, sous-domaine tampon clean, agency ad account).
- `07-relance.md` : alerte — la page « Dr. Tóth Petra » (winner Ads 2) est partagée avec une autre brand du portefeuille ; risque de perte du winner si l'autre brand se fait flaguer.

## 2026-07-14 (bis) — Corrections issues de l'audit

Un agent testeur n'ayant QUE ce repo a audité chaque chiffre contre la donnée brute et relu les 16 copies hongroises. Le socle factuel est passé (perf, pages FB, copies : exacts au centime et au caractère). **Mais l'audit a trouvé que des défauts documentés comme propres à une seule ad en contaminaient plusieurs autres — dont deux qu'on s'apprêtait à financer.** Corrections :

- 🔴 **Le dosage « 3 gélules/jour » (au lieu de 2) ne concerne pas qu'Ads 12** : il est aussi dans **Ads 4** — l'ad que le plan de relance programmait explicitement pour un test — et dans **Ads 14**. On allait payer pour diffuser une ad qui contredit le site. Les 3 fiches sont désormais flaguées.
- 🔴 **Le titre orphelin « Katalin » ne concerne pas qu'Ads 12** : il est aussi sur **Ads 10** — qui est **le seul vrai échec financé de la campagne** (13,09 $, 0 vente). Un titre qui promet une histoire que le texte ne raconte pas : c'est une piste sérieuse pour expliquer cet échec. Flagué.
- 🔴 **La copy d'Ads 12 réellement diffusée contient des mots hongrois cassés** (`üvegtutty`, `Ednyény`, `fótelk`, `eskeuvőjéről`…). Un faux témoignage avec des fautes de hongrois = crédibilité détruite. Relecture par un natif désormais exigée avant relance.
- 💡 **Ads 8 — la variante du winner, jamais diffusée (0 $) — était absente du plan de relance.** Même angle, même titre, même page, corps différent : c'est le test le moins cher et le plus évident de la relance. Ajoutée en Étape 1.
- ❌ **« 5 ads n'ont jamais eu de budget » était faux : elles sont 11.** Corrigé partout (le « 5 » venait d'une confusion avec les 5 *angles* jamais testés).
- 🟠 Ads 12 est en **tegező** alors que la règle de la brand est le **magázó** — incohérence de registre, jamais signalée. Flaguée.
- 🟠 **Ads 17** mélange deux ads (le titre d'un angle, le texte d'un autre). Flaguée.
- 🟠 **Le disclaimer obligatoire n'apparaît dans aucune des 16 copies diffusées** — la règle a été posée le 26/06, la campagne lancée le 27/06. À trancher avec Hugo : les ads diffusées ne sont pas conformes à notre propre règle.
- 🟡 Colonne « Revenue » du tableau par page : arrondis faux (2 332,34 → **2 332,20** · 222,85 → **222,80** · 155,96 → **155,99**). La somme tombe maintenant exactement sur 2 710,99 $.
- 🟡 `ads.json` : ajout des **chemins réels des visuels** dans le repo (avant : le nom d'asset Meta, inexploitable), des **défauts par ad**, et du flag `jamais_reellement_testee`.
- 🟡 Fiches Ads 10 / 14 / 15 : la ligne « Visuel » disait « aucun fichier image dédié » alors que l'ad avait bien une image — simplement pas archivée ici. Reformulé.

## 2026-07-14 — Création du repo (annuaire complet)

- **Structure complète** : README (routing + timeline + glossaire), 01-brand → 10-operations, ads/, visuels/, assets/, data/.
- **Les 17 copies d'ads** : transcrites depuis l'**export de créatives Meta** = le texte **exactement tel qu'il a été diffusé** (et non le brief Notion). Les 4 ads qui ont vendu ont en plus leur traduction française intégrale.
- **Performance recalculée depuis les exports bruts** (fournis par Hugo le 14/07) : croisement du CSV de performances (`CLN_0428-KN-5`) et de l'export de créatives, sur le nom d'ad. **Contrôle réussi : 306,95 $ / 41 ventes / ROAS 8,83** — la somme des 17 ads recoupe exactement le total de la campagne.
- **Pages Facebook vérifiées** depuis la colonne `Link Object ID` (et non depuis une note) : Dr. Tóth Petra (36 ventes) · Hepavix marque (3) · Varga Nóra (2).
- 🔴 **Règle du 90 % documentée et flaguée** : le site est bien à 90 % (vérifié en ligne), mais **3 copies historiques disent 80 %** — dont le winner. Chaque fiche concernée porte un avertissement. Les autres « 80 % » (choline, cholestérol) sont des claims différents et n'ont pas été touchés.
- **Assets** : 13 statics publiés, le packshot officiel, 4 vidéos, 9 b-rolls, les 8 visuels d'ads du concurrent — tous compressés.
- **Veille concurrent** : Ritual Labs au 14/07 (108 ads actives, 98 669 visites/mois) + leur nouvelle promo BOGO du 23/06 (« We Made Too Much Happy Liver »).
- **Pièges documentés** : le ROAS 66,95 d'Ads 5 (sur 2,33 $), la page Dr. Tóth Petra qui diffuse aussi 15 ads Khloris, l'hôtesse Airbnb publiée depuis une page de sexologue, les 3 défauts d'Ads 12 (titre orphelin, Thanksgiving, dosage).
