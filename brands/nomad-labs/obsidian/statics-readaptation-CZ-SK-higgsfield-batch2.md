# Statiques Nomad Labs — réadaptation CZ / SK, batch 2 (prompts Higgsfield)

Suite de [[statics-readaptation-CZ-SK-higgsfield]] (ads 1-5). Ce fichier couvre les ads 6-14.
Ad copies associées : [[ad-copies-CZ-SK-batch1]]

Workflow identique : Ruben upload l'image HU source dans Higgsfield + colle le prompt.
Niveau d'adaptation : traduction + localisation légère. Casting, décor, packaging, composition, palette, typo, layout strictement identiques.

**Spécificité de ce batch** : deux ratios différents (ads 13-14 en 9:16 story, le reste en 4:5). Chaque prompt dit « preserve the original aspect ratio of the uploaded image » plutôt que de figer une valeur.

## Grille de prix appliquée

| Marché | Prix barré | Bundle 2+1 | À l'unité | Remise |
|---|---|---|---|---|
| HU (source) | 52 200 Ft | 29 900 Ft | 17 400 Ft | −43 % |
| CZ | 3 270 Kč | 1 860 Kč | 1 090 Kč | −43 % |
| SK | 135 € | 77 € | 45 € | −43 % |

## Points de vigilance

1. **Les 4 créas manuscrites (ads 10, 12, 13, 14) sont les plus dures.** Le modèle doit régénérer de l'écriture à la main avec diacritiques — c'est le principal point de casse. Les ads 10 et 12 sont des photos : si le rendu perd le grain ou la lumière naturelle, refaire un passage en réuploadant le résultat.
2. **Ad 8, caption 8** (« Myslíš si, že se to tu stát nemůže ») est la plus longue de la grille — premier endroit où la mise en page se déforme. Vérifier qu'elle tient sur 2 lignes comme les 7 autres.
3. **Ad 9 : le « -43% » du ruban ne se traduit pas et ne se recalcule pas.** Verrouillé explicitement dans le prompt.
4. Diacritiques les plus souvent ratées : `ř` `ě` `ů` (CZ), `ô` `ľ` `ä` (SK).

---

## Ad 6 — Offre « tu paies 2, tu reçois 3 » (fond sombre, table bois)

| Bloc | FR | CZ | SK |
|---|---|---|---|
| Badge L1 | ON VOUS PRÉSENTE | PŘEDSTAVUJEME | PREDSTAVUJEME |
| Badge L2 | LE PACK FAMILLE | RODINNÝ BALÍČEK | RODINNÝ BALÍK |
| Titre | TU PAIES 2 / TU REÇOIS 3 | PLATÍŠ ZA 2 / DOSTANEŠ 3 | PLATÍŠ ZA 2 / DOSTANEŠ 3 |
| Icône 1 | LIVRAISON GRATUITE | DOPRAVA ZDARMA | DOPRAVA ZADARMO |
| Icône 2 | 3 E-BOOKS OFFERTS | 3 E-KNIHY ZDARMA | 3 E-KNIHY ZADARMO |
| Icône 3 | GARANTIE REMBOURSÉ 90 JOURS | 90DENNÍ ZÁRUKA VRÁCENÍ PENĚZ | 90-DŇOVÁ ZÁRUKA VRÁTENIA PEŇAZÍ |
| Prix | 29 900 Ft / 52 200 Ft barré | 1 860 Kč / 3 270 Kč | 77 € / 135 € |

### Prompt CZ

```
Edit the uploaded image. This is a Czech-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image
- Dark charcoal/near-black background with the soft blue gradient glow, and the wooden table surface with its grain and reflections
- The three Hydra X2 filter straws standing on the table: identical 3D render, identical position, scale, spacing, light-blue body, royal-blue cap and base, blue loop handle, identical shadows and reflections, and the vertical "NOMAD LABS" branding printed on each straw (stays in English)
- The thin-outline badge box at the top, the three thin-line white icons (delivery truck, gift box, shield), the thin horizontal divider lines between them, and the white circle at the bottom left with the orange diagonal strikethrough
- All colors: orange for "2-T FIZETSZ" and for the strikethrough, white for the rest, dark text inside the white price circle
- Typography: same heavy condensed all-caps sans-serif for the headline, same small bold all-caps for the badge and the icon captions, same bold for the prices, same left alignment and same vertical position for every text block

CHANGE ONLY these Hungarian strings, replacing them with Czech and converting the currency to Czech koruna:
- Badge line 1: "BEMUTATJUK" becomes "PŘEDSTAVUJEME"
- Badge line 2: "A CSALÁDI CSOMAG" becomes "RODINNÝ BALÍČEK"
- Headline line 1: "2-T FIZETSZ" becomes "PLATÍŠ ZA 2"
- Headline line 2: "3-AT KAPSZ" becomes "DOSTANEŠ 3"
- Icon caption 1: "INGYENES SZÁLLÍTÁS" becomes "DOPRAVA ZDARMA"
- Icon caption 2: "3 AJÁNDÉK E-KÖNYV" becomes "3 E-KNIHY ZDARMA"
- Icon caption 3: "90 NAPOS PÉNZVISSZAFIZETÉSI GARANCIA" becomes "90DENNÍ ZÁRUKA VRÁCENÍ PENĚZ"
- Big price: "29 900 Ft" becomes "1 860 Kč"
- Struck-through price: "52 200 Ft" becomes "3 270 Kč"

TEXT RULES:
- Render Czech diacritics perfectly and legibly: á é ě í ó ú ů ý č ď ň ř š ť ž. Never drop, flatten or distort an accent.
- Format prices Czech style: a thin space as thousands separator and "Kč" after the number, e.g. "1 860 Kč", "3 270 Kč".
- The headline stays on exactly two left-aligned lines. The badge stays on two lines. Icon captions 1 and 2 stay on two lines each, caption 3 stays on three lines, exactly as in the original. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- The orange strikethrough must land precisely over the new struck price, at the same angle and thickness.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

### Prompt SK

```
Edit the uploaded image. This is a Slovak-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image
- Dark charcoal/near-black background with the soft blue gradient glow, and the wooden table surface with its grain and reflections
- The three Hydra X2 filter straws standing on the table: identical 3D render, identical position, scale, spacing, light-blue body, royal-blue cap and base, blue loop handle, identical shadows and reflections, and the vertical "NOMAD LABS" branding printed on each straw (stays in English)
- The thin-outline badge box at the top, the three thin-line white icons (delivery truck, gift box, shield), the thin horizontal divider lines between them, and the white circle at the bottom left with the orange diagonal strikethrough
- All colors: orange for the first headline line and for the strikethrough, white for the rest, dark text inside the white price circle
- Typography: same heavy condensed all-caps sans-serif for the headline, same small bold all-caps for the badge and the icon captions, same bold for the prices, same left alignment and same vertical position for every text block

