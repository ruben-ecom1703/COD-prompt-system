# Hepavix — E-mail de livraison des e-books

Rédigé le 2026-08-06, révisé le même jour : **un seul e-mail pour les 2 e-books** (au lieu de la séquence J+0 / J+1 du modèle Aurivo).

---

## 1. Config du flow

**Flow dédié — ne pas greffer sur « Customer Thank You ».**
Le flow Customer Thank You est Live et envoie le remerciement à tous les acheteurs. Y poser un filtre bundle couperait le thank-you aux acheteurs 1 flacon. Créer un flow séparé « Ebooks delivery ».

**Déclencheur** : `Placed Order` (Shopify → Klaviyo)

**Où poser le filtre** : sur le **trigger** (carte `When someone Placed Order` → *Trigger filters*, icône entonnoir), **pas** dans *Profile filters*. Les profile filters regardent l'historique de la personne, pas le contenu de la commande qui déclenche.

**Quel filtre** — dépend de la construction des bundles dans Shopify. Vérifier sur une vraie commande 2+1 dans Shopify Admin :

- **Cas A — la ligne affiche « Hepavix × 3 »** (bundles en quantité) → trigger filter sur le nombre d'articles `≥ 2`. 1 flacon = 1, 2+1 = 3, 3+2 = 5.
- **Cas B — la ligne affiche « Hepavix – 2+1 INGYEN × 1 »** (bundle = une variante unique) → « au moins 2 produits » est faux pour tout le monde, le flow n'enverrait jamais rien. Dans ce cas :
  1. **Sur la variante** (recommandé) : `Items` / `Variant SKU` → `equals any of` → SKU du 2+1 et du 3+2. Immune aux remises et aux frais de port.
  2. **Sur la valeur** (repli) : `$value` `is at least` **17 000**. Le 1 flacon plafonne à 12 400 Ft + port (~14 000 Ft), le premier bundle démarre à 20 900 Ft.

Le cas B est le plus fréquent sur une PDP à 3 paliers → vérifier avant de se reposer sur la quantité.

**Timing** : un seul e-mail, délai **0 min** (immédiat). La PDP promet « E-mailben küldjük a rendelés után, azonnali letöltéssel ».

**Smart Sending : OFF.** C'est une livraison due au client, elle ne doit jamais sauter parce qu'il a reçu une campagne le même jour.

**Hébergement des PDF** : Shopify → Content → Files (URL CDN permanente, pas de login) plutôt que Google Drive — l'e-mail promet que les liens ne périment pas, et un lien Drive casse si le partage change. Placeholders : `{{ LIEN_EBOOK_1 }}` / `{{ LIEN_EBOOK_2 }}`.

---

## 2. Objet — 2 options à tester

**Option A**
```
HU : Itt a 2 ajándék e-könyved – azonnal letöltheted
FR : Voici tes 2 e-books cadeaux – téléchargeables tout de suite
```

**Option B**
```
HU : Megérkeztek az e-könyveid – 2 × 25 oldal, azonnal letölthető
FR : Tes e-books sont arrivés – 2 × 25 pages, téléchargeables tout de suite
```

## 3. Preheader

```
HU : Töltsd le mindkettőt, és kezdd el még a csomagod érkezése előtt.
FR : Télécharge les deux et commence avant même que ton colis arrive.
```

---

## 4. Corps — HONGROIS (version à envoyer)

```
Szia {{ first_name|default:'' }},

Köszönjük a rendelésed – már készítjük a csomagod.

Amíg úton van, itt a két ajándék e-könyved. Mindkettőt azonnal letöltheted:


📗 A májdetox útmutató (25 oldal · 7 fejezet · 9 990 Ft értékben)

• hogyan méregtelenít a májad valójában – a két fázis, és miért nem elég csak „beindítani"
• mi terheli a legjobban: alkohol, cukor és fruktóz, gyógyszerek, stressz, alváshiány
• a túlterhelt máj jelei – és azok a tünetek, amelyeknél nem detox kell, hanem orvos
• a májbarát tányér: mit egyél, és mit érdemes kerülnöd
• szilimarin, NAC, kolin – mit csinál pontosan a három kulcstápanyag
• a 14 napos májtámogató terv, lépésről lépésre

>> ELSŐ E-KÖNYV LETÖLTÉSE <<
{{ LIEN_EBOOK_1 }}


📙 Energia és emésztés természetesen (25 oldal · 7 fejezet · 6 990 Ft értékben)

• miért hullámzik az energiád – a vércukor-hullámvasút, és hogyan simítsd el
• a rejtett energiaszívók: kiszáradás, túl sok koffein, alváshiány, stressz, túlterhelt máj
• az emésztés útja a szájtól a bélig – és a puffadás négy leggyakoribb oka
• a tányér képlete: fehérje + rost + jó zsír, és miért számít az evés sorrendje
• a bélflóra: mivel táplálod a jó baktériumokat (pre- és probiotikum)
• a 7 napos energiaterv, napi egy lépéssel

>> MÁSODIK E-KÖNYV LETÖLTÉSE <<
{{ LIEN_EBOOK_2 }}


A linkek nem járnak le, bármikor visszatérhetsz rájuk.

Egy tipp: mindkét útmutató végén van egy terv – 14 napos az elsőben, 7 napos a másodikban. Ne próbáld egyszerre bevezetni az összes lépést. Válassz egyet, tartsd egy hétig, és csak utána tegyél hozzá egy másikat. Így marad meg.

És amit érdemes már most tudnod: a Hepavix ajánlott adagja napi 2 kapszula, étkezés közben. A legtöbb visszajelzés szerint a különbség a 2–3. héten kezd érezhetővé válni. Ezért adunk 60 nap pénzvisszafizetési garanciát – üres üveggel is.

Ha bármi kérdésed van, válaszolj erre az e-mailre – olvassuk.

Üdv,
a Hepavix csapata
```

