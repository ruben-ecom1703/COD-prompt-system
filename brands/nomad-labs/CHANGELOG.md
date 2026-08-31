# CHANGELOG

## 2026-08-31 — sync : ROAS par pays et décision scaling (21/08)

- Source : conversation Claude du 2026-08-21 ("Scaling massif & stats live" — citée comme source du sync du 22/08 mais son détail chiffré n'avait pas été repris à l'époque).
- `06-resultats.md` : nouvelle section ROAS 7j glissants par pays (HU 4,89x, SK 7,06x, CZ 6,82x, global 5,52x ; veille HU 4,27x, CZ 5,01x, SK 2,80x ⚠️) + constat stock non limitant.
- `07-relance.md` : décision de scaling ajoutée (tripler progressivement le spend si le ROAS tient, priorité Hongrie, test week-end, palier suivant si ROAS week-end > 4x ; Slovaquie signalée comme marché fragile).
- **Non ajouté / détecté mais ignoré** :
  - Reste de la session du 21/08 (audit HYDRA-X1 vs HYDRA-X2 sur les créas HU, backlog scripts natifs relancé) — déjà couvert par les syncs précédents (22/08 et 29/08), vérifié sans doublon.
  - Chiffres de spend en $ absolus associés à cet arbitrage — filtre bloquant coûts, non repris (seuls les ratios ROAS sont conservés).

## 2026-08-29 — sync : pipeline vidéo natives, recombinaison patterns, expansion DE/AT/SI, incident BM