CHANGE ONLY these Hungarian strings, replacing them with Slovak and converting the currency to euro:
- Badge line 1: "BEMUTATJUK" becomes "PREDSTAVUJEME"
- Badge line 2: "A CSALÁDI CSOMAG" becomes "RODINNÝ BALÍK"
- Headline line 1: "2-T FIZETSZ" becomes "PLATÍŠ ZA 2"
- Headline line 2: "3-AT KAPSZ" becomes "DOSTANEŠ 3"
- Icon caption 1: "INGYENES SZÁLLÍTÁS" becomes "DOPRAVA ZADARMO"
- Icon caption 2: "3 AJÁNDÉK E-KÖNYV" becomes "3 E-KNIHY ZADARMO"
- Icon caption 3: "90 NAPOS PÉNZVISSZAFIZETÉSI GARANCIA" becomes "90-DŇOVÁ ZÁRUKA VRÁTENIA PEŇAZÍ"
- Big price: "29 900 Ft" becomes "77 €"
- Struck-through price: "52 200 Ft" becomes "135 €"

TEXT RULES:
- Render Slovak diacritics perfectly and legibly: á ä é í ó ô ú ý č ď ľ ĺ ň ŕ š ť ž. Never drop, flatten or distort an accent.
- Format prices Slovak style: the euro sign after the number with a space, e.g. "77 €", "135 €".
- The headline stays on exactly two left-aligned lines. The badge stays on two lines. Icon captions 1 and 2 stay on two lines each, caption 3 stays on three lines, exactly as in the original. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- The orange strikethrough must land precisely over the new struck price, at the same angle and thickness.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

---

## Ad 7 — Démo 3 verres « microplastique filtré »

| Bloc | FR | CZ | SK |
|---|---|---|---|
| Titre | MICROPLASTIQUE FILTRÉ | MIKROPLASTY ODFILTROVÁNY | MIKROPLASTY ODFILTROVANÉ |
| Sous-titre | OU TU ES REMBOURSÉ | NEBO DOSTANEŠ PENÍZE ZPĚT | ALEBO DOSTANEŠ PENIAZE SPÄŤ |
| Verre 1 | EAU DU ROBINET | VODA Z KOHOUTKU | VODA Z KOHÚTIKA |
| Verre 2 | FILTRATION | FILTRACE | FILTRÁCIA |
| Verre 3 | EAU PROPRE | ČISTÁ VODA | ČISTÁ VODA |

### Prompt CZ

```
Edit the uploaded image. This is a Czech-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image
- White background
- The black horizontal bar at the top holding the headline
- The three black photo panels of backlit glasses of water: same images, same crops, same order and same particle progression (many visible particles, fewer particles, perfectly clear). Do not regenerate, re-light or re-render the glasses or the water.
- The three orange hand-drawn circle annotations over the glasses: same stroke weight, same position, same imperfect hand-drawn look
- The three Hydra X2 filter straws at the bottom: identical 3D render, identical position, scale, tilt, spacing, light-blue body, royal-blue cap and base, blue loop handle, and the vertical "NOMAD LABS" branding on each (stays in English)
- Typography: same heavy black all-caps condensed sans-serif, white on the black bar for the headline, black for the sub-headline and the three panel labels, same centering and same vertical position for every text block

CHANGE ONLY these Hungarian strings, replacing them with Czech:
- Headline in the black bar: "MIKROMŰANYAG KISZŰRVE" becomes "MIKROPLASTY ODFILTROVÁNY"
- Sub-headline: "VAGY VISSZAKAPOD A PÉNZED" becomes "NEBO DOSTANEŠ PENÍZE ZPĚT"
- Label under panel 1: "CSAPVÍZ" becomes "VODA Z KOHOUTKU"
- Label under panel 2: "SZŰRÉS" becomes "FILTRACE"
- Label under panel 3: "TISZTA VÍZ" becomes "ČISTÁ VODA"

TEXT RULES:
- Render Czech diacritics perfectly and legibly: á é ě í ó ú ů ý č ď ň ř š ť ž. Never drop, flatten or distort an accent.
- Every string stays on one centered line, exactly as in the original. The headline must still fit inside the black bar with the same margins. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

### Prompt SK

```
Edit the uploaded image. This is a Slovak-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image
- White background
- The black horizontal bar at the top holding the headline
- The three black photo panels of backlit glasses of water: same images, same crops, same order and same particle progression (many visible particles, fewer particles, perfectly clear). Do not regenerate, re-light or re-render the glasses or the water.
- The three orange hand-drawn circle annotations over the glasses: same stroke weight, same position, same imperfect hand-drawn look
- The three Hydra X2 filter straws at the bottom: identical 3D render, identical position, scale, tilt, spacing, light-blue body, royal-blue cap and base, blue loop handle, and the vertical "NOMAD LABS" branding on each (stays in English)
- Typography: same heavy black all-caps condensed sans-serif, white on the black bar for the headline, black for the sub-headline and the three panel labels, same centering and same vertical position for every text block

