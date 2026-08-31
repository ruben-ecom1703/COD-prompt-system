# 07 — Plan de relance (actions priorisées)

> 📅 Dernière mise à jour : 2026-08-28 · Statut : campagne « 26/06/26 Hepavix » **relancée le 07/08 sur le compte de base** (150 $/j, 16 ads d'origine) — migration ReStart abandonnée · 🚩 pixel flaggé « Some website data blocked » le 08/08, confirmé domain-level le 20/08 → [10-operations.md](10-operations.md#-maj-2026-08-07-suite--import-abandonné-relance-sur-le-compte-de-base) · 🔴 **top-up Drenia/Kuronet quasi à sec (24/08)** → recharge sous 4 jours, [10-operations.md](10-operations.md#-maj-2026-08-19--top-up-confirmé--hepavix--kuronet-compte-drenia) · 🚨 **audit pré-lancement V3 (25/08) : 4 rouges à régler avant le 26/08 00h00** (ci-dessous) · 🎨 **35 prompts d'images du batch Ritual Labs écrits et posés le 28/08** (PHASE 2 débloquée, aucun visuel encore généré) · Gérant : Hugo

**Hepavix = la 2e priorité du portefeuille à la relance** (ROAS 8,83, juste derrière Ezovix). Sa force : on sait exactement ce qui marche. Sa fragilité : **tout repose sur une seule ad**.

---

## 🎨 MAJ 2026-08-28 — Les 35 prompts d'images du batch Ritual Labs écrits et posés sur Notion

Suite directe de la PHASE 2 (30 briefs visuels validés le 22/08) : les briefs décrivaient les visuels en tableau, mais aucun prompt prêt à coller dans ChatGPT n'existait — Hugo ne pouvait donc pas générer. Comblé le 28/08.

- **7 fiches natives traitées, 35 prompts au total** (5 par fiche), posés dans chaque fiche juste sous son tableau de briefs (jamais sur la page de référence) : R1 · R1b · R2 · R3 · R4 · R5 · R6.
- **Format** : trame validée par Hugo (français parlé, description « on voit que… », prise de vue nommée, défauts de photo assumés, anti-liste) + paragraphe réalisme verrouillé recopié mot pour mot en fin de chaque prompt.
- **🔴 Exception au bloc réalisme** : R1-1 et R1-2 sont des illustrations médicales 3D fond blanc (foies) — le bloc « qualité iPhone, photo amateur » y serait contre-productif. Elles portent un bloc de contraintes adapté au rendu médical (illustration de labo, fond blanc, anatomiquement juste, aucune photo). Règle générale retenue : bloc réalisme = photos réelles uniquement, tout visuel schématique a son propre bloc de fin.
- **Contraintes intégrées** : textes hongrois donnés au caractère près (progression ALT/AST, `Laboreredmény`, `Fibroscan eredmény` F2→F3), photo produit à joindre dans ChatGPT pour les 3 visuels montrant le flacon (R2-1, R2-4, R6-2) sinon l'étiquette est inventée, scans médicaux volontairement illisibles (aucun logo d'hôpital, aucun nom de patient).
- **Angle alcool** : les 2 visuels à alcool visible (R1b-1 bouteille de bière, R5-3 verres de vin) portent le rappel du retest assumé et du compteur de refus. R1b-2 reste le plan B sans bouteille.
- 🔴 **Statut inchangé : aucun des 35 visuels n'est encore généré** — la phase suivante est la génération elle-même.

## 🚨 MAJ 2026-08-25 — Audit pré-lancement « 26/08/2026 - V3 Campagne Hepavix HU » : 4 rouges, pas un GO en l'état

