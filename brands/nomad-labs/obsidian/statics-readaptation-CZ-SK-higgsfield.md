# Statiques Nomad Labs — réadaptation CZ / SK (prompts Higgsfield)

Workflow : Ruben upload l'image de la statique HU source dans Higgsfield + colle le prompt correspondant.
Niveau d'adaptation retenu : **traduction + localisation légère** (texte + devise). Casting, décor, packaging, composition, palette, typo, layout = strictement identiques à la source.
Prompts rédigés en anglais, textes cibles cités en dur.

## Grille de prix validée (source : expansion-sk-cz-strategy.md + research-sk-cz-expansion.md)

| Marché | Prix barré (3×) | Bundle 2+1 | À l'unité | Remise |
|---|---|---|---|---|
| HU (source) | 52 200 Ft | 29 900 Ft | 17 400 Ft | −43 % |
| **CZ** | 3 270 Kč | **1 860 Kč** | 1 090 Kč | −43 % |
| **SK** | 135 € | **77 €** | 45 € | −43 % |

Le « −43 % » reste valable tel quel sur les deux marchés — aucun recalcul du chiffre affiché.
Référence prix concurrent (ad 4, « 80 000 Ft-os víztisztító ») → **5 000 Kč** (CZ) / **200 €** (SK).

Liens produit :
- CZ → `https://cz.nomadlabs.shop/products/hydra-x2-survival-filtracni-brcko-na-vodu-pro-400-litru-pitne-vody`
- SK → `https://sk.nomadlabs.shop/products/hydra-x2-slamka-na-prezitie-s-vodnym-filtrom-na-400-litrov-pitnej-vody`

---

## Batch 1 — 5 statiques (2026-08-13)

### Ad 1 — Offre « −43 % Pack Famille » (fond navy, rayons, 3 pailles)

| Bloc | FR | CZ | SK |
|---|---|---|---|
| Titre 2 | PACK FAMILLE | RODINNÝ BALÍČEK | RODINNÝ BALÍK |
| Bas | L'OFFRE EXPIRE CE SOIR ! | NABÍDKA KONČÍ DNES VEČER! | PONUKA KONČÍ DNES VEČER! |

#### Prompt CZ

```
Edit the uploaded image. This is a Czech-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, 4:5 vertical aspect ratio
- Dark navy/near-black background with the radial light-burst rays and blue glow
- The three Hydra X2 filter straws: identical 3D render, identical position, scale, tilt, spacing, light-blue body, royal-blue cap and base, blue loop handle, and the vertical "NOMAD LABS" branding printed on each straw (stays in English)
- The "NOMAD LABS" wordmark at the top (stays in English, unchanged)
- All colors: bright orange for "-43%", warm off-white for the other headline text
- Typography: same heavy condensed all-caps sans-serif, same weights, same centering, same size hierarchy, same vertical position of each text block

CHANGE ONLY these Hungarian strings, replacing them with Czech:
- "CSALÁDI CSOMAG" becomes "RODINNÝ BALÍČEK"
- "AZ AJÁNLAT MA ESTE LEJÁR!" becomes "NABÍDKA KONČÍ DNES VEČER!"
- "-43%" stays exactly "-43%"

TEXT RULES:
- Render Czech diacritics perfectly and legibly: á é ě í ó ú ů ý č ď ň ř š ť ž. Never drop, flatten or distort an accent.
- Keep each replaced string on the same number of lines as the original and centered on the same axis. You may slightly adjust letter-spacing or horizontal scale so the line spans the same width as the original, but do not change the typeface, the weight, or the block's vertical position.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

#### Prompt SK

```
Edit the uploaded image. This is a Slovak-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, 4:5 vertical aspect ratio
- Dark navy/near-black background with the radial light-burst rays and blue glow
- The three Hydra X2 filter straws: identical 3D render, identical position, scale, tilt, spacing, light-blue body, royal-blue cap and base, blue loop handle, and the vertical "NOMAD LABS" branding printed on each straw (stays in English)
- The "NOMAD LABS" wordmark at the top (stays in English, unchanged)
- All colors: bright orange for "-43%", warm off-white for the other headline text
- Typography: same heavy condensed all-caps sans-serif, same weights, same centering, same size hierarchy, same vertical position of each text block