CHANGE ONLY these Hungarian strings, replacing them with Slovak:
- Headline in the black bar: "MIKROMŰANYAG KISZŰRVE" becomes "MIKROPLASTY ODFILTROVANÉ"
- Sub-headline: "VAGY VISSZAKAPOD A PÉNZED" becomes "ALEBO DOSTANEŠ PENIAZE SPÄŤ"
- Label under panel 1: "CSAPVÍZ" becomes "VODA Z KOHÚTIKA"
- Label under panel 2: "SZŰRÉS" becomes "FILTRÁCIA"
- Label under panel 3: "TISZTA VÍZ" becomes "ČISTÁ VODA"

TEXT RULES:
- Render Slovak diacritics perfectly and legibly: á ä é í ó ô ú ý č ď ľ ĺ ň ŕ š ť ž. Never drop, flatten or distort an accent.
- Every string stays on one centered line, exactly as in the original. The headline must still fit inside the black bar with the same margins. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

---

## Ad 8 — Checklist « 8 signes »

| Bloc | FR | CZ | SK |
|---|---|---|---|
| Titre | 8 SIGNES | 8 ZNAMENÍ | 8 ZNAKOV |
| Bandeau orange | QUE TA FAMILLE N'EST PAS PRÊTE | ŽE TVOJE RODINA NENÍ PŘIPRAVENÁ | ŽE TVOJA RODINA NIE JE PRIPRAVENÁ |
| 1 | Tu n'as pas d'eau pour 2 jours | Nemáš vodu na 2 dny | Nemáš vodu na 2 dni |
| 2 | Tu ne sais pas où est la source d'eau | Nevíš, kde je zdroj vody | Nevieš, kde je zdroj vody |
| 3 | C'est une pompe qui amène ton eau | Vodu ti žene čerpadlo | Vodu ti ženie čerpadlo |
| 4 | Tu comptes sur le magasin | Spoléháš na obchod | Spoliehaš sa na obchod |
| 5 | Les petits-enfants dorment chez toi | Spí u tebe vnoučata | Spia u teba vnúčatá |
| 6 | Tu vis en appartement, sans puits | Bydlíš v bytě, bez studny | Bývaš v byte, bez studne |
| 7 | Tu ne sais pas purifier l'eau | Neumíš vodu vyčistit | Nevieš vyčistiť vodu |
| 8 | Tu crois que ça ne peut pas arriver ici | Myslíš si, že se to tu stát nemůže | Myslíš si, že sa to tu stať nemôže |
| Lien | Prépare-toi avant d'en avoir besoin | Připrav se dřív, než to budeš potřebovat | Priprav sa skôr, než to budeš potrebovať |
| Bouton | ESSAIE SANS RISQUE → | VYZKOUŠEJ BEZ RIZIKA → | VYSKÚŠAJ BEZ RIZIKA → |

### Prompt CZ

```
Edit the uploaded image. This is a Czech-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image
- White background
- The eight blue thin-line icons in their 4x2 grid: two bottles, question-mark map pin, electric pump, shopping cart, grandmother with child, apartment block, crossed-out tap, shrugging person. Same style, same stroke weight, same size, same positions. Do not redraw or reinterpret them.
- The orange rounded sub-headline bar under the "8" headline, the orange underlined link line, and the black rounded CTA button with its white arrow
- All colors: black headline, white text on the orange bar, black icon captions, orange underlined link, white text on the black button
- Typography: same very heavy black sans-serif for the "8" headline, same bold all-caps for the orange bar, same bold sentence-case for the eight captions, same bold for the link, same bold all-caps for the button, same centering and same vertical position for every text block

CHANGE ONLY these Hungarian strings, replacing them with Czech:
- Headline: "8 JEL" becomes "8 ZNAMENÍ"
- Orange bar: "HOGY A CSALÁDOD NINCS FELKÉSZÜLVE" becomes "ŽE TVOJE RODINA NENÍ PŘIPRAVENÁ"
- Caption 1: "Nincs 2 / napra vized" becomes "Nemáš vodu / na 2 dny"
- Caption 2: "Nem tudod, / hol a vízforrás" becomes "Nevíš, kde / je zdroj vody"
- Caption 3: "Szivattyú / viszi a vized" becomes "Vodu ti / žene čerpadlo"
- Caption 4: "A boltra / számítasz" becomes "Spoléháš / na obchod"
- Caption 5: "Nálad alszanak / az unokák" becomes "Spí u tebe / vnoučata"
- Caption 6: "Lakásban / laksz, kút nélkül" becomes "Bydlíš v bytě, / bez studny"
- Caption 7: "Nem tudsz / vizet tisztítani" becomes "Neumíš / vodu vyčistit"
- Caption 8: "Azt hiszed, / itt nem történhet meg" becomes "Myslíš si, že se / to tu stát nemůže"
- Orange link line: "Készülj fel, mielőtt szükség lesz rá" becomes "Připrav se dřív, než to budeš potřebovat"
- Black button: "PRÓBÁLD KI KOCKÁZAT NÉLKÜL →" becomes "VYZKOUŠEJ BEZ RIZIKA →" (keep the arrow glyph)

TEXT RULES:
- Render Czech diacritics perfectly and legibly: á é ě í ó ú ů ý č ď ň ř š ť ž. Never drop, flatten or distort an accent.
- Each of the eight captions stays on exactly two centered lines under its icon. The orange bar, the link line and the button each stay on one centered line. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- Keep the orange underline under the link line, matching the new text width.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

### Prompt SK

```
Edit the uploaded image. This is a Slovak-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image
- White background
- The eight blue thin-line icons in their 4x2 grid: two bottles, question-mark map pin, electric pump, shopping cart, grandmother with child, apartment block, crossed-out tap, shrugging person. Same style, same stroke weight, same size, same positions. Do not redraw or reinterpret them.
- The orange rounded sub-headline bar under the "8" headline, the orange underlined link line, and the black rounded CTA button with its white arrow
- All colors: black headline, white text on the orange bar, black icon captions, orange underlined link, white text on the black button
- Typography: same very heavy black sans-serif for the "8" headline, same bold all-caps for the orange bar, same bold sentence-case for the eight captions, same bold for the link, same bold all-caps for the button, same centering and same vertical position for every text block

