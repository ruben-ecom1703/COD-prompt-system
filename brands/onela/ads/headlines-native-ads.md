# Headlines & sub-headlines — Native Ads Onela

---

# ⚡ PACK DE DÉPLOIEMENT (copier-coller) — v3, 2026-08-07

**Domaine affiché :** `ONELA.SHOP` — **CTA :** `Vásárlás`

**Sub-headline HU — IDENTIQUE sur les 16 :**
```
Természetes étrend-kiegészítő, amely az emésztőrendszerben semlegesíti a kénvegyületeket. Onnan, ahonnan a szag valójában ered. Eredmények…
```
> FR : « Complément alimentaire naturel qui neutralise les composés soufrés dans le système digestif. Là d'où l'odeur vient vraiment. Résultats… »

**Les 3 headlines HU :**

| Code | Hongrois | FR |
|---|---|---|
| **H1** | `Nem a szájában kezdődik.` | Ce n'est pas votre bouche. / Ça ne commence pas dans votre bouche. |
| **H2** | `Rossz helyet tisztít.` | Vous nettoyez au mauvais endroit. |
| **H3** | `A szájszag nem normális.` | La mauvaise haleine n'est pas normale. |

> Arbitrages à faire trancher par le natif :
> - H2 : `Rossz helyen keresi.` ("vous cherchez au mauvais endroit") est plus idiomatique que `tisztít`, mais perd le verbe "nettoyer".
> - H3 : `szájszag` = mot courant/mass market · `rossz lehelet` = mot propre. `szájszag` frappe plus fort.
> - ⚠ H3 est en formulation **générale** (`A szájszag…`), jamais possessive — voir § Policy Meta plus bas.

## Affectation headline × script — compatibilité (meilleure en premier)

**H1 passe sur les 16.** Solution zéro-réflexion : la coller partout. Le tableau donne les alternatives pour affiner.

| # | Script | Headlines qui passent |
|---|---|---|
| 1 | Caséum × F1 — "J'ai arrêté de gratter" | **H2** · H1 |
| 2 | Caséum × F4 — "Le dentiste qui a changé d'avis" | **H1** · H2 |
| 3 | Caséum × F2 — "Mon copain dort dos à moi" | **H3** · H1 |
| 4 | Reflux × F3 — "Le gastro-entérologue" | **H1** · H2 · H3 |
| 5 | Reflux × F1 — "J'ai tout arrêté" | **H2** · H1 |
| 6 | Reflux × F4 — "Le médecin qui n'a jamais posé la question" | **H1** · H3 · H2 |
| 7 | Langue blanche × F5 — "2 heures" | **H2** · H1 · H3 |
| 8 | Langue blanche × F3 — "L'hygiéniste dentaire" | **H2** · H1 |
| 9 | Langue blanche × F4 — "La pharmacienne qui vend des gratte-langues" | **H2** · H1 |
| 10 | Fumeur × F2 — "C'est pas la cigarette" | **H3** · H1 |
| 11 | Fumeur × F1 — "Le test des 24 heures" | **H1** · H3 |
| 12 | Fumeur × F4 — "Le pharmacien qui fume" | **H1** · H3 |
| 13 | Dating × F2 — "Première date, dernière date" | **H3** · H1 |
| 14 | Dating × F5 — "Chaque mec, même scénario" | **H3** · H1 |
| 15 | Haleine du matin × F1 — "Le test de la brosse du soir" | **H2** · H3 · H1 |
| 16 | Haleine du matin × F4 — "Le dentiste qui se lève avant sa femme" | **H1** · H3 · H2 |

**Les 5 scripts où les 3 passent :** #4, #6, #7, #15, #16.

### Mode "3 copier-coller" (workflow de saisie)

| Copie | Headline | Scripts |
|---|---|---|
| 1 | `Rossz helyet tisztít.` (H2) | 1, 5, 7, 8, 9, 15 |
| 2 | `A szájszag nem normális.` (H3) | 3, 10, 13, 14 |
| 3 | `Nem a szájában kezdődik.` (H1) | 2, 4, 6, 11, 12, 16 |
| — | Sub-headline HU | les 16 |

### Les 2 règles bloquantes