CHANGE ONLY these Hungarian strings, replacing them with Slovak:
- "CSALÁDI CSOMAG" becomes "RODINNÝ BALÍK"
- "AZ AJÁNLAT MA ESTE LEJÁR!" becomes "PONUKA KONČÍ DNES VEČER!"
- "-43%" stays exactly "-43%"

TEXT RULES:
- Render Slovak diacritics perfectly and legibly: á ä é í ó ô ú ý č ď ľ ĺ ň ŕ š ť ž. Never drop, flatten or distort an accent.
- Keep each replaced string on the same number of lines as the original and centered on the same axis. You may slightly adjust letter-spacing or horizontal scale so the line spans the same width as the original, but do not change the typeface, the weight, or the block's vertical position.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

---

### Ad 2 — Grille 4 panneaux « coupure de courant »

| Bloc | FR | CZ | SK |
|---|---|---|---|
| Titre | QUAND LE COURANT S'ARRÊTE / TON EAU S'ARRÊTE AUSSI | KDYŽ VYPADNE PROUD / VYPADNE I VAŠE VODA | KEĎ VYPADNE PRÚD / VYPADNE AJ VAŠA VODA |
| Panneau 1 | EAU DU ROBINET | VODA Z KOHOUTKU | VODA Z KOHÚTIKA |
| Panneau 2 | 6 HEURES | 6 HODIN | 6 HODÍN |
| Panneau 3 | 48 HEURES | 48 HODIN | 48 HODÍN |
| Panneau 4 | HYDRA X2 | HYDRA X2 | HYDRA X2 |

#### Prompt CZ

```
Edit the uploaded image. This is a Czech-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, 4:5 vertical aspect ratio
- Cream / off-white background
- The 2x2 grid of four rounded photo panels: same photos, same crops, same rounded corners, same gaps, same positions. Do not regenerate, re-light or re-render the kitchen scenes, the stainless faucet, the glasses, or the water inside them. The progression must stay identical: clear tap water, faintly cloudy water, heavily brown sediment-filled water, and clean filtered water with the small Hydra X2 straw lying beside the glass.
- The large Hydra X2 filter straw on the right: identical 3D render, position, scale, light-blue body, royal-blue cap and base, blue loop handle, and vertical "NOMAD LABS" branding (stays in English)
- The small "NOMAD LABS" text printed on the straw inside panel 4 (stays in English)
- Typography: same heavy black all-caps sans-serif for the headline, same smaller bold all-caps for the four panel labels, same near-black color, same alignment and same vertical position for every text block

CHANGE ONLY these Hungarian strings, replacing them with Czech:
- Headline line 1: "AMIKOR LEÁLL AZ ÁRAM" becomes "KDYŽ VYPADNE PROUD"
- Headline line 2: "A VIZED IS LEÁLL" becomes "VYPADNE I VAŠE VODA"
- Panel label: "CSAPVÍZ" becomes "VODA Z KOHOUTKU"
- Panel label: "6 ÓRA" becomes "6 HODIN"
- Panel label: "48 ÓRA" becomes "48 HODIN"
- Panel label: "HYDRA X2" stays exactly "HYDRA X2"

TEXT RULES:
- Render Czech diacritics perfectly and legibly: á é ě í ó ú ů ý č ď ň ř š ť ž. Never drop, flatten or distort an accent.
- The headline must stay on exactly two centered lines. Each panel label stays on one line, left-aligned above its panel exactly as in the original. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

#### Prompt SK

```
Edit the uploaded image. This is a Slovak-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, 4:5 vertical aspect ratio
- Cream / off-white background
- The 2x2 grid of four rounded photo panels: same photos, same crops, same rounded corners, same gaps, same positions. Do not regenerate, re-light or re-render the kitchen scenes, the stainless faucet, the glasses, or the water inside them. The progression must stay identical: clear tap water, faintly cloudy water, heavily brown sediment-filled water, and clean filtered water with the small Hydra X2 straw lying beside the glass.
- The large Hydra X2 filter straw on the right: identical 3D render, position, scale, light-blue body, royal-blue cap and base, blue loop handle, and vertical "NOMAD LABS" branding (stays in English)
- The small "NOMAD LABS" text printed on the straw inside panel 4 (stays in English)
- Typography: same heavy black all-caps sans-serif for the headline, same smaller bold all-caps for the four panel labels, same near-black color, same alignment and same vertical position for every text block