CHANGE ONLY these Hungarian strings, replacing them with Slovak:
- Headline: "8 JEL" becomes "8 ZNAKOV"
- Orange bar: "HOGY A CSALÁDOD NINCS FELKÉSZÜLVE" becomes "ŽE TVOJA RODINA NIE JE PRIPRAVENÁ"
- Caption 1: "Nincs 2 / napra vized" becomes "Nemáš vodu / na 2 dni"
- Caption 2: "Nem tudod, / hol a vízforrás" becomes "Nevieš, kde / je zdroj vody"
- Caption 3: "Szivattyú / viszi a vized" becomes "Vodu ti / ženie čerpadlo"
- Caption 4: "A boltra / számítasz" becomes "Spoliehaš sa / na obchod"
- Caption 5: "Nálad alszanak / az unokák" becomes "Spia u teba / vnúčatá"
- Caption 6: "Lakásban / laksz, kút nélkül" becomes "Bývaš v byte, / bez studne"
- Caption 7: "Nem tudsz / vizet tisztítani" becomes "Nevieš / vyčistiť vodu"
- Caption 8: "Azt hiszed, / itt nem történhet meg" becomes "Myslíš si, že sa / to tu stať nemôže"
- Orange link line: "Készülj fel, mielőtt szükség lesz rá" becomes "Priprav sa skôr, než to budeš potrebovať"
- Black button: "PRÓBÁLD KI KOCKÁZAT NÉLKÜL →" becomes "VYSKÚŠAJ BEZ RIZIKA →" (keep the arrow glyph)

TEXT RULES:
- Render Slovak diacritics perfectly and legibly: á ä é í ó ô ú ý č ď ľ ĺ ň ŕ š ť ž. Never drop, flatten or distort an accent.
- Each of the eight captions stays on exactly two centered lines under its icon. The orange bar, the link line and the button each stay on one centered line. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- Keep the orange underline under the link line, matching the new text width.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

---

## Ad 9 — Urgence « ruban −43 % »

| Bloc | FR | CZ | SK |
|---|---|---|---|
| Titre L1 | CETTE OFFRE | TAHLE NABÍDKA | TÁTO PONUKA |
| Titre L2 | NE DURERA PAS | DLOUHO NEVYDRŽÍ | DLHO NEVYDRŽÍ |
| Pilule | 3 E-BOOKS OFFERTS + LIVRAISON GRATUITE | 3 E-KNIHY ZDARMA + DOPRAVA ZDARMA | 3 E-KNIHY ZADARMO + DOPRAVA ZADARMO |

### Prompt CZ

```
Edit the uploaded image. This is a Czech-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image
- The concrete/stone backdrop, the dark pebbles, the water droplets and the soft shadows
- The Hydra X2 filter straw floating in the centre: identical 3D render, identical position, tilt, scale, light-blue body, royal-blue cap and base, blue loop handle, and the vertical "NOMAD LABS" branding (stays in English)
- The orange ribbon spiralling around the straw with the repeated "-43%" printed on it: same shape, same curl, same number of turns, same shadows. Every "-43%" on the ribbon stays exactly "-43%" and is not translated.
- The orange rounded pill bar at the bottom
- All colors: orange for the ribbon, for "EZ AZ AJÁNLAT" and for the pill; near-black for the second headline line; white text on the pill
- Typography: same heavy condensed all-caps sans-serif for the headline, same small bold all-caps for the pill, same centering and same vertical position for every text block

CHANGE ONLY these Hungarian strings, replacing them with Czech:
- Headline line 1 (orange): "EZ AZ AJÁNLAT" becomes "TAHLE NABÍDKA"
- Headline line 2 (dark): "NEM TART SOKÁIG" becomes "DLOUHO NEVYDRŽÍ"
- Pill bar: "3 AJÁNDÉK E-KÖNYV + INGYENES SZÁLLÍTÁS" becomes "3 E-KNIHY ZDARMA + DOPRAVA ZDARMA"

TEXT RULES:
- Render Czech diacritics perfectly and legibly: á é ě í ó ú ů ý č ď ň ř š ť ž. Never drop, flatten or distort an accent.
- The headline stays on exactly two centered lines. The pill text stays on one centered line inside the pill, with the same margins. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

### Prompt SK

```
Edit the uploaded image. This is a Slovak-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image
- The concrete/stone backdrop, the dark pebbles, the water droplets and the soft shadows
- The Hydra X2 filter straw floating in the centre: identical 3D render, identical position, tilt, scale, light-blue body, royal-blue cap and base, blue loop handle, and the vertical "NOMAD LABS" branding (stays in English)
- The orange ribbon spiralling around the straw with the repeated "-43%" printed on it: same shape, same curl, same number of turns, same shadows. Every "-43%" on the ribbon stays exactly "-43%" and is not translated.
- The orange rounded pill bar at the bottom
- All colors: orange for the ribbon, for the first headline line and for the pill; near-black for the second headline line; white text on the pill
- Typography: same heavy condensed all-caps sans-serif for the headline, same small bold all-caps for the pill, same centering and same vertical position for every text block

CHANGE ONLY these Hungarian strings, replacing them with Slovak:
- Headline line 1 (orange): "EZ AZ AJÁNLAT" becomes "TÁTO PONUKA"
- Headline line 2 (dark): "NEM TART SOKÁIG" becomes "DLHO NEVYDRŽÍ"
- Pill bar: "3 AJÁNDÉK E-KÖNYV + INGYENES SZÁLLÍTÁS" becomes "3 E-KNIHY ZADARMO + DOPRAVA ZADARMO"

