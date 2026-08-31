---
date: 2026-08-10
type: audit-performance
sources:
  - CLN_0428-KN-3---Nomadsla-s-Ads-11-Jul-2026-9-Aug-2026.csv (export Meta interne, 11/07 → 09/08)
  - 7 screenshots Meta Ad Library (filtre "nomadlabs.shop", statut Actives, tri spend décroissant, CPM custom 9€)
  - toute la data interne du dossier Nomad Labs (scripts, briefs, audits 22/07 et 30/07)
---

# Audit performance Nomad Labs — 11 juillet → 9 août 2026

Premier point complet depuis l'audit bibliothèque du 30/07. Croisement de trois sources : l'export Meta interne (vérité sur le spend et les achats), la bibliothèque publicitaire (vérité sur *quel* créa tourne et son poids relatif), et le corpus de scripts du vault (vérité sur *quel* angle/framework est derrière).

## 1. Chiffres globaux (29 jours)

| Métrique | Valeur |
|---|---|
| Spend | **$14 814,77** |
| Achats | **1 745** |
| CPA moyen | **$8,49** |
| ROAS reporté | **11,66x** (revenu déclaré ~$172 700) |
| AOV implicite | ~$99 → cohérent avec un mix 29 900 Ft (2+1) / 49 900 Ft (3+3) |
| Ads ayant tourné | 168 (avec spend > 0) |
| Ads à 0 achat | 110 sur 168 — mais **seulement $271 de spend cumulé** |

**Lecture :** le rythme est passé de $4 352 sur les 20 premiers jours de juillet (audit du 20/07) à ~$14 800 sur 29 jours, soit **~$510/jour** contre ~$218/jour. On a plus que doublé le rythme de dépense en gardant un CPA stable ($6,59 → $8,49 ; la dégradation est réelle mais modérée pour un x2,3 de budget).

⚠️ **ROAS à lire en COD** : 11,66x est du revenu commandé, pas encaissé. À taux de livraison 65-70 %, le ROAS net réel est de l'ordre de **7,5-8x**. Les 110 ads à 0 achat ne sont pas un problème : $271 de gaspillage total, la méthode de test large + kill rapide fonctionne.

## 2. Où part l'argent

| Bloc | Spend | Part | CPA | ROAS |
|---|---|---|---|---|
| Adsets de scale legacy (Adset 1 → 5 BOF) | $8 558,93 | 58 % | $8,57 | 11,65x |
| Batchs de test datés (16/07 → 08/08) | $5 746,86 | 39 % | $8,43 | 11,65x |
| Vidéo (Adset 6 VIDEO + 03/08 video) | $769,44 | **5,2 %** | $8,95 | 10,38x |

Deux constats structurels :

1. **58 % du budget tourne sur 4 slots créa dans les adsets legacy**, et d'après le mapping du 22/07 ces 4 slots ne représentent que **2 scripts** — László/Voisine (ads 2, 3, 4) et Chauffeur Bolt (ads 1). Autrement dit : la majorité du business repose encore sur deux native ads écrites le 12 juin.
2. **La vidéo pèse 5,2 % du spend** alors que 13 briefs vidéo ont été produits (5 le 29/07, 5 le 09/08 sur framework 7 blocs, + les 3 VSL László). Le goulot n'est pas la production de scripts, c'est la mise en ligne.

### Détail des 4 slots legacy

| Slot | Script (mapping 22/07) | Spend | Achats | CPA | ROAS |
|---|---|---|---|---|---|
| ads 3 | László / Voisine | **$4 447,50** | 510 | $8,72 | 11,71x |
| ads 4 | László / Voisine | $1 825,46 | 248 | **$7,36** | **13,37x** |
| ads 1 | Chauffeur Bolt | $1 402,83 | 168 | $8,35 | 11,80x |
| ads 2 | László / Voisine | $1 316,95 | 127 | **$10,37** | 8,99x |
| ads 5 | Chauffeur Bolt | $72,99 | 10 | $7,30 | 13,02x |

