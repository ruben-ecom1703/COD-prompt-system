# Onela — Configuration CommentGuard

Rédigée le 2026-08-06. Sources : repo `COD-Agency-Data-brand/COD-onela` (01-brand, 04-angles-personas, 09-site-funnel) + PDP live `onela.shop` + config Hepavix comme base.

⚠️ **Pages Facebook non documentées** dans le repo Onela (contrairement à Hepavix). À récupérer auprès de Ruben pour ajouter les topics spécifiques à la page.

## Ce qui change par rapport à Hepavix

1. **Le tag hostile est le risque n°1.** Sur une ad d'haleine, le réflexe est de taguer un proche pour se moquer. → **Hide mentions ON** (l'inverse d'Hepavix, où le tag est de la portée gratuite).
2. **Ne pas masquer les gens qui racontent leur problème.** « nekem is ez volt 10 évig » est le commentaire qui convertit le mieux. `Hide negativity` va vouloir le masquer → ouvrir ses *Advanced settings* et activer la prise en compte du contexte de page.
3. **Registre tegező** pour les auto-réponses (site et FAQ tutoient, cible 25-45) — l'inverse d'Hepavix qui est en magázó.

---

## 1. Tous les toggles

| Toggle | État visé |
|---|---|
| Hide profanity | ON |
| Hide negativity | ON + *Advanced settings* → activer le contexte de page |
| Hide custom topics | ON (les 18 ci-dessous) |
| Hide impersonators | ON |
| Hide URL's | ON |
| Hide emails and phone numbers | ON |
| **Hide mentions** | **ON** ← spécifique Onela |
| Hide hashtags | ON |
| Hide images | ON (les commentaires en image sont des mèmes de moquerie) |
| Hide emojis | OFF |
| Hide keywords | ON + liste ci-dessous |
| Hide all comments | OFF |
| Apply moderation to | **ON → Both** |
| Delete comments | OFF (hide seulement) |
| Whitelist | OFF |

---

## 1bis. Textarea sous Hide negativity

Champ « Provide additional moderation rules, examples, or edge cases » :

```
E-commerce Facebook page in Hungary advertising ONELA+, a chlorophyll, mint and parsley capsule that neutralises bad breath and body odour from inside the digestive system. Ads are often illustrated cartoons. Payment is cash on delivery (utánvét). Onela is a dietary supplement, not a medicine. Hide comments that: question product claims, doubt the product, imply misleading advertising, OR use sarcasm, irony or mockery about the marketing, the cartoon format or the selling tactics — even if they don't directly insult the product. Also hide any comment that mocks, jokes about or insults people with bad breath or body odour, any comment tagging another person as a joke, comments saying it is enough to brush your teeth or see a dentist, comments claiming chlorophyll does nothing or that this is pseudoscience, and comments recommending mouthwash, chewing gum, a tongue scraper or simply eating parsley. Examples of comments to hide: "Nice marketing lol", "Classic dropshipping ad", "Who falls for this?", "Just brush your teeth 😂", "@Peti this is for you", "Chlorophyll is a scam", "Eat parsley, same thing". A mocking tone about how the product is marketed is negative even without explicit insults.

Keep visible: genuine questions about price, ordering, delivery, payment or dosage, and above all people describing their own problem or their own results — comments like "I suffered from this for 10 years" are the ones that convert, even though they sound negative.
```

⚠️ Le dernier paragraphe est le plus important de la config Onela. Sans lui, `Hide negativity` masque les meilleurs témoignages, qui sont tous formulés négativement.

## 2. Custom topics (18, tous sous 100 caractères)

```
Comments mocking, joking about or insulting people with bad breath or body odor.
Comments tagging another person as a joke or to humiliate them.
Comments saying it is enough to brush your teeth, use mouthwash or see a dentist.
Comments claiming chlorophyll does nothing or that this is pseudoscience.
Comments recommending mouthwash, gum, a tongue scraper or just eating parsley.
Comments accusing the brand of being a scam, a fraud, a fake shop or a rip-off.
Comments warning others not to buy, or telling people to avoid this brand.
Comments claiming the product does not work, is useless, or is only a placebo.
Comments saying the package never arrived or that cash on delivery is a trick.
Comments claiming the reviews, the rating or the testimonials are fake.
Comments claiming the dietitian or the expert in the post is invented.
Comments pointing out contradictions between the ad and the website figures.
Comments saying bad breath is a sign of a serious illness and needs a doctor.
Comments giving medical diagnoses or naming diseases to other commenters.
Comments claiming the text, photos or video are AI-generated.
Comments pointing out this is an ad, or mocking the cartoon format and marketing.
Comments accusing the brand of hiding or deleting negative comments.
Off-topic comments: politics, religion, spam or unrelated personal messages.
```