CHANGE ONLY these Hungarian strings, replacing them with Slovak:
- Headline line 1: "AMIKOR LEÁLL AZ ÁRAM" becomes "KEĎ VYPADNE PRÚD"
- Headline line 2: "A VIZED IS LEÁLL" becomes "VYPADNE AJ VAŠA VODA"
- Panel label: "CSAPVÍZ" becomes "VODA Z KOHÚTIKA"
- Panel label: "6 ÓRA" becomes "6 HODÍN"
- Panel label: "48 ÓRA" becomes "48 HODÍN"
- Panel label: "HYDRA X2" stays exactly "HYDRA X2"

TEXT RULES:
- Render Slovak diacritics perfectly and legibly: á ä é í ó ô ú ý č ď ľ ĺ ň ŕ š ť ž. Never drop, flatten or distort an accent.
- The headline must stay on exactly two centered lines. Each panel label stays on one line, left-aligned above its panel exactly as in the original. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

---

### Ad 3 — Fiche mécanisme « fonctionne sans piles ? »

| Bloc | FR | CZ | SK |
|---|---|---|---|
| Titre | ÇA MARCHE SANS PILES ? | FUNGUJE BEZ BATERIÍ? | FUNGUJE BEZ BATÉRIÍ? |
| Corps | LE NOMAD LABS HYDRA X2 UTILISE UNE MEMBRANE À FIBRES CREUSES — LES PORES FILTRENT PAR GRAVITÉ ET PAR ASPIRATION, SANS SOURCE D'ÉNERGIE. | NOMAD LABS HYDRA X2 POUŽÍVÁ MEMBRÁNU S DUTÝMI VLÁKNY — PÓRY FILTRUJÍ GRAVITACÍ A SÁNÍM, BEZ ZDROJE ENERGIE. | NOMAD LABS HYDRA X2 POUŽÍVA MEMBRÁNU S DUTÝMI VLÁKNAMI — PÓRY FILTRUJÚ GRAVITÁCIOU A SANÍM, BEZ ZDROJA ENERGIE. |
| Icône 1 | Bloque tout au-dessus de 0,1 micron | Blokuje vše nad 0,1 mikronu | Blokuje všetko nad 0,1 mikrónu |
| Icône 2 | Qualité militaire / Testé en laboratoire | Vojenská kvalita / Laboratorně testováno | Vojenská kvalita / Laboratórne testované |
| Icône 3 | 400 litres par filtre / Pas de date de péremption | 400 litrů na filtr / Bez data spotřeby | 400 litrov na filter / Bez dátumu spotreby |
| Icône 4 | Rivière, lac, pluie, baignoire | Řeka, jezero, déšť, vana | Rieka, jazero, dážď, vaňa |

#### Prompt CZ

