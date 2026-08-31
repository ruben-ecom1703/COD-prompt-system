# 02 — Le concurrent cloné : Ritual Labs / Happy Liver

> 📅 Dernière mise à jour : 2026-08-24 · Gérant : Hugo

**Ce que contient ce fichier :**
- Le profil du concurrent dont Hepavix est le clone
- Ce qu'on a copié et ce qu'on a volontairement changé
- La veille datée (ce qu'ils font en ce moment)
- Leurs visuels d'ads, archivés dans le repo

**Sommaire** : [Profil](#profil) · [Ce quon a copié et ce quon a changé](#ce-quon-a-copié-et-ce-quon-a-changé) · [Leurs visuels dads](#leurs-visuels-dads) · [Veille datée](#veille-datée)

---

## Profil

| | |
|---|---|
| **Brand** | Ritual Labs — produit « **Happy Liver** » |
| **URL** | https://rituallabs.shop/products/happy-liver |
| **Marché** | US (anglophone) |
| **Trafic** | **98 669 visites/mois** (relevé Brandsearch le 14/07/2026) |
| **Ads Meta actives** | **108** (relevé le 14/07) |
| **Prix** | $34.99 · B2G1 $69.99 · B3G2 $104.98 — ⚠️ **jamais utiliser ces prix**, on est en Ft ([01-brand.md](01-brand.md#offre)) |

**Hepavix = clone fidèle** : même produit (complément foie, gélules), même formule à 3 ingrédients (silymarine + NAC + choline), même architecture de page, mêmes mécanismes narratifs. La doctrine : **traduire et adapter, pas réinventer.**

## Ce qu'on a copié et ce qu'on a changé

| Élément | Concurrent | Nous |
|---|---|---|
| Formule | Silymarine + NAC + choline | ✅ Identique |
| Mécanisme narratif | Foie surchargé → un symptôme qui ne se résout pas par la voie évidente → les 3 ingrédients débloquent l'organe | ✅ Identique — c'est le cœur de ce qui vend |
| Prix | $ (abonnement/packs US) | ❌ **Ft** : 12 400 / 20 900 / 27 900 |
| Garantie | (leur durée) | ❌ **60 jours** chez nous |
| Preuve sociale | 34 423 avis | ❌ **2 184 avis · 4,8/5** chez nous |
| Silymarine | (leur %) | ❌ **90 %** chez nous — [règle absolue](03-compliance.md#la-règle-du-90--silymarine) |
| Paiement | Carte | ❌ **utánvét** (paiement à la livraison) — l'argument n°1 en Hongrie |
| Flacon | Happy Liver (blanc/bleu pâle) | ❌ Rebrandé **HEPAVIX** (flacon blanc) — voir [assets/](assets/) |

**Le « mécanisme profond » commun à toutes leurs ads gagnantes** (et aux nôtres) : le foie est l'organe qui traite tout, il prend du retard, et **le symptôme visible (ventre, cholestérol, fatigue, gueule de bois) n'est que la conséquence.** On ne vend pas un complément foie : on vend **la vraie cause d'un symptôme qui ne part pas**.

## Leurs visuels d'ads

8 visuels de leurs ads sont archivés dans [visuels/concurrent/](visuels/concurrent/) — utiles pour comprendre leur grammaire visuelle et pour cloner un angle :

| Fichier | Angle |
|---|---|
| `apron-belly-fupa.jpg` · `apron-fupa-9x16-papier.jpg` | Le ventre en tablier (= la source du visuel de **notre winner**) |
| `no-more-statin.jpg` · `lost-my-206-ldl.jpg` | Cholestérol / statines |
| `dont-stop-drinking.jpg` · `drink-all-you-want.jpg` · `drinkers-liver-evolution.jpg` | Alcool / detox |
| `liver-overworked.jpg` | Le foie surchargé (mécanisme) |

## Itérations clonées — batch natives concurrent (19-22/08, PHASE 1 terminée)

Flux de production : classification de l'ad source (awareness + type de hook + type de visuel) → validation Hugo → itération swap-brand (Ritual Labs → Hepavix) → vérification externe hongroise → fiche Notion sous « 19/08/2026 — Ads ». **6 ads sources clonées, 7 fiches** (le #3 partage la copy exacte du #1, cf. ci-dessous) :

| # | Ad source (ID Meta) | Page concurrent | Classification | Page Hepavix routée | Adaptations clés |
|---|---|---|---|---|---|
| #1 | `1258849389464277` (actif depuis 16/06) | David Hudgens (homme, expert) | Problem aware · correction de croyance + mécanisme nommé (acétaldéhyde) · before/after natif (2 foies WEEK 0/6) | Nagy István (à créer) | Happy Liver→Hepavix · 80 %→90 % · bourbon→pálinka · disclaimer ajouté |
| #2 | `1319040523689609` (actif depuis 17/06) | Jessica Smith (femme, lambda) | Problem→solution aware · aveu personnel · product native UGC (femme + flacon) | Kovács Éva | inositol→kolin (le rôle décrit correspond réellement à la choline) · 90 % · lbs→kg |
| #3 (jumelle de #1) | `955626090856428` (actif depuis 16/06) | Vivienne Ashcombe (femme, médicale) — copy identique mot pour mot à #1 | Idem #1 | Dr. Tóth Petra | copy recopiée à l'identique (le concurrent scale sa copy winner tel quel) ; visuel prévu = concept marqueur-joue, bouteille visible = retest alcool assumé |
| #4 | `1713495923007334` (actif depuis 21/06) | Jessica Smith (3e copy différente sur la même page) | Solution aware saturée → problem aware sur 2 problèmes neufs (cycle de rupture cellulaire ALT, silymarine dégradée) · méga-advertorial (19 700 caractères) | Kovács Éva | offre concurrent « Buy 2 get 1 free »→notre 2+1 réel · noms localisés (Éva/Margit/Dr. Szabó) · 90 % |
| #5 | `1966846090616333` | — | Problem aware · pattern interrupt pro-alcool → pivot enzymes (acétaldéhyde ×30, glutathion chronique) | Dr. Tóth Petra | pas de garantie/scarcité (fidélité au close du concurrent) · Tylenol→fájdalomcsillapító |
| #6 | `1786685415850177` | — | Solution→product aware · avatar selfie « after » · hook protocole documenté (ALT 132→28) | Kovács Éva | inositol→kolin · 90 % · pas de garantie/scarcité |

⚠️ **Retests alcool assumés** (compteur refus historique : 1, Ad #16) : le concept marqueur-joue avec bouteille visible (fiche #3) et un brief dîner avec verres de vin (fiche #5) — des versions de repli sans bouteille sont déjà briefées en cas de flag Meta.

**Vérification externe systématique** (2e conversation dédiée) sur chaque itération hongroise avant mise en fiche — le type d'erreur dominant n'est jamais l'orthographe de base mais les **calques idiomatiques anglais** (tournures littérales mal transposées) et les **rections de verbes (vonzat)** propres au hongrois.

**PHASE 2 (visuels)** : 30 briefs posés (5 par fiche, tableau standardisé) — détail du flux → [07-relance.md](07-relance.md). Dossiers prévus dans [visuels/](visuels/README.md) : `statics-ritualN-…` (génération encore en cours au 22/08, pas encore livrés — non listés à ce jour dans le dossier).

**PHASE 3 FAITE (24/08)** : les 2 pages Facebook persona (Kovács Éva / Nagy István) sont créées, bios neutres, routing final audité et figé → [01-brand.md § Pages Facebook](01-brand.md#pages-facebook).

## Veille datée

> Refresh à faire ~1×/mois (Brandsearch sur `rituallabs.shop`). Chaque relevé = une nouvelle sous-section datée.

### Relevé du 2026-07-14

- **108 ads Meta actives**, 98 669 visites/mois. La marque tourne toujours à plein régime → le produit et l'offre restent valides.
- **Leur ad la plus récente (23/06/2026)** : une **promo BOGO** — headline « **We Made Too Much Happy Liver 😬** », copy « BUY 2 GET 1 FREE — TIME TO GIVE YOUR LIVER A REAL SHOT ». Angle « surproduction / stock en trop » pour justifier la promo. Les symptômes listés en tête sont exactement les nôtres : *the stubborn belly, the 2 PM crash, the brain fog, the climbing cholesterol numbers*.
  → **Réutilisable** : c'est un mécanisme de promo (« on en a fabriqué trop ») qu'on n'a jamais testé et qui s'adapte directement à notre 2+1 ajándék.
- Rien d'autre de radicalement neuf détecté sur ce relevé — leur socle reste les advertorials longs (ventre/cortisol, statines, alcool).

### Relevé du 2026-08-06

- **Échelle mise à jour (Brandsearch)** : page « Ritual Labs Happy Liver » = **219 ads au total, 147 actives**, créée nov. 2025, 6 054 likes.
- **Stratégie de page confirmée : une seule page marque porte quasi toutes les ads actives.** Une page secondaire « Jennifer Hudgens » testée en persona n'a produit qu'1 ad, jamais activée — le test persona a été abandonné côté concurrent.
  → **Lecture pour nous** : le concurrent gagne sur la page marque seule, à l'inverse de notre stratégie pages persona/médecin (Dr. Tóth Petra, Varga Nóra). Pas une raison de tout changer (nos pages persona restent nos meilleures perf à date), mais un signal à garder si un test page-marque-only est un jour envisagé.

---

*Navigation : [← 01 — Brand](01-brand.md) · [03 — Compliance →](03-compliance.md)*