## 5. Corps — FRANÇAIS (contrôle, ne pas envoyer)

```
Salut {{ first_name }},

Merci pour ta commande – on prépare déjà ton colis.

En attendant qu'il arrive, voici tes deux e-books cadeaux. Tu peux télécharger les deux tout de suite :


📗 Le guide de la détox du foie (25 pages · 7 chapitres · d'une valeur de 9 990 Ft)

• comment ton foie détoxifie vraiment – les deux phases, et pourquoi il ne suffit pas de « lancer » la détox
• ce qui le charge le plus : alcool, sucre et fructose, médicaments, stress, manque de sommeil
• les signes d'un foie surchargé – et les symptômes qui relèvent du médecin, pas d'une détox
• l'assiette amie du foie : ce qu'il faut manger, et ce qu'il vaut mieux éviter
• silymarine, NAC, choline – ce que font exactement les trois nutriments clés
• le plan de soutien du foie en 14 jours, étape par étape

>> TÉLÉCHARGER LE PREMIER E-BOOK <<
{{ LIEN_EBOOK_1 }}


📙 Énergie et digestion naturellement (25 pages · 7 chapitres · d'une valeur de 6 990 Ft)

• pourquoi ton énergie fait des vagues – les montagnes russes de la glycémie, et comment les lisser
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

## 6. QA du build Klaviyo (2026-08-06)

E-mail HU monté dans Klaviyo et prévisualisé dans Gmail. Objet retenu : `Itt a 2 ajándék e-könyved` (variante courte de l'option A). Correctifs relevés avant passage Live :

1. **Footer d'unsubscribe en anglais** — à traduire : *« Ezt az e-mailt a Hepavix küldte neked. / Ha nem szeretnél több e-mailt kapni, itt iratkozhatsz le. »*
2. **« Szia Berecz »** — Berecz est un nom de famille. En hongrois l'ordre est nom-prénom, donc `first_name` récupère souvent le patronyme. Soit vérifier le mapping Shopify → Klaviyo sur plusieurs commandes réelles, soit mettre `Szia,` sans variable. **Règle à retenir pour toutes les marques HU.**
3. **Badge Klaviyo** en pied de mail (plan gratuit) — à retirer.
4. ~~CTA en liens texte à remplacer par des boutons~~ — **arbitré : on garde les liens texte.** Sur un e-mail de livraison post-achat l'intention de clic est maximale, ce n'est pas un e-mail de conversion, et le lien texte passe souvent mieux en délivrabilité. Seul ajustement : retirer l'italique et passer en gras plus gros, pour la zone de tap sur mobile.
5. **Interligne des bullets** trop large (une puce = un paragraphe) — à resserrer.
6. **Preheader** : champ « Preview text » séparé dans Klaviyo, à remplir.
7. Vérifier que les deux boutons pointent bien vers **deux PDF différents**.

## 7. À trancher / vérifier

- **Construction des bundles** dans Shopify (cas A ou B ci-dessus) + SKU exacts des variantes 2+1 et 3+2.
- ✅ **Bullets vérifiées contre les PDF réels (2026-08-06).** 3 erreurs corrigées dans la version initiale : « l'alcool n'est pas en tête de liste » (faux — le chapitre 2 ouvre sur l'alcool), « les 30 premiers jours » (le plan fait 14 jours), et « comment intégrer les 2 gélules » (absent de l'ebook 2). Leçon : ne jamais écrire les bullets d'un lead magnet depuis le positionnement de la PDP — toujours attendre le fichier.