TEXT RULES:
- Render Slovak diacritics perfectly and legibly: á ä é í ó ô ú ý č ď ľ ĺ ň ŕ š ť ž. Never drop, flatten or distort an accent.
- The headline stays on exactly two centered lines. The pill text stays on one centered line inside the pill, with the same margins. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

---

## Ad 10 — UGC « écriture sur la vitre de douche »

| Bloc | FR | CZ | SK |
|---|---|---|---|
| Cercle gauche | Il filtre ce que tu ne vois pas | Vyfiltruje, co nevidíš | Vyfiltruje, čo nevidíš |
| Cercle droit | Zéro produit chimique, zéro pile | Nula chemie, nula baterií | Nula chémie, nula batérií |

### Prompt CZ

```
Edit the uploaded image. This is a Czech-market localization of an existing ad creative. Only the handwritten copy on the glass changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image
- The fogged-up shower glass, the wet grey tiles behind it, the condensation, the water streaks and the drips running down from the writing
- The two hand-drawn circles finger-written in the condensation: same size, same position, same imperfect wobbly stroke
- The real human hand entering from the bottom of the frame: identical skin, identical grip, identical pose and lighting
- The Hydra X2 filter straw held in the hand: identical product, position, angle, light-blue body, royal-blue cap and base, blue loop handle, and the "NOMAD LABS" branding on it (stays in English)
- The amateur smartphone-photo look: same grain, same soft focus, same colour cast, same natural bathroom lighting. This must still read as a real UGC photo, not as a clean graphic.

CHANGE ONLY the handwritten Hungarian text finger-written in the condensation, replacing it with Czech:
- Left circle: "Kiszűri, amit nem látsz" becomes "Vyfiltruje, co nevidíš"
- Right circle: "Nulla vegyszer, nulla elem" becomes "Nula chemie, nula baterií"

TEXT RULES:
- The new text must be written in the SAME finger-on-fogged-glass handwriting: same uneven stroke width, same slight slant, same smeared edges, same clear-glass-through-condensation look, with the same water drips running down from the letters.
- Render Czech diacritics perfectly and legibly: á é ě í ó ú ů ý č ď ň ř š ť ž. Write them as handwritten finger strokes too, never as printed type. Never drop or flatten an accent.
- Keep each phrase inside its circle, on the same number of lines as the original (left: three lines, right: two lines), at the same size relative to the circle.
- Do not add printed text, watermark, logo or any graphic overlay. The image must stay a photograph.
```

### Prompt SK

```
Edit the uploaded image. This is a Slovak-market localization of an existing ad creative. Only the handwritten copy on the glass changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image
- The fogged-up shower glass, the wet grey tiles behind it, the condensation, the water streaks and the drips running down from the writing
- The two hand-drawn circles finger-written in the condensation: same size, same position, same imperfect wobbly stroke
- The real human hand entering from the bottom of the frame: identical skin, identical grip, identical pose and lighting
- The Hydra X2 filter straw held in the hand: identical product, position, angle, light-blue body, royal-blue cap and base, blue loop handle, and the "NOMAD LABS" branding on it (stays in English)
- The amateur smartphone-photo look: same grain, same soft focus, same colour cast, same natural bathroom lighting. This must still read as a real UGC photo, not as a clean graphic.

CHANGE ONLY the handwritten Hungarian text finger-written in the condensation, replacing it with Slovak:
- Left circle: "Kiszűri, amit nem látsz" becomes "Vyfiltruje, čo nevidíš"
- Right circle: "Nulla vegyszer, nulla elem" becomes "Nula chémie, nula batérií"

TEXT RULES:
- The new text must be written in the SAME finger-on-fogged-glass handwriting: same uneven stroke width, same slight slant, same smeared edges, same clear-glass-through-condensation look, with the same water drips running down from the letters.
- Render Slovak diacritics perfectly and legibly: á ä é í ó ô ú ý č ď ľ ĺ ň ŕ š ť ž. Write them as handwritten finger strokes too, never as printed type. Never drop or flatten an accent.
- Keep each phrase inside its circle, on the same number of lines as the original (left: three lines, right: two lines), at the same size relative to the circle.
- Do not add printed text, watermark, logo or any graphic overlay. The image must stay a photograph.
```

---

## Ad 11 — Verre coupé en deux « purificateur vs Hydra X2 »

| Bloc | FR | CZ | SK |
|---|---|---|---|
| Gauche | PURIFICATEUR D'EAU | ČISTIČKA VODY | ČISTIČKA VODY |
| Droite | PURIFICATEUR D'EAU + HYDRA X2 | ČISTIČKA VODY + HYDRA X2 | ČISTIČKA VODY + HYDRA X2 |
| Légende | LE PURIFICATEUR NE FILTRE PAS LE MICROPLASTIQUE. LE HYDRA X2 SI. | ČISTIČKA VODY MIKROPLASTY NEODFILTRUJE. HYDRA X2 ANO. | ČISTIČKA VODY MIKROPLASTY NEODFILTRUJE. HYDRA X2 ÁNO. |
| Bouton | ESSAIE SANS RISQUE → | VYZKOUŠEJ BEZ RIZIKA → | VYSKÚŠAJ BEZ RIZIKA → |

### Prompt CZ