```
Edit the uploaded image. This is a Czech-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, 4:5 vertical aspect ratio
- Cream / off-white background
- The central Hydra X2 filter straw: identical 3D render, position, scale, vertical orientation, light-blue body, royal-blue cap and base, blue loop handle, and vertical "NOMAD LABS" branding (stays in English)
- The still-life arrangement around the straw: same white and grey pebbles, same green moss, same green and brown autumn leaves, same water splash, same soft shadows. Do not regenerate or reposition any of it.
- The four thin-line blue circular icons (microscope, shield, water drop, mountains): identical style, stroke weight, size and position
- Typography: same heavy black all-caps sans-serif for the headline, same medium all-caps for the body paragraph, same bold sentence-case for the four icon captions, same near-black color, same alignment and same vertical position for every text block

CHANGE ONLY these Hungarian strings, replacing them with Czech:
- Headline: "ELEM NÉLKÜL MŰKÖDIK?" becomes "FUNGUJE BEZ BATERIÍ?"
- Body paragraph: "A NOMAD LABS HYDRA X2 ÜREGES SZÁLAS MEMBRÁNT HASZNÁL — A PÓRUSOK GRAVITÁCIÓVAL ÉS SZÍVÁSSAL SZŰRNEK, ENERGIAFORRÁS NÉLKÜL." becomes "NOMAD LABS HYDRA X2 POUŽÍVÁ MEMBRÁNU S DUTÝMI VLÁKNY — PÓRY FILTRUJÍ GRAVITACÍ A SÁNÍM, BEZ ZDROJE ENERGIE."
- Top-left caption: "Mindent blokkol / 0,1 mikron felett" becomes "Blokuje vše / nad 0,1 mikronu"
- Top-right caption: "Katonai minőség / Laborban tesztelt" becomes "Vojenská kvalita / Laboratorně testováno"
- Bottom-left caption: "400 liter szűrőnként / Nincs lejárati idő" becomes "400 litrů na filtr / Bez data spotřeby"
- Bottom-right caption: "Folyó, tó, eső / fürdőkád" becomes "Řeka, jezero, / déšť, vana"
- "NOMAD LABS" and "HYDRA X2" stay in English everywhere they appear

TEXT RULES:
- Render Czech diacritics perfectly and legibly: á é ě í ó ú ů ý č ď ň ř š ť ž. Never drop, flatten or distort an accent.
- Write the decimal as "0,1" with a comma, never "0.1".
- The headline stays on one centered line. The body paragraph stays on exactly three centered lines. Each icon caption stays on exactly two centered lines. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

#### Prompt SK

```
Edit the uploaded image. This is a Slovak-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, 4:5 vertical aspect ratio
- Cream / off-white background
- The central Hydra X2 filter straw: identical 3D render, position, scale, vertical orientation, light-blue body, royal-blue cap and base, blue loop handle, and vertical "NOMAD LABS" branding (stays in English)
- The still-life arrangement around the straw: same white and grey pebbles, same green moss, same green and brown autumn leaves, same water splash, same soft shadows. Do not regenerate or reposition any of it.
- The four thin-line blue circular icons (microscope, shield, water drop, mountains): identical style, stroke weight, size and position
- Typography: same heavy black all-caps sans-serif for the headline, same medium all-caps for the body paragraph, same bold sentence-case for the four icon captions, same near-black color, same alignment and same vertical position for every text block