- Source : conversations Claude du 2026-08-24 au 26 (sessions du jour, hors routine de sync elle-même).
- `04-angles-personas.md` : 5 nouveaux scripts natifs HU (recombinaison de patterns : inversion publique, test invalidant, gaslighting, Bolt × Colonel, débunk expert) + 5 scripts adaptés Primitive Labs (Ads 22-26) + 7 patterns narratifs gagnants récurrents identifiés sur l'historique du compte + expansion marché confirmée (DE/AT/SI)
- `05-ads.md` : pipeline de passage natif → vidéo acté (ElevenLabs EN + doublage HU par Lya), classement des natives pas encore en vidéo par spend (priorité pipeline) + 5 nouveaux concepts statiques BOF (3 adaptés Primitive Labs + 2 originaux) déployés HU/DE/AT/SI
- `06-resultats.md` : pointeur ajouté vers le classement spend natifs (détail dans 05-ads.md)
- `07-relance.md` : chantier vidéo + nouveau lot de scripts ajouté en tête de page + nouveau flow email post-achat (3 guides bonus offerts, localisé DE unifié DE/AT + SI)
- `09-site-funnel.md` : expansion multi-marchés documentée (de.nomadlabs.shop, sl.nomadlabs.shop, AT rattachée au store DE) + bug listing produit DE/AT repéré ("1 500L" au lieu de 400L, même famille d'erreur que le cas HU déjà tracké)
- `10-operations.md` : incident Meta du 26/08 (2 Business Managers agence restreints pour suspicion d'automatisation ; compte pub dédié Nomad Labs confirmé sain) + note workflow monteur (retours "Sylvio" positifs, livraison B-roll à faire par Drive plutôt que zip)
- **Non ajouté / détecté mais ignoré** :
  - Correction potentielle de la couleur produit (une session mentionne un inscription "NOMAD LABS" en noir ; la fiche 01-brand.md actuelle, basée sur des photos produit confirmées le 2026-07-15, indique une inscription blanche) — contradiction non tranchée, **à confirmer avec Ruben avant toute correction** de [01-brand.md](01-brand.md)
  - Idée de SOP "Native Maker" + outil SaaS pour déléguer la traduction/adaptation d'ads à une VA/IA, avec estimation qu'une personne à temps plein serait nécessaire pour l'expansion multi-pays de Nomad Labs seule — décision/outillage au niveau agence, pas une donnée de marque ; non écrit dans ce repo, à re-signaler si ça devient un projet concret
  - Toute donnée chiffrée de prix/coût des guides bonus de l'email post-achat — filtre bloquant prix/coûts, non repris
  - Détail nominatif des 7 patterns narratifs gagnants identifiés — non retrouvé sous forme exploitable dans les extraits disponibles, à compléter dans un futur sync si la liste complète est retrouvée
  - Mention "Onela" isolée (compte pub "CLK_0693-Onela" listé) — aucune information Onela substantielle au-delà de la simple existence du compte, rien à écrire
  - Mention d'une marque "Hepavik"/"Hepavix" côtoyant Nomad Labs et Onela dans une liste de comptes pub et une arborescence de dossiers — hors des 4 marques suivies par cette routine, signalée mais **non traitée** (possible marque d'un autre gérant)

## 2026-08-22 — sync : virage stratégique, bibliothèque organique, 8 briefs, CZ/SK batch 1-2, pattern-level

- Source : vault Obsidian, contenu produit entre le 2026-08-12 et le 2026-08-22 (`bibliotheque-organiques-validee.md`, `statics-readaptation-CZ-SK-higgsfield.md` + `-batch2.md`, `ad-copies-CZ-SK-batch1.md` + `-batch2.md`, `briefs/brief-{demo-muette,tu-boirais-ca,les-resultats-sont-la,tu-penses-toujours-invente,microscope-comparatif,explainer-source,neuf-secondes,test-absurde}.md`, `_context.md` sections "2026-08-12 — Virage stratégique", "2026-08-21 — Scaling massif & stats live", "2026-08-22 — Brief d'itération native ads").
- `04-angles-personas.md` : décision de sortir du mécanisme narratif saturé (signal confirmé par les commentaires, sans chiffres CPA) + learnings de la bibliothèque organique validée (9 vidéos, 3 concepts dérivés) + nouveau pattern "inversion du secret" (script Colonel) + changement de méthode d'itération (POV → pattern-level)
- `05-ads.md` : index des 8 nouveaux briefs vidéo (démo silencieuse, réponse au sceptique, explainer sourcé, déclaration courte, test démonstratif) + référence bibliothèque organique + index des statiques/ad copies CZ/SK batch 1-2 (14 statiques, 14 ad copies) + fiche du nouveau script Colonel (hook HU + traduction FR)
- `07-relance.md` : nouveau chantier pattern-level (livrables en attente) + arbitrage média en cours (décisions de coupe/surveillance/maintien, sans les CPA associés) + lot prêt monteur (8 briefs + CZ/SK batch 1-2, 2 points d'arbitrage ouverts)
- `10-operations.md` : stock mis à jour au 21/08 (réception ~10 000 unités/5 jours, stock estimé ~30 000 unités, pas de risque de rupture)
- **Non ajouté / détecté mais ignoré** :
  - Toutes les données chiffrées de performance du 15-21/08 (stats commandes/CA/ROAS par pays, tableau CPA Meta Ads Manager, classement EU spend Meta Ad Library, chiffres d'arbitrage adsets) — filtre bloquant coûts/marges/unit economics, non repris dans ce sync
  - Texte intégral des 14 statiques (prompts Higgsfield) et des 14 ad copies CZ/SK batch 1-2 — restent dans le vault, résumés seulement ici (même convention que le sync du 12/08)
  - Corps complet du script Colonel — pas encore récupéré côté vault, seul le hook est documenté ; fiche à compléter dans un futur sync
  - Preuve sociale "17 000 familles tchèques/slovaques" sur les ad copies CZ/SK — limite floue (chiffre porté sur un marché où la marque n'a pas encore vendu) : signalée comme point d'arbitrage ouvert dans le repo plutôt que validée telle quelle

## 2026-08-12 — sync : audit perf 11/07-9/08, expansion SK/CZ, hook-lab László, 4 nouveaux scripts, 5 briefs vidéo

- Source : vault Obsidian, sessions du 2026-07-31 au 2026-08-10 (`perf-audit-2026-08-10.md`, `native-ads-repartition-2026-08-10.md`, `expansion-sk-cz-strategy.md`, `research-sk-cz-expansion.md`, `hook-lab-01-laszlo-voisine.md`, `hook-lab-01b-registre-identite.md`, `hook-lab-01c-shortlist-7-charnieres.md`, `laszlo-v2-titkosszolgalat*.md`, `sandor-nyugdij-51-SCRIPT-COMPLET.md`, `briefs/brief-{compte-tes-bouteilles,inondation-60s,la-liste-60s,le-traducteur-60s,les-colis}.md`, fichiers `ad*-SK.md`/`ad*-CZ.md`). Rattrapage : le sync automatisé était resté bloqué depuis le 30/07 (curseur `.last-sync` avancé le 10/08 sans écriture réelle — voir note vault `0 Inbox/2026-08-12-routine-cod-sync-interrompue.md`).
- `06-resultats.md` : nouvel audit perf 11/07→9/08 ($14 815 spend, 1 745 achats, CPA $8,49, ROAS 11,66x reporté / 7,5-8x net COD) + répartition des 13 native ads actives par origine (85% rip concurrent Primitive Labs) + frictions HYDRA-X1/X2 et claim militaire à corriger
- `04-angles-personas.md` : décision d'expansion Slovaquie/Tchéquie (data marché, scores angles par pays, adaptations systématiques) + hook-lab László (décomposition du hook winner + 6 déclinaisons d'identité testables)
- `05-ads.md` : index des 32 ads SK/CZ traduites (pas encore lancées) + 4 nouveaux scripts natifs patchés sur László (László V2, Sándor, Zsolt, Le camion du jeudi) + 5 nouveaux briefs vidéo framework maison
- **Non ajouté** : texte intégral des scripts (László V2, Sándor, Zsolt, Le camion du jeudi) et des 32 fiches SK/CZ — restent dans le vault, résumés seulement dans ce repo (cohérent avec la convention existante de ne pas dupliquer les scripts complets ici) ; configs CommentGuard Onela/Keskia du 06/08 — pas de section dédiée dans la structure du repo, à trancher avec Ruben avant d'en créer une

## 2026-07-30 — sync : créatives Mars Men, briefs monteur, scripts Primitive Labs, audit CommentGuard

- Source : vault Obsidian, sessions du 2026-07-27 au 2026-07-30 (`_context.md`, `statics-readaptation-marsmen.md`, `briefs/`, `script-*.md`, `scripts-testes-periode-essai.md`)
- `04-angles-personas.md` : règles du process de réadaptation statiques Mars Men (structure + POV conservés à 100%, sauf empêchement factuel — déjà tracée dans `memory.md` du vault, non dupliquée en détail) ; palette dédiée fond clair/bleu "hydration"/orange urgence ; note qualité traduction sur les scripts Primitive Labs (incohérence garantie 60j/90j repérée sur 9 des 10 scripts adaptés, à corriger avant envoi monteur)
- `05-ads.md` : 3 nouvelles sections — index des 4 statiques Mars Men réadaptées (scores, décisions clés, bilan portefeuille), index des 8 briefs vidéo monteur (batch face caméra/3D), index des 10 scripts native ads adaptés de Primitive Labs (le script "EMP / Hálózat" marqué faible priorité pour la Hongrie — seul du batch sans narration insider)
- `10-operations.md` : audit CommentGuard (modération commentaires Facebook) — doublon de règle trouvé, 4 nouveaux topics recommandés, activation "Hide impersonators" recommandée, auto-réponses à configurer
- `07-relance.md` : note ajoutée sur le nouveau lot de créatives prêtes pour handoff monteur (statiques, briefs, scripts)
- **Non ajouté** : le débat stratégique rapporté sur la "constellation militaire" (angle #1 crise vs. preuve produit pure pour ouvrir un nouveau TAM outdoor/rando) n'a pas pu être retrouvé, avec les chiffres associés, dans les sources vault disponibles (`_context.md`, briefs, scripts, `scripts-native-ads-batch2.md`) malgré recherche approfondie — à fournir/confirmer avant ajout pour éviter d'inventer des chiffres

## 2026-07-18 — sync : 10-operations.md (stock)

- Source : conversation Claude du 2026-07-17 (chiffres stock donnés directement par Ruben, pas d'export système)
- `10-operations.md` : rempli avec le stock au 17/07 (2 000 unités dispo, +4 000 en douane, +10 000 attendues ~5 août puis 10k/semaine), vélocité de vente (46 cmd/j, 140 items/j), et le calcul de marge avant rupture (~3 340 unités d'avance au 5 août, pas de risque de rupture au rythme actuel)
- Compte pub / logistique 3PL / stack toujours en attente (bloqué par la capture Business Manager, voir 07-relance.md)
- Rien d'autre à rejouer pour Nomad Labs sur cette fenêtre : le contenu scripts/angles des sessions du 16-17/07 était déjà commité (`0368d4d`, `5d75ca0`)

## 2026-07-16 — 4 scripts László passés au stade final + brief monteur

- Source archivée : `data/notes-sessions/2026-07-16-session-scripts-finalises.md` (sync depuis conversation Claude du 16 juillet, 17h46-21h59)
- `04-angles-personas.md` : itérations 1 (László), 2 (Ági), 3 (la fille) et 5 (2ème personne) passent de "script validé en concept" à **script final compressé/traduit + brief monteur complet**, prêtes à être copiées dans le Notion monteur
- `07-relance.md` : les 2 livrables prioritaires (itération 2 Ági, itération 5 2ème personne) marqués comme livrés ; ⚠️ fichiers voix ElevenLabs encore manquants pour itérations 2, 3, 5 (seule l'itération 1 en a un confirmé)
- Rien poussé pour Keskia / Onela / Pulmavi Labs — aucune activité détectée sur ces marques depuis le dernier sync (repos toujours au stade "Initial commit")

## 2026-07-15 — 03/04/05/07 remplis depuis les notes de session créative

- Source archivée : `data/notes-sessions/2026-07-15-session-scripts-video.md` (compte rendu complet fourni par Ruben)
- `04-angles-personas.md` : angles en circulation (Chauffeur Bolt, László, statique "MAJDNEM ELFOGYOTT"), 5 itérations POV du mécanisme László, 5 scripts courts produit — ⚠️ noms d'angles pas encore mappés aux Ad ID du CSV, signal perf déclaré non recoupé
- `03-compliance.md` : chiffres canoniques (400L), incident de cohérence corrigé (1500L → 400L), claim "autorité militaire" flaggé comme sensible/non sourcé, règles B-Roll IA
- `07-relance.md` : plan priorisé (quoi produire, tester, abandonner) + rappel que l'export créatives reste le prérequis avant tout scaling
- `05-ads.md` : règles de production vidéo remplies ; structure de campagne toujours en attente de l'export créatives

## 2026-07-15 — 08-brand-system.md + correction FAQ dans 09-site-funnel.md

- `08-brand-system.md` rempli : palette couleurs extraite du CSS du site live (--orange #e2611c, --charbon #16181a, --sable #d7cfbe + variations), typo (Inter, 700/400)
- ⏳ Packshot et doctrine visuelle des ads winners toujours en attente (créas originales / export créatives)
- **Correction** : `09-site-funnel.md` disait à tort "aucune FAQ" — en fait présente (accordéon HTML natif raté par le premier fetch). FAQ verbatim (6 Q/R) ajoutée.

## 2026-07-15 — 02-concurrent.md enrichi (scan ads + concurrents similaires + emails)

- Scan des 8 ads actives les mieux rangées de Primitive Labs (Brandtracker) : angles regroupés par pattern, jours en ligne, signal de rang — copy exacte non reproduite (droits du concurrent)
- Repéré : 1 winner tourne depuis 69 jours (signal de performance durable)
- Concurrents similaires identifiés (LifeStraw, PureFlow, Icon Lifesaver, Seychelle) — pour info, pas encore documentés en détail
- Stratégie email notée : ~4 emails/semaine, quasi tout promo/urgence

## 2026-07-15 — 02-concurrent.md (Primitive Labs Research)

- Concurrent identifié et confirmé par Ruben : primitivelabsresearch.com (HYDRA-X1, clone direct de notre HYDRA-X2)
- Ajouté au Brandtracker de l'équipe pour suivi continu des ads
- Profil, trafic, catalogue, écarts d'offre (garantie à vie + FAQ chez eux) et pattern d'ads ("advertorial" sous page tierce "USA Ready Families") documentés

## 2026-07-15 — Export perf mis à jour (Ad ID)

- Remplacement du CSV perf par une version incluant la colonne **Ad ID** (24 IDs uniques) — résout l'ambiguïté des noms d'ads dupliqués ("ads 1" apparaissait 5x)
- Colonne revenue toujours absente

## 2026-07-15 — 01-brand.md et 09-site-funnel.md (site live)

- Rempli à partir d'un fetch du site live (https://nomadlabs.shop/) le 2026-07-15 : produit HYDRA-X2, mécanisme, offre 3 paliers, garantie 90j, funnel COD
- ⚠️ Aucune FAQ détectée sur la page (à confirmer manuellement — accordéon JS possible)
- ⏳ Pages Facebook (Link Object ID) pas encore renseignées — en attente de l'export créatives

## 2026-07-15 — Ajout export brut perf Meta

- Ajout `data/exports-meta/CLN_0428-KN-3---Nomadsla-s-Ads-15-Jun-2026-14-Jul-2026.csv` (export Ads Manager, 24 ads, fenêtre 15 juin → 14 juil 2026)
- Fenêtre de dates confirmée par Ruben : testing relancé début juillet, les ~14 derniers jours (inclus dans les 30 jours exportés) sont la donnée pertinente
- ⚠️ Colonne revenue toujours absente de l'export — ROAS/revenue non calculable pour l'instant ; build de 05-ads.md / 06-resultats.md en attente de l'export créatives (item 2/7) pour le croisement nom d'ad + ad set

## {DATE} — Création du repo (build initial)

- {résumé du build}