```
Edit the uploaded image. This is a Czech-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image
- Light warm-grey background
- The single illustrated glass split down the middle by a thin vertical black line: identical flat-vector illustration style, identical shape, identical position and scale. The left half stays murky beige-orange with the same orange debris, bacteria and microplastic shapes in the same places. The right half stays clean blue with the same gradient. Do not redraw, restyle or re-arrange any of it.
- The blue rounded CTA button with its white arrow
- All colors: black headings and caption, blue button, white button text, "Nomad Labs" in dark grey at the bottom
- Typography: same bold all-caps sans-serif for the two column headings, same bold all-caps for the caption line, same bold all-caps for the button, same regular title-case for "Nomad Labs", same centering and same vertical position for every text block
- The "Nomad Labs" signature at the bottom stays in English, unchanged

CHANGE ONLY these Hungarian strings, replacing them with Czech:
- Left heading: "VÍZTISZTÍTÓ" becomes "ČISTIČKA VODY"
- Right heading: "VÍZTISZTÍTÓ / + HYDRA X2" becomes "ČISTIČKA VODY / + HYDRA X2"
- Caption under the glass: "A VÍZTISZTÍTÓ NEM SZŰRI A MIKROMŰANYAGOT. A HYDRA X2 IGEN." becomes "ČISTIČKA VODY MIKROPLASTY NEODFILTRUJE. HYDRA X2 ANO."
- Blue button: "PRÓBÁLD KI KOCKÁZAT NÉLKÜL →" becomes "VYZKOUŠEJ BEZ RIZIKA →" (keep the arrow glyph)

TEXT RULES:
- Render Czech diacritics perfectly and legibly: á é ě í ó ú ů ý č ď ň ř š ť ž. Never drop, flatten or distort an accent.
- The left heading stays on one line, the right heading on exactly two lines, the caption on one line, the button on one line — all centered exactly as in the original. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

### Prompt SK

```
Edit the uploaded image. This is a Slovak-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image
- Light warm-grey background
- The single illustrated glass split down the middle by a thin vertical black line: identical flat-vector illustration style, identical shape, identical position and scale. The left half stays murky beige-orange with the same orange debris, bacteria and microplastic shapes in the same places. The right half stays clean blue with the same gradient. Do not redraw, restyle or re-arrange any of it.
- The blue rounded CTA button with its white arrow
- All colors: black headings and caption, blue button, white button text, "Nomad Labs" in dark grey at the bottom
- Typography: same bold all-caps sans-serif for the two column headings, same bold all-caps for the caption line, same bold all-caps for the button, same regular title-case for "Nomad Labs", same centering and same vertical position for every text block
- The "Nomad Labs" signature at the bottom stays in English, unchanged

CHANGE ONLY these Hungarian strings, replacing them with Slovak:
- Left heading: "VÍZTISZTÍTÓ" becomes "ČISTIČKA VODY"
- Right heading: "VÍZTISZTÍTÓ / + HYDRA X2" becomes "ČISTIČKA VODY / + HYDRA X2"
- Caption under the glass: "A VÍZTISZTÍTÓ NEM SZŰRI A MIKROMŰANYAGOT. A HYDRA X2 IGEN." becomes "ČISTIČKA VODY MIKROPLASTY NEODFILTRUJE. HYDRA X2 ÁNO."
- Blue button: "PRÓBÁLD KI KOCKÁZAT NÉLKÜL →" becomes "VYSKÚŠAJ BEZ RIZIKA →" (keep the arrow glyph)

TEXT RULES:
- Render Slovak diacritics perfectly and legibly: á ä é í ó ô ú ý č ď ľ ĺ ň ŕ š ť ž. Never drop, flatten or distort an accent.
- The left heading stays on one line, the right heading on exactly two lines, the caption on one line, the button on one line — all centered exactly as in the original. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

---

## Ad 12 — Tableau blanc cuisine « traitée, pas propre »

| Bloc | FR | CZ | SK |
|---|---|---|---|
| Gauche | Purificateur d'eau | Čistička vody | Čistička vody |
| Droite | Purificateur d'eau + Hydra X2 | Čistička vody + Hydra X2 | Čistička vody + Hydra X2 |
| Flèche G | CE QUE LE PURIFICATEUR LAISSE PASSER | CO ČISTIČKA PROPUSTÍ | ČO ČISTIČKA PREPUSTÍ |
| Flèche D | 0,1 MICRON — RIEN NE PASSE | 0,1 MIKRONU — NIC NEPROJDE | 0,1 MIKRÓNU — NIČ NEPREJDE |
| Punchline | Traitée. Pas propre. | Upravená. Ne čistá. | Upravená. Nie čistá. |
| Sous-ligne | Essaie sans risque | Vyzkoušej bez rizika | Vyskúšaj bez rizika |
| Mention | limite de filtration 0,1 micron · 400 litres max par filtre | filtrační limit 0,1 mikronu · nejvýše 400 litrů na filtr | filtračný limit 0,1 mikrónu · najviac 400 litrov na filter |

### Prompt CZ

```
Edit the uploaded image. This is a Czech-market localization of an existing ad creative. Only the handwritten copy on the whiteboard changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image
- The real kitchen photograph: the granite countertop, the wooden cabinets, the knife block, the background blur, the natural lighting, the grain and the amateur smartphone-photo look
- The aluminium-framed whiteboard: same board, same frame, same angle, same reflections and smudges
- The two hand-drawn marker glasses: identical drawing, position and size. The left glass keeps the same orange squiggles and dots inside it. The right glass keeps the same blue scribble fill. Do not redraw or re-arrange them.
- The two hand-drawn curved marker arrows pointing at the glasses: same shape, same position, same stroke
- The real Hydra X2 filter straw standing on the counter at the bottom right: identical product, position, angle, light-blue body, royal-blue cap and base, blue loop handle, and the vertical "NOMAD LABS" branding (stays in English)
- "Hydra X2" stays in English wherever it appears

CHANGE ONLY the handwritten Hungarian marker text on the whiteboard, replacing it with Czech:
- Left column heading: "Víztisztító" becomes "Čistička vody"
- Right column heading: "Víztisztító / + Hydra X2" becomes "Čistička vody / + Hydra X2"
- Left arrow label: "AMIT A TISZTÍTÓ / ÁTENGED" becomes "CO ČISTIČKA / PROPUSTÍ"
- Right arrow label: "0,1 MIKRON — / SEMMI NEM JUT ÁT" becomes "0,1 MIKRONU — / NIC NEPROJDE"
- Big punchline: "Kezelt. Nem tiszta." becomes "Upravená. Ne čistá."
- Sub-line: "Próbáld ki kockázat nélkül" becomes "Vyzkoušej bez rizika"
- Small print at the bottom: "0,1 mikronos szűrési határ · legfeljebb 400 liter szűrőnként" becomes "filtrační limit 0,1 mikronu · nejvýše 400 litrů na filtr"

TEXT RULES:
- The new text must be written in the SAME black dry-erase marker handwriting: same stroke width, same casual hand, same slight unevenness, same size hierarchy. It must look drawn on the board, not typeset over the photo.
- Render Czech diacritics perfectly and legibly: á é ě í ó ú ů ý č ď ň ř š ť ž. Draw them as handwritten marker strokes. Never drop, flatten or distort an accent.
- Keep the line breaks exactly as listed above, and keep every block in the same position and at the same size relative to the board.
- Write the decimal as "0,1" with a comma, never "0.1". Keep the figure 400 unchanged.
- Do not add printed text, watermark, logo or any graphic overlay. The image must stay a photograph.
```