- **Contenu prévu** : 17 ads, 1 adset « Adset 1 - Static/Native », CBO 150 $/j, Sales/PURCHASE, HU 18-65, départ 26/08 00h00. Copies historiques du testing (statics + natives + 2 vidéos) + 2 natives from scratch. **Pixel V3 = `2133570580843947`** (nouveau, ni V1 ni V2).
- **🔴 Les 4 bloquants (statut au check : non corrigés)** :
  1. 13 ads sur 17 ont encore `hepavix.com` (domaine flaggé) écrit en toutes lettres **dans le corps de la copy** (pas juste le bouton, déjà propre en `.shop`) — Ads 1, 2, 3, 4, 5, 6, 7, 8, 9, 12, 14, 15-Copy, 16. Fix : remplacer `.com`→`.shop` dans les bodies.
  2. « 80 % » de silymarine dans 3 copies du testing d'origine (Ads 1, 2, 3) — règle produit = **90 %, jamais 80**.
  3. Ads 12 relancée avec ses 7 mots hongrois cassés (faux hongrois documenté depuis le 14/07, jamais corrigé).
  4. Advantage+ enrollé sur les 17 ads (`USER_ENROLLED_AUTOFLOW`) — à décocher.
- **🟠 À trancher/vérifier** : handle produit `.shop` contient les claims en clair (risque re-flag rapide, changer avant lancement = indolore, après = casse les 17 ads) · confirmer que le Pixel ID dans EasySell = bien le V3 · 4 pages FB dans le même adset dont **« Varga Nóra Szexológus »** (narrateur infirmière sur page sexologue, incohérence narrateur↔page, partagée avec Khloris) sur 4 ads — à trancher (garder ou router vers Kovács Éva) · « Ads 15 native from scratch – Copy 2 » = brouillon fantôme à supprimer.
- **✅ Décision actée : domaine primaire Shopify reste `hepavix.com`** (pas de bascule vers `.shop`) — `.com` spend 650 $/j et convertit bien, changer le primaire risquerait de perturber le learning de la campagne live. `.shop` reste connecté en secondaire, sert de lien propre dans les nouvelles copies + UTM.
- **CAPI confirmé** : setup Rapi + EasySell combinés gardé tel quel (886 PageView reçus, courbe active).
- **UTM en cours de pose** sur chaque ad (`utm_source=facebook&utm_medium=paid&utm_campaign={{campaign.name}}&utm_content={{ad.name}}`), champ « URL parameters » — filet de sécurité si le pixel V3 redevient aveugle, vérif via Shopify → Commandes.
- **Lien produit `.shop`** : `https://hepavix.shop/products/hepavix-gyogyszereszeti-minosegu-majvedelem-es-regeneracio`.
- ⏳ **À revérifier au prochain sync** : les 4 rouges corrigés avant 00h00 le 26/08 ? Décision sur la page Varga Nóra Szexológus ?

## Étape 0 — Sécuriser l'actif (bloquant)

