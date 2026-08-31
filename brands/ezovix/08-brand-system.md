# 08 — Brand system : code couleur & identité visuelle

> 📅 Dernière mise à jour : 2026-07-14 · Source : site live ezovix.shop (CSS extrait le 14/07) + créas de prod + logos pages FB · Gérant : Hugo

**Ce que contient ce fichier :**
- Le code couleur exact du site (hex, extraits du CSS live)
- Les typographies
- Le style visuel codifié des créas (ce qui vend vs ce qui ne vend pas)
- Le ton de voix hongrois (tegező, vérifié sur le site)
- Les conventions des 2 pages FB et le nommage des fichiers

**Sommaire** : [Code couleur](#code-couleur) · [Typographies](#typographies) · [Style visuel des créas](#style-visuel-des-créas) · [Ton de voix](#ton-de-voix) · [Identité des 2 pages FB](#identité-des-2-pages-fb) · [Nommage des fichiers](#nommage-des-fichiers)

---

## Code couleur

Palette extraite du CSS live de ezovix.shop le 2026-07-14 (fréquence d'usage réelle dans la page) :

| Rôle | Hex | Usage |
|---|---|---|
| **Teal principal** | `#1a8a8f` | Couleur de marque n°1 : logo EZOVIX, titres H1/accents, éléments actifs |
| **Teal foncé** | `#0e5b60` | Titres, bandeau d'urgence header, contrastes |
| **Quasi-noir teal** | `#17282a` | Texte principal |
| **Gris-teal atténué** | `#5c7375` | Texte secondaire |
| **Fond menthe très clair** | `#f5faf9` | Fond de sections |
| **Fonds teal pâles** | `#eaf6f6` · `#e3efee` · `#eef6f5` | Cartes, blocs alternés |
| **Or/ambre CTA** | `#e0a52a` | ⭐ Le bouton « Rendelés » et les CTA — le SEUL accent chaud |
| **Vert validation** | `#2f9e6b` | Badges « LEGNÉPSZERŰBB », checks ✓ |
| **Orange alerte** | `#f97316` | Urgence/stock limité |
| **Jaune étoiles** | `#ffb400` | Notes ★ des avis |

**Logique** : univers **teal médical/apaisant** (confiance, santé digestive) + **un seul accent or** pour l'action. Le produit lui-même (packshot) = boîte **bleu marine/navy** + flacon ambré à pipette noire, badge « NANOTECHNOLÓGIA ».

## Typographies

| Usage | Police |
|---|---|
| Principale (site) | **Plus Jakarta Sans** (fallback : Arial, sans-serif) |
| Secondaire | **Inter** |
| Fallback système | Helvetica Neue |

## Style visuel des créas

Le style codifié par les résultats réels (cf. [06-resultats.md](06-resultats.md#learnings)) :

**✅ CE QUI VEND — le « schéma médical »** :
- Blueprint / plan d'architecte bleu (le winner : coupe gorge + mucus)
- Infographie comparative (« GERD vs LPR : la flamme vs le brouillard »)
- Gravure anatomique ancienne style parchemin (« A Nyákcsapda », reprise du concurrent « THE PHLEGM TRAP »)
- Codes : aspect éducatif/scientifique, curiosité (« curiosity meme »), texte HU intégré au visuel, **heure au format 24 h** si UI/timestamp à l'écran

**❌ CE QUI NE VEND PAS (0 vente, prouvé)** :
- Packshot produit, visuel d'offre/promo, liste d'ingrédients
- Aucun produit, aucun prix, aucun visage dans les visuels gagnants

## Ton de voix

- **Tegező** (tutoiement) partout — vérifié sur le site live : « Kérdéseid, válaszaink », « A kosarad üres », « Válaszd ki a formulád », « kérd ki orvosod véleményét ». **Zéro « Ön »** sur la page.
- Registre : éducatif-rassurant côté site ; récit à la 1re personne côté natives (voix du persona).
- **Jamais le jargon « COD »** face au marché : « **utánvét** » / « fizetés átvételkor ».
- Hedges santé obligatoires — voir [03-compliance.md](03-compliance.md).

## Identité des 2 pages FB

Logos et déclinaisons dans [assets/logos-pages-fb/](assets/logos-pages-fb/) — pour chaque page : logo carré, version cercle transparent, et 4 fonds couleur (navy · sable · teal · vert clair).

| Page | Style | Voix |
|---|---|---|
| Emésztési Egészség Labor | Autorité scientifique (labo/recherche) | Science, mécanisme, reveal médical |
| Természetes Emésztési Egészség Hálózat | Communauté naturelle | Témoignage « je », UGC |

## Nommage des fichiers

Conventions du repo (appliquées et à maintenir) :
- Ads : `ads/NN-slug-descriptif.md` (numéro Notion à 2 chiffres)
- Visuels : `visuels/<angle-persona>/ideeN-description-vN.jpg` (banque) · `visuels/ads-testees/<nom-ad-meta-slugifié>.jpg` (publiés)
- Jamais d'espaces, d'accents ni de **parenthèses** dans les noms de fichiers (les parenthèses cassent les liens markdown GitHub).
- Repos GitHub : préfixe `COD-` (convention portefeuille).

---

*Navigation : [← 07 — Relance](07-relance.md) · [09 — Site & funnel →](09-site-funnel.md)*