- **ads 3 = 30 % du spend total de la période à lui seul.** C'est le pilier absolu du compte.
- **ads 4 est le meilleur ratio du compte à volume** ($7,36 CPA / 13,37x) et n'a que 41 % du budget de ads 3 → premier levier de scale évident, avant toute nouvelle créa.
- **ads 2 est le maillon faible du bloc legacy** ($10,37, 8,99x) : 1 316 $ à CPA +22 % vs la moyenne. À couper ou à remplacer par un duplicata de ads 4.
- Meilleur ratio absolu du compte : **Adset 5 BOF / ads 4** — $833,97, 146 achats, **CPA $5,71, ROAS 16,81x**. Le BOF est nettement plus rentable que le TOF et est sous-financé.

### Courbe des batchs de test — le signal important

| Période de lancement | Spend | Achats | CPA | ROAS |
|---|---|---|---|---|
| 16/07 → 25/07 | $2 226,49 | 323 | **$6,89** | **14,37x** |
| 29/07 → 08/08 | $3 520,37 | 359 | $9,81 | 9,92x |
| dont 07/08 + 08/08 seuls | $578,85 | 34 | **$17,03** | 5,81x |

**Les batchs de juillet battaient le compte ; les batchs de fin juillet / août le dégradent.** Le CPA des nouveaux tests a été multiplié par 2,5 entre mi-juillet et le 8 août.

Deux explications possibles, non exclusives :
- **Fatigue de mécanisme.** Les batchs 29/07 → 08/08 sont majoritairement des adaptations du corpus concurrent Primitive Labs (Ad 13 à Ad 21), toutes construites sur la même cascade insider → énergie → eau. On empile des variantes de narrateur sur un mécanisme déjà exposé à l'audience depuis deux mois. C'est exactement le risque de diminishing returns noté au 16/07 sur le corpus László, et ça se confirme dans les commentaires ("Ezt már olvastam taxissal is").
- **Lag d'attribution.** Les batchs 07/08 et 08/08 n'ont que 1-2 jours de recul dans un export qui s'arrête le 09/08, sur une fenêtre 7-day click en COD. Leur CPA va mécaniquement s'améliorer.

→ **Ne pas tuer 07/08 et 08/08 maintenant.** Mais le batch 29/07 (CPA $11,26) et le 03/08 vidéo (CPA $11,84) ont assez de recul : ceux-là sont jugés.

### Batchs par ordre de mérite

| Batch | Spend | CPA | Verdict |
|---|---|---|---|
| 24/07 adset 1 | $1 196,38 | **$6,80** | ✅ meilleur batch à volume — seulement 4 ads, très concentré |
| 16/07 adset 1 | $690,70 | **$6,22** | ✅ meilleur CPA de la période |
| 01/08 adset 1 - native | $530,87 | $7,17 | ✅ le seul bon batch d'août (ads 9 : $486 / CPA $7,26 / 15,05x) |
| 31/07 adset 1 - bof/tof | $438,92 | $8,28 | ➖ dans la moyenne |
| 22/07 adset 1 | $178,43 | $7,43 | ➖ correct mais jamais scalé |
| 30/07 adset 1 - native | $956,75 | $8,78 | ➖ moyenne, porté par un seul ad (ads 4 (2) : $836) |
| 29/07 adset 1 - native | $754,52 | $11,26 | ❌ sous la moyenne à volume significatif |
| 03/08 adset 1 - video | $260,46 | $11,84 | ❌ les concepts vidéo hongrois ne tiennent pas le CPA native |
| 08/08 native ads | $327,54 | $16,38 | ⏳ trop récent |
| 07/08 native ads | $251,31 | $17,95 | ⏳ trop récent |
| 17/07, 23/07, 25/07, 18/07 | < $75 chacun | $8,60 → $19,68 | ❌ morts, correctement coupés |