- **H2 INTERDITE sur #10, #11, #12 (Fumeur) et #13, #14 (Dating).** Le lecteur n'y nettoie rien — il fume ou il rate ses dates. La headline promet un contenu qui n'arrive jamais : on paye le clic et on perd la vente.
- **H3 faible sur #1, #2, #5, #8, #9.** Elle passe mais ces scripts n'ont pas de moment "on m'a dit que c'était normal". Fallback acceptable, pas une erreur.
- **H1 sans contre-indication** — valeur par défaut sur n'importe quel script, y compris les futurs (Ménopause, Odeurs alimentaires).

**Logique de l'affectation par défaut :**
- **H2** → uniquement les scripts où le héros **fait un geste de nettoyage inutile** (gratter, gratte-langue, brossage du soir, langue qui reblanchit). Le titre est la conclusion littérale du script. **Zéro H2 sur Fumeur et Dating** — le lecteur n'y nettoie rien.
- **H3** → les 4 scripts en **F2 gaslighting / F5 cycle**, où l'entourage dit "c'est normal, c'est dans ta tête, tu fumes forcément que ça sent". Le titre casse le "c'est normal" avant le clic.
- **H1** → tout le reste : les 7 scripts d'**autorité et d'insider** (dentiste, gastro, généraliste, hygiéniste, pharmacien) + le test 24h. Titre neutre et universel, il porte les créas les plus fortes (#12 et #16, les 10/10).

**Alternative plus propre statistiquement :** H1 sur les 16 au round 1 (isole la variable script), H2/H3 ressortis au round 2 sur les gagnants. Le tableau ci-dessus est la version optimisée pour qui veut démarrer calé.

---


> Bloc link preview Facebook (domaine affiché / headline / description / bouton CTA).
> Compatible avec les 16 scripts de `scripts-native-ads.md`.
> Date : 2026-08-07

---

## Modèle décortiqué — Lynae (lynae.co)

```
LYNAE.CO
C'est pas dans votre tête.                                    [ Acheter ]
Complément naturel pour réduire la rétention d'eau, dégonfler
durablement et relancer le drainage lymphatique. Résultats…
```

**Pourquoi ça marche :**

1. **Headline** — 5 mots, une négation, un point final. Ne vend rien, ne promet rien, ne nomme pas le produit. Elle **valide** le lecteur ("t'es pas fou"). Ouverture d'article, pas de pub.
2. **Sub-headline** — 100 % descriptive, ton notice de complément. Catégorie + mécanismes en verbes. Zéro émotion, zéro "découvrez", zéro chiffre. Le contraste headline émotionnelle / sub plate = signal "lien d'article".
3. **Le "Résultats…" tronqué** — Facebook coupe la description à ~2 lignes. La phrase est écrite pour que la coupe tombe sur un mot ouvert → boucle ouverte gratuite.

---

## Setup Onela — recommandé

```
ONELA.SHOP
Ce n'est pas votre bouche.                                    [ Acheter ]
Complément naturel à base de chlorophylle pour neutraliser les
composés soufrés dans le système digestif, là où l'odeur se
forme. Premiers résultats…
```

**Headline :** `Ce n'est pas votre bouche.`

Jumeau structurel exact de "C'est pas dans votre tête." — négation + déplacement du problème. Et c'est **littéralement la thèse des 16 scripts** : caséum, reflux, langue blanche, fumeur, dating, haleine du matin — tous retournent sur "le problème est dans l'estomac, la bouche c'est juste où tu le vois". Un seul headline couvre les 6 angles sans mentir sur le contenu derrière.

**Sub-headline retenue (v2, 2026-08-07) :** « Complément alimentaire naturel qui neutralise les composés soufrés dans le système digestif. Là d'où l'odeur vient vraiment. Résultats… »

**Domaine affiché :** ONELA.SHOP — **CTA :** Acheter

### Sub-headlines FR — variantes notées

| # | Sub-headline | Note |
|---|---|---|
| **A** ⭐ | Complément alimentaire naturel qui neutralise les composés soufrés dans le système digestif. Là d'où l'odeur vient vraiment. Résultats… | 9.5/10 |
| B | Complément alimentaire naturel pour retrouver une haleine fraîche en neutralisant les composés soufrés dans le système digestif. Résultats… | 9/10 |
| C | Complément alimentaire naturel qui agit sur les composés soufrés produits par la flore digestive, pas sur la bouche. Résultats… | 8.5/10 |

- **A** — même longueur que Lynae, la troncature FB tombe pile après le payoff. Deux phrases courtes = ton notice.
- **B** — garde le bénéfice explicite ("retrouver une haleine fraîche"). Plus vendeuse, un cran moins "article", parfaitement safe.
- **C** — la plus mécanique mais redondante avec la headline "Ce n'est pas votre bouche."

---

## Rotation headlines

| Headline | Pourquoi ça marche | Note |
|---|---|---|
| **Ce n'est pas votre bouche.** | ⭐ le pick — couvre les 16 | 9.5/10 |
| Vous nettoyez au mauvais endroit. | même retournement, plus actif — **⚠ ne colle PAS aux scripts #10-12 Fumeur ni #13-14 Dating** (le lecteur n'y "nettoie" pas). Réserver aux 12 autres. | 9/10 |
| La mauvaise haleine n'est pas normale. | retournement de croyance, formulation générale (voir § policy Meta) | 9/10 |
| Ça revient en 2 heures. | pure observation, zéro promesse | 9/10 |
| Le brossage ne suffit pas. | frustration partagée, très neutre | 8.5/10 |
| Ça ne vient pas de là. | le plus vague, le plus "article" | 8.5/10 |

### ⚠ Policy Meta — Attributs personnels

**Ne jamais écrire `Votre mauvaise haleine ...`** — la politique "Attributs personnels" interdit d'affirmer ou de sous-entendre qu'on connaît l'état de santé du lecteur. Le possessif transforme la phrase en affirmation directe → motif de refus classique sur les compléments, et à répétition ça tape le compte pub.

- ❌ `Votre mauvaise haleine n'est pas normale.`
- ✅ `La mauvaise haleine n'est pas normale.` / `La mauvaise haleine n'est pas une fatalité.`

Les headlines en négation pure (`Ce n'est pas votre bouche.`) passent parce qu'elles n'affirment rien sur le lecteur.

---

## Combien de headlines par pub — stratégie de test

Meta accepte jusqu'à **5 titres / 5 textes principaux / 5 descriptions** par pub ("plusieurs versions de texte"). **À ne PAS utiliser au round 1.**

Raison : Meta mélange les combinaisons et optimise, mais le reporting par combinaison est inexploitable. Avec 16 scripts × 4 headlines = 64 combinaisons pour ~20 achats de data → impossible de savoir si un script gagne par sa qualité ou par la headline qu'il a reçue. La contrainte réelle est le **volume de data**, pas le nombre de créas.

| Round | Objectif | Setup |
|---|---|---|
| **1** | Tester les 16 scripts | **1 seule headline, la même sur les 16.** Sortir 2-3 scripts gagnants. |
| **2** | Tester les headlines | Les 2-3 scripts gagnants dupliqués en **pubs séparées**, 1 headline par pub. Data propre. |
| **Scaling** | Gratter du CPM | Là oui : 4 headlines gagnantes en "plusieurs versions de texte". On n'apprend plus, on laisse Meta optimiser. |

---

## Headlines par angle (même sub-headline pour les 6)

| Angle | Scripts | Headline |
|---|---|---|
| 1 — Caséum | #1 #2 #3 | Le grattage ne sert à rien. |
| 2 — Reflux silencieux | #4 #5 #6 | Vous ne sentez rien remonter. |
| 3 — Langue blanche | #7 #8 #9 | Elle redevient blanche en 2h. |
| 4 — Fumeur | #10 #11 #12 | Ce n'est pas la cigarette. |
| 5 — Dating / intimité | #13 #14 | Il ne vous le dira pas. |
| 7 — Haleine du matin | #15 #16 | Ça revient pendant la nuit. |

---

## Version hongroise (déploiement) — 5 variantes notées

**CTA :** Vásárlás — **Domaine affiché :** ONELA.SHOP

### Headlines

| # | Hongrois | Traduction FR | Note |
|---|---|---|---|
| V1 | `Nem a szája a probléma.` | "Votre bouche n'est pas le problème." | 9/10 |
| V2 | `Nem a szájában kezdődik.` | "Ça ne commence pas dans votre bouche." | **9.5/10** |
| V3 | `Hiába mos fogat.` | "Vous avez beau vous brosser les dents." | **9.5/10** |
| V4 | `Nem ott van a baj.` | "Le problème n'est pas là." | 8.5/10 |
| V5 | `Nem a szájával van baj.` | "Ce n'est pas votre bouche qui pose problème." | 9/10 |

- **V1** — le plus proche du FR, négation propre et claire. Bémol : `probléma` est un mot un peu abstrait/marketing.
- **V2** ⭐ — la notion d'**origine** est explicite (`kezdődik` = ça commence). Annonce le retournement des scripts sans rien promettre. La plus "article".
- **V3** ⭐ — `hiába` (= "en vain / vous avez beau") est une tournure intraduisible et 100 % native : zéro odeur de traduction, la plus forte émotionnellement. Bémol : moins universelle sur les angles Fumeur et Dating.
- **V4** — la plus vague donc la plus "blog", mais peut-être trop floue pour accrocher.
- **V5** — registre parlé, très naturel. Un peu plus longue visuellement.

### Sub-headlines

**Sub A ⭐ 9.5/10** — la plus mécanique, colle au fil rouge des 16
`Természetes étrend-kiegészítő, amely a kénvegyületeket az emésztőrendszerben semlegesíti – ott, ahol a szag keletkezik. Az első eredmények…`
> "Complément alimentaire naturel qui neutralise les composés soufrés dans le système digestif — là où l'odeur se forme. Les premiers résultats…"

**Sub B — 9/10** — calque exact de la structure Lynae (3 mécanismes en verbes)
`Természetes étrend-kiegészítő a kénvegyületek semlegesítésére, a bélflóra egyensúlyának helyreállítására és a szagok forrásának kezelésére. Eredmények…`
> "Complément alimentaire naturel pour neutraliser les composés soufrés, rétablir l'équilibre de la flore intestinale et traiter la source des odeurs. Résultats…"

**Sub C — 8.5/10** — trop redondante avec la headline
`Klorofillt tartalmazó étrend-kiegészítő. Az emésztőrendszerben ható hatóanyagok, nem a szájban. Az első eredmények…`
> "Complément alimentaire contenant de la chlorophylle. Des actifs qui agissent dans le système digestif, pas dans la bouche. Les premiers résultats…"

### Combo recommandé — ROUND 1

```
ONELA.SHOP
Nem a szájában kezdődik.                                     [ Vásárlás ]
Természetes étrend-kiegészítő, amely a kénvegyületeket az
emésztőrendszerben semlegesíti. Onnan, ahonnan a szag
valójában ered. Eredmények…
```

> Équivalent FR : « Ce n'est pas votre bouche. » + Sub A.
> Réserve round 2 : `Vous nettoyez au mauvais endroit.` (12 scripts /16) et `La mauvaise haleine n'est pas normale.`

### Glossaire de vérification

| HU | FR |
|---|---|
| szag | odeur |
| kénvegyület | composé soufré |
| emésztőrendszer | système digestif |
| étrend-kiegészítő | complément alimentaire |
| klorofill | chlorophylle |
| bélflóra | flore intestinale |
| hiába | en vain / avoir beau |
| baj | problème (familier) |
| kezdődik | ça commence |
| eredmények | résultats |

> ⚠️ À faire relire par un natif avant launch — la négation hongroise a plusieurs tournures possibles, il ne faut pas que ça sonne traduit.

---

## Les 5 règles à ne pas casser

1. **Jamais le nom du produit dans le headline** — signal n°1 "c'est une pub".
2. **Jamais de chiffre, de %, de point d'exclamation, de majuscules** dans le headline.
3. **Le même headline sur les 16 au premier round** — sinon deux variables testées en même temps, impossible de savoir si c'est le script ou la headline qui performe.
4. **Sub-headline toujours ennuyeuse.** Si elle devient vendeuse, tout l'effet tombe.
5. **Ne pas utiliser "C'est pas dans votre tête"** tel quel — headline actif de Lynae, même plateforme, risque de se faire absorber par leur créa.
