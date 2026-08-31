# Hepavix SK — E-mail de livraison des e-books (version slovaque)

Rédigé le 2026-08-06. Adaptation de `flow-emails-ebooks.md` (version HU) au marché slovaque.

## Décisions prises

- **Registre : tykanie** (tutoiement), pour rester aligné sur le tegező hongrois et sur le reste de COD Empire. Le vykanie se défendrait sur une cible santé 55+ en Slovaquie — bascule possible si Ruben le demande.
- **Devise : EUR.** Valeurs perçues converties sur ~395 HUF/EUR puis arrondies en prix marketing : 9 990 Ft → **24,90 €**, 6 990 Ft → **17,90 €**. À caler sur la vraie PDP SK quand elle existe.
- Config Klaviyo identique à la version HU (trigger `Placed Order`, trigger filter sur les SKU bundles, délai 0 min, Smart Sending OFF). Si le store SK est un Shopify séparé → flow distinct dans le compte SK. Si store unique multi-marchés → ajouter une condition de langue/pays au trigger filter et dupliquer la branche.

## ⚠️ Bloquants avant envoi

1. **Les 2 PDF n'existent qu'en hongrois.** L'e-mail SK annonce « 25 strán · 7 kapitol » et livrerait un fichier hongrois. Faire traduire les 2 ebooks en slovaque avant de brancher le flow.
2. **Pricing SK non connu** — les valeurs 24,90 € / 17,90 € sont des conversions, pas des prix vérifiés sur une PDP SK.

---

## Objet — 2 options

**Option A**
```
SK : Tu sú tvoje 2 darčekové e-knihy – stiahni si ich hneď
FR : Voici tes 2 e-books cadeaux – télécharge-les tout de suite
```

**Option B**
```
SK : Tvoje e-knihy dorazili – 2 × 25 strán, na okamžité stiahnutie
FR : Tes e-books sont arrivés – 2 × 25 pages, téléchargement immédiat
```

## Preheader

```
SK : Stiahni si obe a začni ešte predtým, než ti dorazí balík.
FR : Télécharge les deux et commence avant même que ton colis arrive.
```

---

## Corps — SLOVAQUE (version à envoyer)

```
Ahoj {{ first_name|default:'' }},

Ďakujeme za tvoju objednávku – už ti pripravujeme balík.

Kým je na ceste, tu sú tvoje dve darčekové e-knihy. Obe si môžeš stiahnuť hneď teraz:


📗 Sprievodca detoxikáciou pečene (25 strán · 7 kapitol · v hodnote 24,90 €)

• ako tvoja pečeň v skutočnosti detoxikuje – dve fázy a prečo nestačí detox len „naštartovať"
• čo ju zaťažuje najviac: alkohol, cukor a fruktóza, lieky, stres, nedostatok spánku
• príznaky preťaženej pečene – a tie, pri ktorých nepotrebuješ detox, ale lekára
• tanier pre zdravú pečeň: čo jesť a čomu sa radšej vyhnúť
• silymarín, NAC, cholín – čo presne robia tri kľúčové živiny
• 14-dňový plán podpory pečene, krok za krokom

>> STIAHNUŤ PRVÚ E-KNIHU <<
{{ LIEN_EBOOK_1 }}


📙 Energia a trávenie prirodzene (25 strán · 7 kapitol · v hodnote 17,90 €)

• prečo tvoja energia kolíše – horská dráha krvného cukru a ako ju vyrovnať
• skrytí zlodeji energie: dehydratácia, priveľa kofeínu, málo spánku, stres, preťažená pečeň
• cesta trávenia od úst po črevá – a štyri najčastejšie príčiny nadúvania
• vzorec taniera: bielkoviny + vláknina + zdravý tuk, a prečo záleží na poradí jedla
• črevná mikroflóra: čím kŕmiť dobré baktérie (pre- a probiotiká)
• 7-dňový energetický plán, jeden krok denne

>> STIAHNUŤ DRUHÚ E-KNIHU <<
{{ LIEN_EBOOK_2 }}


Odkazy nevypršia, môžeš sa k nim kedykoľvek vrátiť.

Jeden tip: na konci každého sprievodcu nájdeš plán – 14-dňový v prvom, 7-dňový v druhom. Neskúšaj zaviesť všetky kroky naraz. Vyber si jeden, drž sa ho týždeň, a až potom pridaj ďalší. Takto ti to vydrží.

A ešte niečo, čo je dobré vedieť už teraz: odporúčaná dávka Hepavixu sú 2 kapsuly denne, počas jedla. Podľa väčšiny ohlasov sa rozdiel začína prejavovať v 2. – 3. týždni. Preto dávame 60 dní záruku vrátenia peňazí – aj s prázdnymi fľaštičkami.

Ak máš akúkoľvek otázku, odpovedz na tento e-mail – čítame ich.

S pozdravom,
tím Hepavix
```