CHANGE ONLY these Hungarian strings, replacing them with Slovak:
- Headline: "ELEM NÉLKÜL MŰKÖDIK?" becomes "FUNGUJE BEZ BATÉRIÍ?"
- Body paragraph: "A NOMAD LABS HYDRA X2 ÜREGES SZÁLAS MEMBRÁNT HASZNÁL — A PÓRUSOK GRAVITÁCIÓVAL ÉS SZÍVÁSSAL SZŰRNEK, ENERGIAFORRÁS NÉLKÜL." becomes "NOMAD LABS HYDRA X2 POUŽÍVA MEMBRÁNU S DUTÝMI VLÁKNAMI — PÓRY FILTRUJÚ GRAVITÁCIOU A SANÍM, BEZ ZDROJA ENERGIE."
- Top-left caption: "Mindent blokkol / 0,1 mikron felett" becomes "Blokuje všetko / nad 0,1 mikrónu"
- Top-right caption: "Katonai minőség / Laborban tesztelt" becomes "Vojenská kvalita / Laboratórne testované"
- Bottom-left caption: "400 liter szűrőnként / Nincs lejárati idő" becomes "400 litrov na filter / Bez dátumu spotreby"
- Bottom-right caption: "Folyó, tó, eső / fürdőkád" becomes "Rieka, jazero, / dážď, vaňa"
- "NOMAD LABS" and "HYDRA X2" stay in English everywhere they appear

TEXT RULES:
- Render Slovak diacritics perfectly and legibly: á ä é í ó ô ú ý č ď ľ ĺ ň ŕ š ť ž. Never drop, flatten or distort an accent.
- Write the decimal as "0,1" with a comma, never "0.1".
- The headline stays on one centered line. The body paragraph stays on exactly three centered lines. Each icon caption stays on exactly two centered lines. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

---

### Ad 4 — Comparatif prix « pas un purificateur à 80 000 Ft »

| Bloc | FR | CZ | SK |
|---|---|---|---|
| Titre | CE N'EST PAS UN PURIFICATEUR D'EAU À 80 000 Ft. | NENÍ TO ČISTIČKA VODY ZA 5 000 Kč. | NIE JE TO ČISTIČKA VODY ZA 200 €. |
| Sous-titre | Juste un filtre de poche qui bloque tout au-dessus de 0,1 micron. | Jen kapesní filtr, který blokuje vše nad 0,1 mikronu. | Len vreckový filter, ktorý blokuje všetko nad 0,1 mikrónu. |
| Prix | 52 200 Ft barré → 29 900 Ft | 3 270 Kč → 1 860 Kč | 135 € → 77 € |
| Ligne pack | Pack famille 2+1 / Ou 17 400 Ft l'unité | Rodinný balíček 2+1 / Nebo 1 090 Kč za kus | Rodinný balík 2+1 / Alebo 45 € za kus |
| Bandeau bas | 52 200 Ft BARRÉ. 29 900 Ft CETTE SEMAINE. | 3 270 Kč PŘEŠKRTNUTO. 1 860 Kč TENTO TÝDEN. | 135 € PREŠKRTNUTÉ. 77 € TENTO TÝŽDEŇ. |

**Point ouvert** — le bandeau du bas de la créa HU dit littéralement « 52 200 Ft *barré*. 29 900 Ft cette semaine. », le mot « barré » étant écrit dans le texte. Traduit fidèlement (règle : structure source à 100 %). Variante propre disponible si Ruben la valide : « 3 270 Kč → 1 860 Kč TENTO TÝDEN. » / « 135 € → 77 € TENTO TÝŽDEŇ. »

#### Prompt CZ