### Prompt SK

```
Edit the uploaded image. This is a Slovak-market localization of an existing ad creative. Only the handwritten copy on the whiteboard changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image
- The real kitchen photograph: the granite countertop, the wooden cabinets, the knife block, the background blur, the natural lighting, the grain and the amateur smartphone-photo look
- The aluminium-framed whiteboard: same board, same frame, same angle, same reflections and smudges
- The two hand-drawn marker glasses: identical drawing, position and size. The left glass keeps the same orange squiggles and dots inside it. The right glass keeps the same blue scribble fill. Do not redraw or re-arrange them.
- The two hand-drawn curved marker arrows pointing at the glasses: same shape, same position, same stroke
- The real Hydra X2 filter straw standing on the counter at the bottom right: identical product, position, angle, light-blue body, royal-blue cap and base, blue loop handle, and the vertical "NOMAD LABS" branding (stays in English)
- "Hydra X2" stays in English wherever it appears

CHANGE ONLY the handwritten Hungarian marker text on the whiteboard, replacing it with Slovak:
- Left column heading: "Víztisztító" becomes "Čistička vody"
- Right column heading: "Víztisztító / + Hydra X2" becomes "Čistička vody / + Hydra X2"
- Left arrow label: "AMIT A TISZTÍTÓ / ÁTENGED" becomes "ČO ČISTIČKA / PREPUSTÍ"
- Right arrow label: "0,1 MIKRON — / SEMMI NEM JUT ÁT" becomes "0,1 MIKRÓNU — / NIČ NEPREJDE"
- Big punchline: "Kezelt. Nem tiszta." becomes "Upravená. Nie čistá."
- Sub-line: "Próbáld ki kockázat nélkül" becomes "Vyskúšaj bez rizika"
- Small print at the bottom: "0,1 mikronos szűrési határ · legfeljebb 400 liter szűrőnként" becomes "filtračný limit 0,1 mikrónu · najviac 400 litrov na filter"

TEXT RULES:
- The new text must be written in the SAME black dry-erase marker handwriting: same stroke width, same casual hand, same slight unevenness, same size hierarchy. It must look drawn on the board, not typeset over the photo.
- Render Slovak diacritics perfectly and legibly: á ä é í ó ô ú ý č ď ľ ĺ ň ŕ š ť ž. Draw them as handwritten marker strokes. Never drop, flatten or distort an accent.
- Keep the line breaks exactly as listed above, and keep every block in the same position and at the same size relative to the board.
- Write the decimal as "0,1" with a comma, never "0.1". Keep the figure 400 unchanged.
- Do not add printed text, watermark, logo or any graphic overlay. The image must stay a photograph.
```

---

## Ad 13 — Marker story « 2 achetés = 1 offert »

| Bloc | FR | CZ | SK |
|---|---|---|---|
| Titre | PACK FAMILLE | RODINNÝ BALÍČEK | RODINNÝ BALÍK |
| Annotation | GRATUIT | ZDARMA | ZADARMO |
| Punchline | Tu en prends 2 = 1 gratuit | Koupíš 2 = 1 zdarma | Kúpiš 2 = 1 zadarmo |
| Bas | Stock limité | Zásoby omezené | Zásoby obmedzené |

### Prompt CZ

```
Edit the uploaded image. This is a Czech-market localization of an existing ad creative. Only the handwritten copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image (this is a tall vertical story format)
- Plain white background
- The three Hydra X2 filter straws: identical 3D render, identical positions (two on top, one below centre), identical scale, tilt and spacing, light-blue body, royal-blue cap and base, blue loop handle, and the vertical "NOMAD LABS" branding on each (stays in English)
- The three hand-drawn red marker arrows: same shape, same curve, same position, same stroke weight
- All colors: red marker for the top heading, the "INGYEN" annotation and the big punchline; dark grey/black marker for the bottom line

CHANGE ONLY these handwritten Hungarian strings, replacing them with Czech:
- Top heading (red): "CSALÁDI CSOMAG" becomes "RODINNÝ BALÍČEK"
- Annotation next to the third straw (red): "INGYEN" becomes "ZDARMA"
- Big punchline (red): "2-t veszel = 1 ingyen" becomes "Koupíš 2 = 1 zdarma"
- Bottom line (dark): "Készlet korlátozott" becomes "Zásoby omezené"

TEXT RULES:
- The new text must be written in the SAME casual marker handwriting: same stroke width, same slant, same uneven hand-lettered feel, same size for each block. Keep the top heading in the same rough all-caps hand and the punchline in the same mixed-case hand as the original.
- Render Czech diacritics perfectly and legibly: á é ě í ó ú ů ý č ď ň ř š ť ž. Draw them as handwritten marker strokes. Never drop, flatten or distort an accent.
- Every string stays on one line, centered on the same axis and at the same vertical position as the original. You may slightly adjust letter-spacing or scale so a line fits the same width.
- No printed type, no added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

### Prompt SK

```
Edit the uploaded image. This is a Slovak-market localization of an existing ad creative. Only the handwritten copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image (this is a tall vertical story format)
- Plain white background
- The three Hydra X2 filter straws: identical 3D render, identical positions (two on top, one below centre), identical scale, tilt and spacing, light-blue body, royal-blue cap and base, blue loop handle, and the vertical "NOMAD LABS" branding on each (stays in English)
- The three hand-drawn red marker arrows: same shape, same curve, same position, same stroke weight
- All colors: red marker for the top heading, the free-gift annotation and the big punchline; dark grey/black marker for the bottom line