## Corps — FRANÇAIS (contrôle, ne pas envoyer)

```
Salut {{ first_name }},

Merci pour ta commande – on prépare déjà ton colis.

En attendant qu'il arrive, voici tes deux e-books cadeaux. Tu peux télécharger les deux tout de suite :


📗 Le guide de la détox du foie (25 pages · 7 chapitres · d'une valeur de 24,90 €)

• comment ton foie détoxifie vraiment – les deux phases, et pourquoi il ne suffit pas de « lancer » la détox
• ce qui le charge le plus : alcool, sucre et fructose, médicaments, stress, manque de sommeil
• les signes d'un foie surchargé – et ceux pour lesquels il te faut un médecin, pas une détox
• l'assiette amie du foie : ce qu'il faut manger, et ce qu'il vaut mieux éviter
• silymarine, NAC, choline – ce que font exactement les trois nutriments clés
• le plan de soutien du foie en 14 jours, étape par étape

>> TÉLÉCHARGER LE PREMIER E-BOOK <<
{{ LIEN_EBOOK_1 }}


📙 Énergie et digestion naturellement (25 pages · 7 chapitres · d'une valeur de 17,90 €)

• pourquoi ton énergie fluctue – les montagnes russes de la glycémie, et comment les lisser
• les voleurs d'énergie cachés : déshydratation, excès de caféine, manque de sommeil, stress, foie surchargé
• le trajet de la digestion, de la bouche à l'intestin – et les quatre causes les plus fréquentes des ballonnements
• la formule de l'assiette : protéines + fibres + bon gras, et pourquoi l'ordre des aliments compte
• le microbiote : avec quoi nourrir les bonnes bactéries (pré- et probiotiques)
• le plan énergie en 7 jours, une étape par jour

>> TÉLÉCHARGER LE DEUXIÈME E-BOOK <<
{{ LIEN_EBOOK_2 }}


Les liens n'expirent pas, tu peux y revenir quand tu veux.

Un conseil : chaque guide se termine par un plan – 14 jours pour le premier, 7 jours pour le second. N'essaie pas d'appliquer toutes les étapes d'un coup. Prends-en une, tiens-la une semaine, et ajoutes-en une autre seulement après. C'est comme ça que ça tient.

Et une chose à savoir dès maintenant : la dose recommandée de Hepavix est de 2 gélules par jour, pendant un repas. D'après la plupart des retours, la différence commence à se sentir à la 2e–3e semaine. C'est pour ça qu'on donne 60 jours de garantie satisfait ou remboursé – même avec les flacons vides.

Si tu as la moindre question, réponds directement à cet e-mail – on les lit.

À bientôt,
l'équipe Hepavix
```

---

## Mapping HU → SK

| HU | SK |
|---|---|
| Szia | Ahoj |
| A májdetox útmutató | Sprievodca detoxikáciou pečene |
| Energia és emésztés természetesen | Energia a trávenie prirodzene |
| 25 oldal · 7 fejezet | 25 strán · 7 kapitol |
| 9 990 Ft / 6 990 Ft értékben | v hodnote 24,90 € / 17,90 € |
| szilimarin, NAC, kolin | silymarín, NAC, cholín |
| vércukor-hullámvasút | horská dráha krvného cukru |
| bélflóra | črevná mikroflóra |
| napi 2 kapszula, étkezés közben | 2 kapsuly denne, počas jedla |
| 60 napos pénzvisszafizetési garancia | 60 dní záruka vrátenia peňazí |
| üres üveggel is | aj s prázdnymi fľaštičkami |
| a Hepavix csapata | tím Hepavix |