```
Edit the uploaded image. This is a Czech-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, 4:5 vertical aspect ratio
- Cream / off-white background and the thin horizontal divider line above the bottom bar
- The Hydra X2 filter straw on the right: identical 3D render, position, scale, vertical orientation, light-blue body, royal-blue cap and base, blue loop handle, and vertical "NOMAD LABS" branding (stays in English)
- The hand-drawn red diagonal strikethrough over the old price in the main price row, and the second red strikethrough over the old price in the bottom bar: same red color, same angle, same rough hand-drawn stroke
- Typography: same heavy black all-caps condensed sans-serif for the headline, same regular sentence-case for the sub-line, same bold condensed for the prices, same small regular for the pack lines, same heavy all-caps for the bottom bar, same near-black color, same left alignment and same vertical position for every text block

CHANGE ONLY these Hungarian strings, replacing them with Czech and converting the currency to Czech koruna:
- Headline: "NEM EGY / 80 000 Ft-OS / VÍZTISZTÍTÓ." becomes "NENÍ TO / ČISTIČKA VODY / ZA 5 000 Kč."
- Sub-line: "Csak egy zsebszűrő, ami mindent blokkol 0,1 mikron felett." becomes "Jen kapesní filtr, který blokuje vše nad 0,1 mikronu."
- Struck-through price: "52 200 Ft" becomes "3 270 Kč"
- Sale price: "29 900 Ft" becomes "1 860 Kč"
- Pack line 1: "Családi csomag 2+1" becomes "Rodinný balíček 2+1"
- Pack line 2: "Vagy 17 400 Ft darabonként" becomes "Nebo 1 090 Kč za kus"
- Bottom bar: "52 200 Ft ÁTHÚZVA. 29 900 Ft EZEN A HÉTEN." becomes "3 270 Kč PŘEŠKRTNUTO. 1 860 Kč TENTO TÝDEN."

TEXT RULES:
- Render Czech diacritics perfectly and legibly: á é ě í ó ú ů ý č ď ň ř š ť ž. Never drop, flatten or distort an accent.
- Format prices Czech style: a non-breaking thin space as thousands separator and "Kč" after the number, e.g. "3 270 Kč", "1 860 Kč", "5 000 Kč", "1 090 Kč". Write the decimal as "0,1" with a comma, never "0.1".
- The headline stays on exactly three left-aligned lines. The sub-line stays on exactly three lines. The pack block stays on exactly two lines. The bottom bar stays on one centered line. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- The red strikethroughs must land precisely over the new struck prices, at the same angle and thickness as the original.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

#### Prompt SK

```
Edit the uploaded image. This is a Slovak-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, 4:5 vertical aspect ratio
- Cream / off-white background and the thin horizontal divider line above the bottom bar
- The Hydra X2 filter straw on the right: identical 3D render, position, scale, vertical orientation, light-blue body, royal-blue cap and base, blue loop handle, and vertical "NOMAD LABS" branding (stays in English)
- The hand-drawn red diagonal strikethrough over the old price in the main price row, and the second red strikethrough over the old price in the bottom bar: same red color, same angle, same rough hand-drawn stroke
- Typography: same heavy black all-caps condensed sans-serif for the headline, same regular sentence-case for the sub-line, same bold condensed for the prices, same small regular for the pack lines, same heavy all-caps for the bottom bar, same near-black color, same left alignment and same vertical position for every text block

CHANGE ONLY these Hungarian strings, replacing them with Slovak and converting the currency to euro:
- Headline: "NEM EGY / 80 000 Ft-OS / VÍZTISZTÍTÓ." becomes "NIE JE TO / ČISTIČKA VODY / ZA 200 €."
- Sub-line: "Csak egy zsebszűrő, ami mindent blokkol 0,1 mikron felett." becomes "Len vreckový filter, ktorý blokuje všetko nad 0,1 mikrónu."
- Struck-through price: "52 200 Ft" becomes "135 €"
- Sale price: "29 900 Ft" becomes "77 €"
- Pack line 1: "Családi csomag 2+1" becomes "Rodinný balík 2+1"
- Pack line 2: "Vagy 17 400 Ft darabonként" becomes "Alebo 45 € za kus"
- Bottom bar: "52 200 Ft ÁTHÚZVA. 29 900 Ft EZEN A HÉTEN." becomes "135 € PREŠKRTNUTÉ. 77 € TENTO TÝŽDEŇ."

TEXT RULES:
- Render Slovak diacritics perfectly and legibly: á ä é í ó ô ú ý č ď ľ ĺ ň ŕ š ť ž. Never drop, flatten or distort an accent.
- Format prices Slovak style: the euro sign after the number with a space, e.g. "135 €", "77 €", "200 €", "45 €". Write the decimal as "0,1" with a comma, never "0.1".
- The headline stays on exactly three left-aligned lines. The sub-line stays on exactly three lines. The pack block stays on exactly two lines. The bottom bar stays on one centered line. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- The red strikethroughs must land precisely over the new struck prices, at the same angle and thickness as the original.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

