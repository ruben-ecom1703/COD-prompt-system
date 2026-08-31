# 05 — Inventaire des ads

> 📅 Dernière mise à jour : 2026-07-14 · Gérant : Hugo

**Ce que contient ce fichier :**
- Comment les ads sont organisées et où trouver chaque copy
- La répartition par page Facebook
- Les règles de production

✅ **Les copies intégrales sont dans [ads/](ads/README.md)** — une fiche par ad, avec la **copy hongroise exactement telle qu'elle a été diffusée** (transcrite depuis l'export de créatives Meta) + le diagnostic + le résultat réel. Les 4 ads qui ont vendu ont aussi leur traduction française complète.

**Sommaire** : [Ce qui a été lancé](#ce-qui-a-été-lancé) · [Répartition par page Facebook](#répartition-par-page-facebook) · [Règles de production](#règles-de-production) · [Où sont les briefs dorigine](#où-sont-les-briefs-dorigine)

---

## Ce qui a été lancé

**17 ads**, toutes dans un seul ad set (`Adset 1 - Static/Native`), campagne « 26/06/26 Hepavix », lancée le 27/06/2026.

| Type | Ads |
|---|---|
| **Native ads / advertorials** (récit à la 1re personne) | Ads 2 (winner) · Ads 8 · Ads 12 · Ads 10 · Ads 4 · Ads 14 · Ads 15 (×2) |
| **Statics et ads d'offre** (voix de marque) | Ads 1 · Ads 3 · Ads 5 · Ads 6 · Ads 7 · Ads 9 · Ads 11 |
| **Vidéos** | Ads 16 · Ads 17 |

Le détail ad par ad (spend, ventes, ROAS, page) est dans [ads/README.md](ads/README.md) et [06-resultats.md](06-resultats.md#les-17-ads).

## Répartition par page Facebook

> ✅ **Source de vérité** : les pages ci-dessous sont lues depuis la colonne `Link Object ID` de l'export de créatives Meta — pas depuis une note.

| Page FB | Ads | Logique |
|---|---|---|
| **Dr. Tóth Petra Menopauza szakértő** (`1082894771584939`) | Ads 2 · Ads 7 · Ads 8 · Ads 10 · Ads 16 · Ads 17 | Advertorials d'autorité médicale |
| **Hepavix (page marque)** (`1188936560969417`) | Ads 1 · Ads 3 · Ads 5 · Ads 6 · Ads 9 · Ads 11 | Statics et ads d'offre, sans narrateur |
| **Varga Nóra Szexológus** (`1276839362173620`) | Ads 4 · Ads 12 · Ads 14 · Ads 15 | Récits à la première personne |

⚠️ **Problème connu** : l'advertorial de l'**hôtesse Airbnb** (Ads 12) tourne sur la page de la **sexologue**. Le narrateur ne colle pas à la page — c'est probablement ce qui plombe sa performance ([07-relance.md](07-relance.md)).

## Règles de production

1. 🔴 **Silymarine = 90 %.** Trois copies historiques disent 80 % (dont le winner) → corriger avant toute réutilisation ([03-compliance.md](03-compliance.md#la-règle-du-90--silymarine)).
2. **Disclaimer obligatoire** sur toute native : « Az eredmények egyénenként eltérhetnek. »
3. **Le narrateur doit coller à la page** qui publie. Jamais un advertorial médecin sur la page marque, jamais un static de vente sur une page persona.
4. **Scale du winner : un seul élément à la fois** (le titre, OU le visuel, OU l'ouverture, OU la page). Ne jamais élargir à un autre symptôme.
5. **Le visuel ne montre pas le produit** dans une native ad ([08-brand-system.md](08-brand-system.md#style-visuel-des-créas)).
6. Chaque nouvelle ad = fiche complète (angle · narrateur · persona · format · mécanisme · page · visuel · copy).

## Où sont les briefs d'origine

Les **briefs** (avant lancement) vivent dans Notion, sous la semaine « 22/06/2026 → 28/06/2026 » → page « Ads » (numérotés #1 à #18 + 2 vidéos).

⚠️ **Les numéros Notion (#1…#18) ne correspondent PAS aux noms Meta (Ads 1…Ads 17).** Ce repo utilise les **noms Meta**, parce que ce sont eux qui portent la performance réelle. En cas de doute, la copy de référence est **celle du repo** (= celle qui a réellement tourné), pas celle du brief.

---

*Navigation : [← 04 — Angles & personas](04-angles-personas.md) · [06 — Résultats →](06-resultats.md)*