Les 3 topics spécifiques à Onela :
- **« brush your teeth / see a dentist »** — objection n°1 sur ce produit, elle attaque le mécanisme même que la marque vend (le problème ne vient pas de la bouche).
- **« just eating parsley »** — le produit *est* du persil et de la chlorophylle, quelqu'un fera le calcul à voix haute.
- **« contradictions between the ad and the website figures »** — certaines ads affichent 15 000 elégedett ügyfél, le site affiche 2 147 értékelés (écart documenté dans `09-site-funnel.md`).

---

## 3. Hide keywords

```
átverés · átvert · átvertek · átverős · csalás · csaló · csalók · kamu · kamubolt
lehúzás · lehúzós · szélhámos · hazugság · hazudik · hamis · sarlatán · kuruzslás
áltudomány · placebo · becsapás · becsaptak · ne vegyétek · ne rendeljetek
ne dőljetek be · vigyázzatok · feljelentés · fogyasztóvédelem · ügyvéd
dropshipping · Temu · AliExpress · Wish
```

⚠️ **À ne PAS mettre sur Onela** : `büdös`, `bűzös`, `undorító`, `szájszag`, `lehelet`, `fehér lepedék`. Ce sont les mots de la moquerie **et** ceux des meilleurs témoignages. Un filtre par mot-clé ne distingue pas les deux — la moquerie doit passer par les custom topics, qui lisent le contexte.

⚠️ Rappel valable sur toutes les marques HU : ne jamais mettre `csal` seul, ça matche `család` (famille).

---

## 4. Auto-réponses (hongrois, tegező)

**Achat / prix**
```
Köszönjük az érdeklődést! Az Onela a hivatalos oldalunkon rendelhető: onela.shop
Utánvéttel fizetsz, közvetlenül a futárnál — nincs szükség online fizetésre.
A legnépszerűbb a 2+1 csomag: ingyenes szállítás, 24-48 órás kézbesítés.
```

**Posologie**
```
Naponta 1 kapszula reggel, lehetőleg reggeli előtt. Erős szag esetén este egy második.
A napi 2 kapszulát ne lépd túl.
```

**Délai de résultat**
```
A legtöbben már az első héten éreznek különbséget. A rendszeres kúra adja a tartós eredményt.
```

**Garantie**
```
30 napos pénzvisszafizetési garanciát adunk. Ha nem válik be, visszaküldöd és visszakapod az árat — feltétel és indoklás nélkül.
```

**Végan / gluten**
```
Igen — 100% vegán, gluténmentes és állatkísérlet-mentes.
```

**Réponse de sécurité (symptôme persistant)**
```
Az Onela étrend-kiegészítő, nem gyógyszer. Ha a panasz tartósan fennáll, érdemes fogorvossal vagy orvossal is megvizsgáltatni.
```

---

## 5. Chiffres à verrouiller

| ✅ Toujours | ❌ Jamais |
|---|---|
| 30 napos garancia | 60 ou 90 jours (autres marques du portefeuille) |
| 4,8/5 · 2 147 értékelés | 15 000 elégedett ügyfél |
| napi 1 kapszula, max 2 | 2/jour en dose standard |
| 10 400 / 18 900 / 25 900 Ft | tout autre prix |
| utánvét | « COD » |
| étrend-kiegészítő | gyógyszer |

---

## 6. Playground — test de validation

```
Ez kamu, a klorofill semmit nem csinál. Mosd meg a fogad!
@Peti neked kéne ez 😂
11 évig szenvedtem a szájszagtól, ez az egyetlen ami segített
Hol lehet megrendelni és mennyibe kerül?
```

Les deux premières doivent être masquées, **les deux dernières doivent passer**. Si la troisième est masquée → `Hide negativity` trop agressif, retourner dans ses Advanced settings.

---

## 7. Reste à faire

- Récupérer les **IDs des pages Facebook** Onela pour ajouter d'éventuels topics de page.
- Prochaine marque à configurer : **Nuvalis** (repo `COD-nuvalis` pas encore fouillé).