---

### Ad 5 — Storyboard illustré « les voisins demandent mon secret »

| Bloc | FR | CZ | SK |
|---|---|---|---|
| Titre script | Oh là là, les voisins | Jejda, sousedé | Jaj, susedia |
| Titre gras | DEMANDENT MON SECRET... | SE PTAJÍ NA MÉ TAJEMSTVÍ... | SA PÝTAJÚ NA MOJE TAJOMSTVO... |
| Panneaux | JOUR 1 / JOUR 3 / JOUR 7 | 1. DEN / 3. DEN / 7. DEN | 1. DEŇ / 3. DEŇ / 7. DEŇ |
| Carte | OFFRE SPÉCIALE | SPECIÁLNÍ NABÍDKA | ŠPECIÁLNA PONUKA |
| Prix | 52 200 Ft barré → 29 900 Ft | 3 270 Kč → 1 860 Kč | 135 € → 77 € |
| Ruban | LA PLUS GROSSE OFFRE DE L'ANNÉE | NEJVĚTŠÍ NABÍDKA ROKU | NAJVÄČŠIA PONUKA ROKA |

#### Prompt CZ

```
Edit the uploaded image. This is a Czech-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, 4:5 vertical aspect ratio
- Cream / off-white background
- The three rounded illustrated story panels: identical 3D-cartoon rendering style, identical characters (elderly couple, children, middle-aged men, the family drinking from bottles), identical suburban houses, gardens, fences, sky and lighting, identical panel order and mood progression (sunny day, grey overcast day with the hose and worried faces, sunny day with shocked neighbours). Do not regenerate, restyle, reframe or repopulate any panel.
- The three Hydra X2 filter straws at the bottom left: identical cut-out render, position, tilt, scale, light-blue body, royal-blue cap and base, blue loop handle, and the vertical "NOMAD LABS" branding on each (stays in English)
- The white rounded price card and the gold ribbon banner below it: same shapes, same shadows, same gold gradient, same positions
- Typography: same brown handwritten script font for the small top line, same heavy dark-brown all-caps sans-serif for the big headline, same bold all-caps for the day labels, same small bold all-caps for the card's top line, same grey struck price, same large blue sale price, same white all-caps on the gold ribbon
- All colors unchanged: dark brown headline, blue sale price, gold ribbon, grey old price

CHANGE ONLY these Hungarian strings, replacing them with Czech and converting the currency to Czech koruna:
- Script line: "Jajj, a szomszédok" becomes "Jejda, sousedé"
- Headline: "KÉRDEZIK A TITKOMAT..." becomes "SE PTAJÍ NA MÉ TAJEMSTVÍ..."
- Panel labels: "1. NAP" becomes "1. DEN", "3. NAP" becomes "3. DEN", "7. NAP" becomes "7. DEN"
- Card top line: "KÜLÖNLEGES AJÁNLAT" becomes "SPECIÁLNÍ NABÍDKA"
- Struck-through price: "52 200 Ft" becomes "3 270 Kč"
- Sale price: "29 900 Ft" becomes "1 860 Kč"
- Gold ribbon: "AZ ÉV LEGNAGYOBB AJÁNLATA" becomes "NEJVĚTŠÍ NABÍDKA ROKU"

TEXT RULES:
- Render Czech diacritics perfectly and legibly: á é ě í ó ú ů ý č ď ň ř š ť ž. Never drop, flatten or distort an accent. This applies to the handwritten script line too.
- Format prices Czech style: a thin space as thousands separator and "Kč" after the number, e.g. "3 270 Kč", "1 860 Kč".
- Keep the strikethrough line over the old price at the same position, thickness and angle.
- The headline stays on one centered line, the script line on one centered line above it. Each day label stays on one line, centered above its panel. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

#### Prompt SK

```
Edit the uploaded image. This is a Slovak-market localization of an existing ad creative. Only the on-image copy changes.