CHANGE ONLY these handwritten Hungarian strings, replacing them with Slovak:
- Top heading (red): "CSALÁDI CSOMAG" becomes "RODINNÝ BALÍK"
- Annotation next to the third straw (red): "INGYEN" becomes "ZADARMO"
- Big punchline (red): "2-t veszel = 1 ingyen" becomes "Kúpiš 2 = 1 zadarmo"
- Bottom line (dark): "Készlet korlátozott" becomes "Zásoby obmedzené"

TEXT RULES:
- The new text must be written in the SAME casual marker handwriting: same stroke width, same slant, same uneven hand-lettered feel, same size for each block. Keep the top heading in the same rough all-caps hand and the punchline in the same mixed-case hand as the original.
- Render Slovak diacritics perfectly and legibly: á ä é í ó ô ú ý č ď ľ ĺ ň ŕ š ť ž. Draw them as handwritten marker strokes. Never drop, flatten or distort an accent.
- Every string stays on one line, centered on the same axis and at the same vertical position as the original. You may slightly adjust letter-spacing or scale so a line fits the same width.
- No printed type, no added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

---

## Ad 14 — Marker story « 3 achetés = 3 offerts »

| Bloc | FR | CZ | SK |
|---|---|---|---|
| Titre | OFFRE LIMITÉE | LIMITOVANÁ NABÍDKA | LIMITOVANÁ PONUKA |
| Annotation | GRATUIT | ZDARMA | ZADARMO |
| Punchline | Tu en prends 3 = 3 gratuits | Koupíš 3 = 3 zdarma | Kúpiš 3 = 3 zadarmo |
| Bas | Pour toute la famille | Pro celou rodinu | Pre celú rodinu |

### Prompt CZ

```
Edit the uploaded image. This is a Czech-market localization of an existing ad creative. Only the handwritten copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image (this is a tall vertical story format)
- Plain white background
- The two groups of three Hydra X2 filter straws: identical 3D render, identical positions, scale, overlap and spacing, light-blue body, royal-blue cap and base, blue loop handle, and the vertical "NOMAD LABS" branding on each (stays in English)
- The two hand-drawn red marker arrows: same shape, same curve, same position, same stroke weight
- All colors: red marker for the top heading, the "INGYEN" annotation and the big punchline; dark grey/black marker for the bottom line

CHANGE ONLY these handwritten Hungarian strings, replacing them with Czech:
- Top heading (red): "LIMITÁLT AJÁNLAT" becomes "LIMITOVANÁ NABÍDKA"
- Annotation over the right group (red): "INGYEN" becomes "ZDARMA"
- Big punchline (red): "3-at veszel = 3 ingyen" becomes "Koupíš 3 = 3 zdarma"
- Bottom line (dark): "Az egész családnak" becomes "Pro celou rodinu"

TEXT RULES:
- The new text must be written in the SAME casual marker handwriting: same stroke width, same slant, same uneven hand-lettered feel, same size for each block. Keep the top heading and the annotation in the same rough all-caps hand and the bottom line in the same mixed-case hand as the original.
- Render Czech diacritics perfectly and legibly: á é ě í ó ú ů ý č ď ň ř š ť ž. Draw them as handwritten marker strokes. Never drop, flatten or distort an accent.
- Every string stays on one line, at the same position and the same vertical placement as the original. You may slightly adjust letter-spacing or scale so a line fits the same width.
- No printed type, no added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

### Prompt SK

```
Edit the uploaded image. This is a Slovak-market localization of an existing ad creative. Only the handwritten copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, and the original aspect ratio and canvas size of the uploaded image (this is a tall vertical story format)
- Plain white background
- The two groups of three Hydra X2 filter straws: identical 3D render, identical positions, scale, overlap and spacing, light-blue body, royal-blue cap and base, blue loop handle, and the vertical "NOMAD LABS" branding on each (stays in English)
- The two hand-drawn red marker arrows: same shape, same curve, same position, same stroke weight
- All colors: red marker for the top heading, the free-gift annotation and the big punchline; dark grey/black marker for the bottom line

CHANGE ONLY these handwritten Hungarian strings, replacing them with Slovak:
- Top heading (red): "LIMITÁLT AJÁNLAT" becomes "LIMITOVANÁ PONUKA"
- Annotation over the right group (red): "INGYEN" becomes "ZADARMO"
- Big punchline (red): "3-at veszel = 3 ingyen" becomes "Kúpiš 3 = 3 zadarmo"
- Bottom line (dark): "Az egész családnak" becomes "Pre celú rodinu"

TEXT RULES:
- The new text must be written in the SAME casual marker handwriting: same stroke width, same slant, same uneven hand-lettered feel, same size for each block. Keep the top heading and the annotation in the same rough all-caps hand and the bottom line in the same mixed-case hand as the original.
- Render Slovak diacritics perfectly and legibly: á ä é í ó ô ú ý č ď ľ ĺ ň ŕ š ť ž. Draw them as handwritten marker strokes. Never drop, flatten or distort an accent.
- Every string stays on one line, at the same position and the same vertical placement as the original. You may slightly adjust letter-spacing or scale so a line fits the same width.
- No printed type, no added text, no watermark, no logo, no extra graphic element, no visual artifact.
```