- [ ] 🚨 **Séparer la page « Dr. Tóth Petra » de Khloris.** Cette page porte **36 des 41 ventes** de Hepavix — et elle diffuse aussi **15 ads Khloris**. Si Khloris se fait flaguer, on perd le meilleur asset du portefeuille. → Créer une page ménopause dédiée à Khloris ; Dr. Tóth Petra reste à Hepavix, seule.
- [x] Stock vérifié — **10 000 unités confirmées** ([10-operations.md](10-operations.md#-maj-2026-08-06--stock-confirmé-10-000-unités-couverture-large)), ~154 j de couverture à 150 $/j.
- [ ] 🚩 **Traiter le pixel flaggé** (« Some website data blocked », détecté 08/08) : poser les UTM sur les 17 ads live (URL Tags vides), suivre chaque jour si des Purchase remontent encore, préparer le Plan B domaine si la review est refusée. Détail complet → [10-operations.md](10-operations.md#-maj-2026-08-08--pixel-hepavix-flaggé--some-website-data-blocked-).
- [x] Campagne relancée le 07/08 sur le **compte de base** (`CLN_0428-KN-5`, 150 $/j, 16 ads d'origine) — le projet de migration vers un nouveau compte a été abandonné. ⚠️ Elle repart avec ses défauts d'origine non corrigés : **couper Ads 10 et Ads 12** dès que possible (détail [10-operations.md](10-operations.md#-maj-2026-08-07-suite--import-abandonné-relance-sur-le-compte-de-base)).

### 🏛️ Arbitrage tranché 2026-08-07 — NON à la page unique

Question posée : regrouper toutes les ads sur la seule page « Dr. Tóth Petra » ? **Réponse : non**, le setup 3 pages est confirmé et affiné :

| Page | Rôle confirmé | Ventes (testing) |
|---|---|---|
| **Dr. Tóth Petra Menopauza szakértő** | advertorials médecin Hepavix **only** — Khloris déménage sur sa propre page | 36 |
| **Hepavix (page marque)** | statics + offres directes | 3 |
| **Varga Nóra Szexológus** | ⚠️ origine inconnue (ni ce repo ni le vault ne la documentent) — récits pair-à-pair type « femme lambda », pas de casting médecin/sexologue sur un récit qui n'en a pas besoin | 2 |

**3 raisons** : (1) le narrateur doit coller à la page — une doctoresse qui balance une promo ou gère un Airbnb casse la crédibilité, c'est l'erreur inverse de [Ads 12](ads/statines-airbnb.md) sur la page sexologue ; (2) concentration du risque — cette page porte 36/41 ventes **et** 15 ads Khloris, un flag Meta perd les deux d'un coup, le plan dit diluer, pas concentrer ; (3) plafond technique d'ads actives par page (rappel structurel du portefeuille).

**Plan** : Dr. Tóth Petra → advertorials médecin Hepavix uniquement · 2-3 nouvelles pages médecin pour diluer la même copy winner · page marque → statics et offres directes · une page femme lambda (type Kovács Éva) pour les récits pair-à-pair.

💡 **Lecture croisée avec la veille concurrent** : Ritual Labs (147 ads actives, quasi tout sur sa page marque unique) charge surtout des statics d'offre/preuve sociale sur cette page — cohérent avec le rôle qu'on donne à notre page marque. Leur volume d'advertorials longs reste minoritaire ; c'est là que l'edge Hepavix (advertorial médecin) reste différenciant.

## Étape 1 — Scaler le winner, sans le casser

- [ ] **Remettre du budget sur [Ads 2](ads/cortisol-winner.md)** (250,09 $ · 36 ventes · ROAS 9,33). C'est la seule chose qui a prouvé qu'elle vend à l'échelle.
- [ ] 🔴 **Avant toute nouvelle version : corriger la silymarine 80 % → 90 %** dans la copy ([03-compliance.md](03-compliance.md#la-règle-du-90--silymarine)).
- [ ] 💡 **Lancer [Ads 8](ads/cortisol-variante.md) — l'actif dormant.** C'est la **variante du winner déjà écrite** : même angle, même titre, même page, corps différent — et elle n'a **jamais été diffusée (0 $)**. C'est exactement « changer un seul élément à la fois », sans rien produire. **Le test le moins cher de toute la relance.**
- [ ] **Doctrine de scale (règle d'Hugo)** : ne changer **qu'UN seul élément à la fois** — le hook/titre, OU le visuel, OU l'ouverture, OU la page. **Jamais élargir à un autre symptôme.** L'angle reste strictement « ventre / cortisol / foie ».
- [ ] **Diluer le risque de page** : créer 2-3 pages « médecin / expert santé » supplémentaires (noms et photos différents) et y faire tourner la même copy. Aujourd'hui tout dépend d'une seule page.

## Étape 2 — Réparer ce qui est déjà rentable

- [ ] **[Ads 12](ads/statines-airbnb.md) (l'hôtesse Airbnb) : la basculer sur une page persona « femme 55-65 »**, pas une page de sexologue. Le narrateur doit coller à la page. Elle est rentable (ROAS 6,35) **malgré** ce handicap.
  - ⚠️ **Mais ne pas la relancer telle quelle : elle a 5 défauts**, dont des **mots hongrois cassés** dans le texte diffusé (`üvegtutty`, `Ednyény`, `fótelk`…). Un témoignage « authentique » avec des fautes de hongrois ne convainc personne. **Relecture par un natif obligatoire** avant relance. Détail : [03-compliance.md](03-compliance.md#défauts-à-corriger-avant-réutilisation).
- [ ] **[Ads 5](ads/offre-ldl-directe.md) : lui donner un vrai budget.** Coût par vente de 1,17 $ — le meilleur de la campagne — mais sur **2,33 $ de dépense seulement**. Ça ne prouve rien encore : c'est exactement pour ça qu'il faut la financer et voir si ça tient.
- [ ] **[Ads 6](ads/alcool-detox.md)** (alcool, ROAS 20,75 sur 3,22 $) : même logique, à rescaler pour confirmer.

## Étape 3 — Donner leur chance aux jamais-testées

**11 ads** ont reçu moins de 3 $ (parfois 3 centimes) et n'ont jamais eu leur chance. Ce ne sont pas des losers — mais elles ne se valent pas :

- [ ] 🥇 [**Ads 4 — l'infirmière**](ads/infirmiere-statines.md) : **20 423 caractères, la copy la plus travaillée de la brand, 3 centimes de budget.** Elle mérite un vrai test.
  - 🔴 **AVANT de la financer : corriger le dosage.** Sa copy dit « **Naponta három kapszula** » (3 gélules/jour) alors que la posologie officielle est **2/jour**. On s'apprêtait à payer pour diffuser une ad qui contredit le site.
- [ ] Les ads d'offre et statics jamais financés : [Ads 7](ads/offre-ldl-sztatin.md) · [Ads 1](ads/ingredient-mariatovis.md) · [Ads 3](ads/alcool-detox-dynamique.md) · [Ads 11](ads/alcool-8-semaines.md). Peu coûteux à retester, l'angle offre a déjà prouvé qu'il convertit.
- [ ] Les 2 vidéos ([Ads 16](ads/video-cholesterol-statine.md), [Ads 17](ads/video-mariatovis-dilue.md)) : jamais diffusées. ⚠️ Ads 17 mélange deux ads (titre d'un angle, texte d'un autre) — à trancher avant.
- [ ] [Ads 14 — Eszter / le père](ads/eszter-pere.md) et [Ads 15 — Zsuzsa / la fatigue](ads/zsuzsa-fatigue.md) : ⚠️ **Hugo a tranché : ne pas les relancer en priorité** (personas écrits mais jamais rentables). Et Ads 14 a aussi le **défaut du dosage à 3 gélules**.

## Étape 4 — Itérer sur le style qui gagne

- [ ] **Décliner le visuel du winner** : le dessin simple, deux silhouettes, fond blanc, aucun produit. Variantes à produire : la même comparaison vue de face, une progression semaine 0 → semaine 8, un schéma du foie qui « rattrape son retard ».
- [ ] **Ne jamais montrer le produit** dans un visuel de native ad. Le packshot reste pour les ads d'offre sur la page marque.

### ⏳ 3 itérations du winner rédigées — en attente du GO d'Hugo (08/08)

Le défaut d'[Ads 8](ads/cortisol-variante.md) (la variante dormante du winner) est que sa différence avec [Ads 2](ads/cortisol-winner.md) est **invisible dans le feed** (même titre, même visuel). Objectif de ces 3 itérations : demande d'Hugo *« des itérations qui se voient un peu plus »*. Doctrine respectée : angle strict ventre/cortisol, **un seul élément visible changé** par itération, corps du winner conservé (à corriger en 90 % de silymarine), disclaimer `Az eredmények egyénenként eltérhetnek.` ajouté partout.

| # | Élément changé | Titre HU (angle) | Visuel | Page |
|---|---|---|---|---|
| **1 — hook « visage »** | Titre + ouverture | *Le premier changement ne se voit pas sur la balance, mais sur le visage* | même dessin 2 silhouettes, vue de face | Dr. Tóth Petra |
| **2 — hook « ashwagandha »** | Titre + ouverture + visuel | *Vous pouvez prendre de l'ashwagandha encore 2 ans, votre cortisol restera élevé* | schéma robinet fermé / lavabo plein / évacuation bouchée « FOIE » | Dr. Tóth Petra |
| **3 — preuve sociale en hook** | Angle d'entrée, format court | *2 184 avis. 4,8 étoiles. La formule dont tout le monde parle.* | flacon officiel + 5 étoiles + « 2 184 avis » + bandeau 2+1 AJÁNDÉK | Hepavix (page marque) — c'est une ad d'offre |

- **It1** vend le premier résultat concret de la timeline (jour 10 : visage dégonflé) plutôt que le mécanisme → preuve précoce pour une audience qui a déjà tout essayé.
- **It2** attaque l'échec de la solution que la lectrice a déjà essayée (persona PRODUCT AWARE, la moitié prend des adaptogènes) — c'est le passage le plus fort du corps du winner, jamais utilisé en hook.
- **It3** concrétise l'idée notée dans [04-angles-personas.md § Territoires jamais explorés](04-angles-personas.md#territoires-jamais-explorés) — la preuve sociale en ouverture d'ad plutôt qu'en fin de texte, avec nos vrais chiffres (2 184 / 4,8), jamais ceux du concurrent.
- **Bonus non rédigé** : une adaptation du mécanisme de promo « We Made Too Much » de Ritual Labs — ce n'est pas une itération du winner, gardé à part.

> Les copies HU complètes + leur traduction FR n'ont pas encore été posées sur Notion : elles attendent le choix d'Hugo sur laquelle(s) lancer.

## Production natives en cours (19-22/08) — statut détaillé

### Batch « 19/08/2026 — Ads » — itérations du winner [Ads 2](ads/cortisol-winner.md), framework awareness
- **7 copies écrites, posées et validées sur Notion** : #0 winner verbatim · V1 hook constat quotidien (« le 10e jour ») · V2 correction de croyance (ashwagandha) · V3 condensée · V4 révélation d'initié (Éva) · V5 listicle · V6 mécanisme nommé (« 2e métier du foie »).
- **Hooks refaits le 21/08** (correction Hugo : un hook de native = le persona se reconnaît en 1 phrase, jamais une mise en scène narrative longue) sur les 6 itérations, corps inchangés.
- **Visuels** : NATIVE 3/4/5 livrés et importés Notion (7/7 chacun) ; NATIVE 6 à 4/7 (attend 3 photos style B d'Hugo) ; NATIVE 1 (winner verbatim) et NATIVE 7 (mécanisme nommé) restent à produire.

### Batch [Ads 12](ads/statines-airbnb.md) « Anna, l'hôtesse Airbnb » — CLOS à 3 fiches
- Lancé le 20/08 sur un cadre de 6 itérations, **tranché à 3 fiches le 21/08** (2 ventes historiques = pas un winner confirmé) : #0 winner corrigé · V1 « caméra 5h22 » · V2 photo — chacune avec **5 briefs visuels** (règle : 7 pour un winner, 5 pour une non-winner). Les V3-V5 prévues ne seront pas créées.
- Corrections systématiques appliquées à toutes les itérations : dosage aligné sur 2 gélules/j, karácsony (au lieu de Thanksgiving), registre magázó, disclaimer ajouté, ~10 mots hongrois cassés réparés — cohérent avec les défauts déjà documentés en [03-compliance.md](03-compliance.md).
- Visuels de ce batch : **GPT Image 2 pour tout** (y compris les scènes sans personnage — règle actée le 21/08, à la différence du batch Ads 2 qui reste en illustré NB Pro) : context natives + before/after (autorisé à ce niveau solution aware).

### Itérations des natives du concurrent Ritual Labs — PHASE 1 terminée
- **6 ads concurrentes clonées et adaptées** au marché HU, 7 fiches au total (le #3 partage la copy de #1) — détail par ad → [02-concurrent.md](02-concurrent.md).
- **PHASE 2 lancée et validée le 22/08** : 30 briefs visuels (5 par fiche, tableau au modèle Ads 12 : ID · Type de native · Awareness · Modèle · Description · Textes HU · Pourquoi) posés sur Notion. Règle du brief n°1 : recréation quasi identique et localisée HU du visuel concurrent source ; les 4 autres déclinent les beats du récit. Génération des images (GPT Image 2, 30 au total) prévue dans une conversation dédiée, dossiers `visuels/statics-ritualN-…`.
- **✅ PHASE 3 FAITE (24/08)** : les 2 pages Facebook persona sont créées (Kovács Éva / Nagy István, bios neutres) et le routing final des 12 pages Notion du batch a été audité puis figé → détail [01-brand.md § Pages Facebook](01-brand.md#pages-facebook). Reste : warm-up organique + partage BM avant mise en ads.
- **Nouveau format de fiche Notion** (acté le 22/08, généralisé rétroactivement sur les 24 pages du batch) : en-tête 5 lignes **🎯 PERSONA · 📐 ANGLE · 🧠 AWARENESS · 🖼️ TYPE DE VISUEL · 🪝 TYPE DE HOOK**, chacune expliquée en mots simples entre parenthèses ; changements vs concurrent marqués en rouge dans le FR itéré ; traduction FR du concurrent ajoutée en dessous pour comparaison directe.

### 🔴 Décision 22/08 : scaler AGRESSIVEMENT pendant les 30 jours de préavis pixel
- Pixel en pending, préavis 30 jours (2e fois) avant coupure si la review ne passe pas (cf. doctrine domaine flaggé, [10-operations.md](10-operations.md)).
- **Décision actée avec les associés** : plutôt que freiner, **doubler le budget** dès le 22/08 au soir puis augmenter quasi quotidiennement — quitte à retomber à zéro (re-phase d'apprentissage pixel) si la review échoue ; l'ad account garde l'historique acquis pour la relance suivante.
- Munitions : ~50 natives complètes produites pour alimenter ce scaling. Stock ~10 000 unités, jugé large pour 25-30 jours à ce rythme.
- Piste évoquée mais **non retenue** (cloaking d'une LP édulcorée pour les bots Meta) — risque de ban définitif si détecté, gardée pour mémoire uniquement.

## Rappels avant de produire

- Relire [03-compliance.md](03-compliance.md) : le 90 %, le disclaimer, les refus Meta (titre dramatique + verre d'alcool).
- Garantie = **60 jours** (pas 90).
- Offre : 12 400 / 20 900 (2+1) / 27 900 Ft — jamais les $ du concurrent.
- Preuve sociale : 4,8/5 · **2 184** avis (jamais le 34 423 du concurrent).

## Avant de scaler — anti-rejet Meta (MAJ 2026-07-15)

Retour d'expérience d'un call groupe (14/07/2026) sur un scénario vécu par une autre brand santé : les ads passent la review au testing petit budget, puis Meta les re-contrôle dès que le spend monte et les rejette. Ce portefeuille (claims santé, récits façon médecin) est exposé au même profil de risque.

Mécanismes de protection à mettre en place, par ordre :

1. **Post ID organique** : publier la créa en post organique sur la page persona (ou la lancer en objectif interactions), puis créer l'ad de conversion en reprenant ce post ID existant. Review plus légère, pas de re-review de créa à chaque duplication au scale, preuve sociale cumulée sur un seul post. → à la relance : publier Ads 2 en organique quelques jours avant de la relancer en ads.
2. **Sous-domaine tampon clean** : créer un sous-domaine 100 % clean (zéro claim santé, zéro mot flaggé) qui redirige vers l'advertorial — le robot Meta classe le domaine à partir de ce qu'il crawle. Rester sur une page tampon réellement clean et cohérente : un cloaking pur (page robot ≠ page utilisateur) aggrave la sanction si détecté.
3. **Agency ad account** : compte agence whitelisted, tolérance et limites plus hautes (piste non détaillée).

Rappel structurel : la data diffère entre comptes pub — ne jamais conclure qu'une ad est morte sur un seul compte ; garder le pixel, tester l'offre dans une nouvelle campagne (même compte), sur au moins une semaine avant de trancher.

## ⚠️ Page persona partagée avec une autre brand du portefeuille (MAJ 2026-07-15)

La page **« Dr. Tóth Petra Menopauza szakértő »** porte le winner absolu d'Hepavix (Ads 2 — 36 ventes sur 41, ROAS 9,33) et diffuse aussi des ads d'une autre brand du portefeuille (bague + bracelet, angle ménopause). **Risque** : si l'autre brand se fait flaguer par Meta, on perd la page qui porte le meilleur winner du portefeuille entier. **Action recommandée avant relance** : séparer les deux — une page ménopause dédiée à l'autre brand, « Dr. Tóth Petra » réservée à Hepavix.

---

*Navigation : [← 06 — Résultats](06-resultats.md) · [08 — Brand system →](08-brand-system.md)*