## 3. Mapping bibliothèque Meta → scripts du vault

28 ads actives visibles dans les screenshots (tri spend décroissant, plancher ~€31 — tout ce qui est sous €31 n'est pas couvert). Spend EU = estimation à CPM 9€, à lire en **poids relatif**, pas en montant réel.

### Native ads long-form

| EU spend | Hook (HU) | Script vault | Angle | Statut |
|---|---|---|---|---|
| **€1 070** | "A szomszédom férje múlt hónapban hazajött Budapestről…" | László / Voisine (`ad1`, Créa #2) | #1 Insider géo | 🥇 pilier n°1 |
| €670 | "A férfi, aki két hete a Bolt-om hátsó ülésén ült…" | Chauffeur Bolt (`ad2`, Créa #1) | #1 Insider géo | 🥈 pilier n°2 |
| €523 | idem László (visuel différent : réservoir d'eau jardin) | László / Voisine | #1 | duplicata visuel |
| €468 | idem Bolt (visuel frappe/fumée) | Chauffeur Bolt | #1 | duplicata visuel |
| €384 | idem László (visuel van + moto) | László / Voisine | #1 | duplicata visuel |
| €270 | "Hajnali kettőkor kaptam egy negyvenhat másodperces hangüzenetet a húgomtól…" | [[script-hugom-szerbia]] (`adA`, Ad 7 Cuba/Sister) | #1 + émotion familiale | ⭐ meilleure entrée du batch 2 |
| €203 | "Múlt kedden a sürgősségire behoztak egy hároméves gyereket. Súlyos kiszáradás…" | Éva infirmière (`ad4`) | #1 + autorité médicale | ✅ confirme le early winner |
| €152 | "Négy kamerám van a birtokomon, amikről senki nem tud…" | [[script-kamerak-balaton]] (`adB`, Ad 13) | #1 surveillance inversée | ✅ tient |
| €115 | "Huszonkét éve takarítom egy budapesti minisztérium irodáit…" | Takarítónő (`ad5`) | #2 Eau contaminée | ✅ meilleure ad de l'angle #2 |
| €92 | "Múlt kedden jöttem rá, hogy hat hónapja kézbesítek Szigorúan Titkos katonai csomagokat…" | [[script-csomagok-titkos]] (Ad 16) | #1 | ✅ nouvelle entrée |
| €69 | "Egy helikopter szállt le a szomszéd telekre a tanyám mellett…" | [[script-epulet-ablakok-nelkul]] (Ad 15) | #1 | ✅ nouvelle entrée |
| €68 | "A fiam küldött egy csomagot feladó nélkül… Margit vagyok. 62 éves." | Margit anyuka (`ad6`) | #1 insider familial indirect | ➖ plafonne |
| €44 + €39 | "A béketárgyalások összeomlottak, és hétfő reggel életbe lépett a blokád…" | Tibor (`ad8`, script 2 période d'essai) | #1 variante actualité | ➖ 2 pages, faible |
| €38 | "A vízszámlám megduplázódott márciusban. 4 800 Ft-ról 9 200 Ft-ra…" | Ferenc / facture d'eau (`adH`) | #2 Eau contaminée | ➖ démarre |
| €33 | "Az MIT fúziós központjának igazgatóját… hatszor lőtték meg…" | MIT fúzió / frère enquêteur (`adF`) | #1 conspiration | ➖ démarre |
| €32 | "A vendég, aki múlt kedden szállt meg nálam három éjszakára, készpénzzel fizetett…" | [[script-vendegház-andras]] (Ad 4 Marcus/Inn) | #1 méta-narratif | ➖ démarre |

### Statiques / short copy

| EU spend | Contenu | Rattachement | Note |
|---|---|---|---|
| €195 | "3 SZŰRŐ 2 ÁRÁÉRT" + "Ezt a szűrőt nem egy laborban tervezték turistáknak" | Static "3 szűrő" × Ad Copy A3 (mapping 22/07) + script Origine militaire → civil (§9.6) | ✅ meilleure statique BOF |
| €176 + €80 | "Nincs áram = nincs víz" (vidéo + static) | `ad3` short CTA | ✅ format court qui tient |
| €169 | "Gyorsan fogy a HYDRA-X1 családi készlet" | Créa #3 "MAJDNEM ELFOGYOTT" / `ad7` militaire | ⚠️ voir §5 |
| €67 | "MINDENKINEK, AKIT SZERETSZ" (2+1, -43 %) | Static BOF famille | ➖ |
| €61 | "A csapod normálisan folyik… Mi lenne, ha 6-10 héten belül semmi sem jönne belőle?" + static 400L/17 000 | Ad Copy A1 × static 400L | ➖ |
| €58 | "Három hónap múlva vagy ugyanúgy megtöltöd az unokád poharát a csapnál…" + "MIKROMŰANYAG KISZŰRVE" | Script E "Le verre de ton petit-fils" × static Lynae concept 3 | #2, faible mais l'angle vit |
| €36 | "Több mint 17 000 magyar család bízik már a Hydra X2-ben. 4,7 az 5-ből" + "LIMITÁLT AJÁNLAT 3-at veszel = 3 ingyen" | Static social proof (concept 6 "7 sur 12" dérivé) | ➖ BOF |

### Vidéos

| EU spend | Contenu | Script |
|---|---|---|
| €188 | "Képzeld el: hajnali 2:47-kor robban az első transzformátor…" | **Framework 7 blocs maison** (§7.3) — exécution "Le voisin qui savait", immersion 2ᵉ personne |
| €80 | "Nincs áram = nincs víz" (version vidéo) | `ad3` short CTA |

La vidéo €188 est la mieux classée du format et c'est **notre framework interne, pas un framework concurrent** — cohérent avec le virage stratégique du 09/08.

## 4. Le vrai goulot : le backlog de scripts jamais lancés

Croisement corpus écrit ↔ ads live. Sur ~35 scripts long-form rédigés, **16 tournent** (dont 5 sont des duplicatas visuels de 2 scripts). Ce qui n'a jamais été mis en ligne, classé par note d'adaptation :

| Script | Note | Pourquoi c'est un problème qu'il ne tourne pas |
|---|---|---|
| [[script-lista-kertesz]] (Ad 17, avocat énergie / liste de priorité) | **9,5/10 — noté "LE MEILLEUR POUR LA HONGRIE"** | Le seul script du corpus qui **ne dépend pas d'Hormuz/Iran**. Mécanisme = une liste, pas une histoire → aussi le mieux convertible en vidéo 7 blocs. Jamais lancé. |
| [[script-benzinkut-finomito]] (Ad 14, MOL Százhalombatta) | 9/10 | Ancrage 100 % vérifiable et local (une seule raffinerie, un seul oléoduc). |
| [[script-szobak-fordito]] (Ad 12, le traducteur) | 9/10 | "2020 était une répétition" — mécanisme neuf. |
| [[script-ejszakai-szallitmany]] (Ad 20, framework 4 seaux) | 8,5/10 | Framework structurellement différent. |
| [[script-eltunt-srac]] (Ad 21, bunkers milliardaires) | 8/10 | |
| [[script-faraday-kalitka]] (Ad 18) / [[script-kocsma-digitalid]] (Ad 10) / [[script-batyam-tek]] (Ad 8) / [[script-level-honvedseg]] (Ad 11) / [[script-emp-halozat]] (Ad 6) / [[script-repter-wizz]] (Ad 5) / [[script-amis-fuggoseg]] (Ad 19, seul script sans insider) | 7,5 → 8/10 | |
| `scripts-native-ads-batch2.md` — 11 scripts (technicien des eaux ×3 variantes, médecin de campagne, belle-mère, chauffeur BKV, pompier volontaire, Tiszafüred, petit-fils, père en 56, vétérinaire, compteur d'eau, voisine) + constellation militaire M1/M2/M4 | — | Section "TRACKING — Script vers Adset" du fichier **encore vide** : ces scripts n'ont jamais été rattachés à un adset. |
| `adC` (copine du militaire), `adD` (lettre Honvédség), `adE` (père électricien), `adG` (plombier tuyaux) | — | Écrits en HU + déclinés SK/CZ, absents des actives HU. |
| 13 briefs vidéo (`briefs/`) dont les 5 du framework 7 blocs du 09/08 | — | Une seule vidéo 7 blocs tourne (€188). |

**C'est le déséquilibre central du compte :** on écrit beaucoup plus vite qu'on ne met en ligne, et ce qui est en ligne est concentré sur les deux scripts de juin. Le meilleur script jamais écrit pour ce marché (9,5/10) n'a jamais dépensé un dollar.

## 5. Frictions et incohérences détectées sur les ads live

1. **HYDRA-X1 vs HYDRA-X2 sur le marché hongrois.** Trois créas actives sur `nomadlabs.shop` (HU) parlent de **HYDRA-X1** : "Gyorsan fogy a HYDRA-X1 családi készlet" (€169), "katonai minőségű HYDRA-X1 vészhelyzeti víztisztító szívószállal" (€176 + €80). Or HYDRA-X1 est le nom retenu pour les marchés **SK/CZ** (note du 02/08) ; la PDP hongroise vend **HYDRA-X2**. ~€425 d'EU spend estimé sur des ads dont le nom produit ne correspond pas à la page d'atterrissage. À corriger — c'est de la friction de conversion gratuite.
2. **"Katonai minőségű" / claim militaire toujours en ligne** alors que la règle compliance du 18/07 dit explicitement « pas de claim militaire ». Présent sur l'ad €176/€80 et sur la copie de l'ad €169 ("amerikai katonai műveleti egységek is megbíznak").
3. **1500L vs 400L** : friction déjà documentée le 20/07, arbitrée (on ne touche pas aux scripts Bolt/Tibor vu les stats). Toujours vraie sur les deux plus gros dépenseurs. Pas d'action, mais elle nourrit les commentaires sceptiques que CommentGuard doit absorber.
4. **Nommage des ads = angle mort d'attribution.** Les ads s'appellent "ads 1" à "ads 13", plus des suffixes de duplication ("ads 1 - 27_07 (5)", "20_07 - ads 3 (3)"). Résultat : **impossible de relier un chiffre de l'export Meta à un script au-delà des adsets legacy**, où le mapping avait été fait à la main le 22/07. Sur les 144 lignes de batchs datés, on ne peut juger qu'au niveau du batch — pas du script. C'est la raison pour laquelle cet audit doit passer par la bibliothèque publicitaire pour identifier les créas, avec un plancher de visibilité à €31.

## 6. Ce que la data dit, en clair

- **L'angle #1 (insider géopolitique → énergie → eau) reste ~90 % du spend et fonctionne toujours**, mais son rendement marginal baisse : les nouvelles variantes de narrateur sur le même mécanisme passent de CPA $6,89 à $17.
- **Le mécanisme est saturé, pas l'angle.** Ce qui a marché en juillet, ce sont des variantes lancées quand le mécanisme était encore frais pour l'audience. Continuer à empiler des insiders (livreur, chef de chantier, hôte de vendégház, traducteur, gardien…) revient à re-servir la même révélation.
- **L'angle #2 (eau déjà contaminée) est le seul relais crédible déjà validé** : Takarítónő est la meilleure ad non-#1 du compte (€115), la facture d'eau démarre, le verre du petit-fils vit. Il est sous-financé alors que c'est l'angle qui ne repose sur aucun pari géopolitique — et l'audit du 16/07 le notait déjà 9/10 en potentiel.
- **Le BOF est le meilleur ratio du compte et le plus petit budget.** Adset 5 BOF / ads 4 : CPA $5,71, ROAS 16,81x sur $834. Les statiques BOF (3 szűrő 2 áráért, mindenkinek akit szeretsz, limitált ajánlat) tournent toutes en dessous de €200.
- **La vidéo n'est pas disqualifiée, elle est mal servie.** Le seul adset vidéo scalé fait CPA $7,95 / ROAS 12,01x — mieux que la moyenne du compte. C'est le batch du 03/08 (concepts hongrois) qui fait $11,84. Et la vidéo la mieux classée en bibliothèque est celle du framework maison 7 blocs.
- **La méthode de test est saine** : 110 ads à zéro achat pour $271 cumulés. On peut tester beaucoup plus large sans risque.

## 7. Prochaines itérations — priorisation

**Scale immédiat (rien à produire) :**
1. Monter le budget de **ads 4** (legacy) — meilleur ratio à volume, 41 % du budget de ads 3.
2. Monter le **BOF** (Adset 5 BOF, CPA $5,71) et financer réellement les statiques d'offre.
3. Couper ou remplacer **ads 2** ($10,37 CPA sur $1 317).
4. Laisser mûrir 07/08 et 08/08 jusqu'au 12-13/08 avant jugement.

**Native ads — itérer sur ce qui a dépensé, pas sur le corpus concurrent :**
5. **Húgom Szerbiából** (€270) est la meilleure nouvelle entrée : itérer sur *son* levier différenciant — la crise vécue par un proche à l'étranger, preuve par témoignage familial et non par insider. Variantes : le fils en Ukraine, la sœur en Serbie qui rappelle, le cousin qui a vécu le blackout Espagne/Portugal.
6. **Takarítónő** (€115) : itérer l'angle #2 avec la même mécanique « je nettoie/j'entretiens et j'ai vu ce que personne ne voit » → le plombier (`adG`, déjà écrit), le technicien des eaux (batch 2, déjà écrit), la laborantine (brief existant). Ces trois scripts existent déjà et ne tournent pas.
7. **Lancer enfin [[script-lista-kertesz]]** (9,5/10) : c'est le seul angle #1 qui change de *mécanisme* — pas une révélation d'insider sur un scénario futur, mais un document qui existe déjà (la liste de priorité de délestage, data centers avant les familles). Il sort du pari Hormuz que l'audience commence à connaître par cœur.
8. Idem [[script-benzinkut-finomito]] (9/10) — un seul fait vérifiable et local.

**Vidéo — concepts à faire à partir des ads qui dépensent :**
9. **Framework 7 blocs sur László et sur Húgom Szerbiából.** La règle de conversion du 09/08 s'applique : l'insider de la native devient la « figure qui sait » du bloc 2. László est déjà converti ; Húgom Szerbiából ne l'est pas et c'est la native la plus fraîche à performer.
10. **Convertir Takarítónő en vidéo 7 blocs** — angle #2 en vidéo n'existe pas encore, et les 3 briefs qui le couvrent (technicien, laborantine, plombier) sont écrits mais jamais montés.
11. Réutiliser les patterns visuels de la winner interne (satellite nuit + flash, cascade réseau→pompes→robinet, supermarché depuis le parking, archives TV Texas bandeau rouge, mains qui vissent le filtre, coupe 3D membrane, tiroir qu'on referme) — ils sont déjà identifiés au 09/08.

**Process (à faire une fois, débloque tout le reste) :**
12. **Renommer les ads avec le slug du script** (`laszlo-voisine`, `hugom-szerbia`, `lista-kertesz`…) au lieu de "ads 1..13". Sans ça, chaque audit futur devra repasser par la bibliothèque publicitaire avec un plancher de visibilité à €31, et 39 % du spend restera non attribuable à un script.
13. Remplir la section **TRACKING — Script vers Adset** de `scripts-native-ads-batch2.md` au lancement, pas après.
14. Corriger HYDRA-X1 → HYDRA-X2 sur les créas HU et retirer les claims militaires restants.