PRESERVE EXACTLY — do not alter in any way:
- Layout, composition, framing, 4:5 vertical aspect ratio
- Cream / off-white background
- The three rounded illustrated story panels: identical 3D-cartoon rendering style, identical characters (elderly couple, children, middle-aged men, the family drinking from bottles), identical suburban houses, gardens, fences, sky and lighting, identical panel order and mood progression (sunny day, grey overcast day with the hose and worried faces, sunny day with shocked neighbours). Do not regenerate, restyle, reframe or repopulate any panel.
- The three Hydra X2 filter straws at the bottom left: identical cut-out render, position, tilt, scale, light-blue body, royal-blue cap and base, blue loop handle, and the vertical "NOMAD LABS" branding on each (stays in English)
- The white rounded price card and the gold ribbon banner below it: same shapes, same shadows, same gold gradient, same positions
- Typography: same brown handwritten script font for the small top line, same heavy dark-brown all-caps sans-serif for the big headline, same bold all-caps for the day labels, same small bold all-caps for the card's top line, same grey struck price, same large blue sale price, same white all-caps on the gold ribbon
- All colors unchanged: dark brown headline, blue sale price, gold ribbon, grey old price

CHANGE ONLY these Hungarian strings, replacing them with Slovak and converting the currency to euro:
- Script line: "Jajj, a szomszédok" becomes "Jaj, susedia"
- Headline: "KÉRDEZIK A TITKOMAT..." becomes "SA PÝTAJÚ NA MOJE TAJOMSTVO..."
- Panel labels: "1. NAP" becomes "1. DEŇ", "3. NAP" becomes "3. DEŇ", "7. NAP" becomes "7. DEŇ"
- Card top line: "KÜLÖNLEGES AJÁNLAT" becomes "ŠPECIÁLNA PONUKA"
- Struck-through price: "52 200 Ft" becomes "135 €"
- Sale price: "29 900 Ft" becomes "77 €"
- Gold ribbon: "AZ ÉV LEGNAGYOBB AJÁNLATA" becomes "NAJVÄČŠIA PONUKA ROKA"

TEXT RULES:
- Render Slovak diacritics perfectly and legibly: á ä é í ó ô ú ý č ď ľ ĺ ň ŕ š ť ž. Never drop, flatten or distort an accent. This applies to the handwritten script line too.
- Format prices Slovak style: the euro sign after the number with a space, e.g. "135 €", "77 €".
- Keep the strikethrough line over the old price at the same position, thickness and angle.
- The headline stays on one centered line, the script line on one centered line above it. Each day label stays on one line, centered above its panel. You may slightly adjust letter-spacing or horizontal scale so a line fits the same width, but do not change the typeface, the weight, or the block's vertical position.
- No added text, no watermark, no logo, no extra graphic element, no visual artifact.
```

---

## Points de vigilance en production

1. **Les diacritiques sont le point de casse.** `ř`, `ě`, `ů` (CZ) et `ô`, `ľ`, `ä` (SK) sont les caractères les plus souvent ratés par les modèles image. Vérifier mot par mot au rendu, surtout sur l'ad 5 (police script manuscrite = la plus fragile).
2. **L'ad 5 est la plus risquée.** Trois panneaux illustrés avec personnages : le modèle a tendance à régénérer les scènes au lieu de se limiter au texte. En cas de dégradation, faire un second passage en réuploadant le résultat et en ne demandant que le bloc de texte fautif.
3. **Cohérence 400 L** : l'ad 3 dit bien « 400 liter szűrőnként » → conservé en 400 litrů / 400 litrov. Ne jamais laisser passer un 1500 L.
