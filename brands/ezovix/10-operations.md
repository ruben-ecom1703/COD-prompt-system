# 10 — Opérations & fonctionnement

> 📅 Dernière mise à jour : 2026-08-30 · Gérant : Hugo
> ⚠️ **Documentation descriptive uniquement** : ce fichier explique le setup et où chaque chose est gérée. Il ne contient **aucun identifiant d'accès, aucun secret, aucune donnée financière** (COGS/marges exclus par décision du 14/07). Il n'implique aucun accès direct aux comptes Meta.

**Ce que contient ce fichier :**
- Qui gère quoi, et sur quels outils
- Le setup publicitaire (compte, pages, état actuel)
- La logistique COD de bout en bout
- Les données volontairement absentes du repo et où les demander

**Sommaire** : [Qui gère quoi](#qui-gère-quoi) · [Setup publicitaire](#setup-publicitaire) · [Logistique COD](#logistique-cod) · [Stack](#stack) · [Ce qui nest pas dans ce repo](#ce-qui-nest-pas-dans-ce-repo)

---

## Qui gère quoi

| Rôle | Qui |
|---|---|
| Gérant de la brand Ezovix (ads, site, data, ce repo) | **Hugo** |
| Contexte portefeuille | Ezovix = une brand du projet COD (Ruben × Hugo × Danila), testée pendant la semaine « 29/06 → 05/07 » |
| Relation partenaire logistique | Danila (pilote), avec Ruben et Hugo |
| Copies intégrales des ads | Notion « #2 Ads Ezovix » (source), miroir complet dans [ads/](ads/) |

## Setup publicitaire

- **Compte publicitaire** (référence des exports) : `CLN_0645-KN-6` (ID `1588269252528563`, owned by **CLNG4**).
  - ⚠️ État au 13/07/2026 : **plafond de dépense atteint** — « Your ads have stopped running — you've reached your ad account spending limit ». À débloquer avant relance ([07-relance.md](07-relance.md) Étape 0).
  - 🔁 **MAJ 29/08** : campagnes relancées par Hugo. Compte désormais rattaché au BM opérationnel **Abu 3** (nouveau BM de Ruben, remplace **Lydia Martinez** restreinte le 26/08). Cet alias correspond à **« COD 3.0 »** sur Kuronet (top-up) — ne pas confondre avec le compte Nuvalis `CLK_1209` (confusion commise puis corrigée le 28-29/08). ⚠️ **Statut plafond non reconfirmé** : au 28/08 le compte affichait $0,00 dépensé sur 30 jours (toutes campagnes Off) — à vérifier après la relance que le plafond n'est plus bloquant.
- **2 pages Facebook persona** (les ads ne partent JAMAIS d'une page « marque ») : Emésztési Egészség Labor `1155025737700054` · Természetes Emésztési Egészség Hálózat `1212951778564210` — détail et règles de voix dans [01-brand.md](01-brand.md#pages-facebook).
- **Setup ad set = par page** : 1 adset Labor + 1 adset Hálózat (campagne « 03/07/26 - Ezovix - Testing », lancée le 04/07).
- **Méthode de suivi de la perf** : exporter depuis Ads Manager (1) l'export créas .xlsx (contient `Link Object ID` = la page FB) et (2) l'export perf .csv — croiser sur **nom d'ad + ad set**. Méthode complète : [06-resultats.md](06-resultats.md#méthode-de-vérification). Exports bruts archivés : [data/exports-meta/](data/exports-meta/).

## Logistique COD

> 👉 Le **parcours client complet** (de l'ad au paiement au livreur) est décrit en 8 étapes dans [09-site-funnel.md § Funnel COD](09-site-funnel.md#funnel-cod). Ci-dessous : le côté partenaire/entrepôt.

Partenaire 3PL officiel du portefeuille (contact : Teodor ; onboarding piloté par Danila) :

- **Hub : Slovaquie 🇸🇰** → livraison **J+1** sur SK/PL/CZ/**HU**. Les compléments alimentaires (comme Ezovix) sont stockés en Slovaquie pour l'expédition internationale.
- **Flux client utánvét** : commande en ligne sur ezovix.shop (aucune carte requise) → expédition annoncée sous 24 h → livraison 48-72 h → **le client paie en liquide au livreur** → le cash est reversé.
- Le réseau du partenaire couvre toute la CEE (entrepôts BG/RO/HR/IT/ES, hub HU en projet) — utile pour l'expansion pays par pays après validation HU.
- ⚠️ Contexte au 13/07 : les ads du portefeuille sont **en pause en attente de stock** — vérifier le stock avant toute relance.

### MAJ 2026-07-15 — packaging & stock

Packaging à refaire avant relance (nouveau design ~mi-semaine, puis production + livraison) → **stock disponible fin août**, calendrier ralenti par le typhon qui touche la Chine.

### 🟠 MAJ 2026-08-06 — couverture estimée à la relance (~01/09)

Approximation construite depuis le tableau transverse stock/couverture des 4 brands du portefeuille (méthode : couverture en unités, jamais en commandes) :

| Stock | Conso estimée | Couverture | Rupture estimée | Date limite commande |
|---|---|---|---|---|
| 3 000 unités (arrivée fin août) | ~65 u/j dès la relance (~01/09), coût/vente winner proche Hepavix | **~46 j** | **~mi-octobre** | seuil de réassort atteint **quasi dès la relance** (début septembre) |

**Verdict : réassort à décider à la relance**, et avant la deadline dure Q4 (commande devant partir avant mi-septembre pour arriver début novembre, lead time ~45 j Chine → Slovaquie). Chiffres à confirmer une fois la relance effective et le vrai rythme de vente mesuré.

## Stack

| Brique | Outil |
|---|---|
| Boutique | Shopify — ezovix.shop |
| Checkout COD | Pop-up add-to-cart → infos → commande (app type « EasyCell » utilisée sur le portefeuille pour maximiser la conversion) |
| Ads | Meta (2 pages persona + compte `CLN_0645`) |
| Copies & production ads | Notion « #2 Ads Ezovix » + ce repo (miroir) |
| Data & décisions | Ce repo (source de synthèse) + exports Meta bruts dans [data/](data/) |
| Contact client | contact@ezovix.shop |

## Ce qui n'est PAS dans ce repo

Volontairement absent — à demander à Hugo si besoin légitime :

- **Unit economics** : COGS, marges, coûts logistiques chiffrés (décision du 14/07 : hors repo)
- **Accès** : identifiants BM/compte pub/Shopify/Notion, données pixel
- **Vidéos HD originales** (versions compressées dans [visuels/videos/](visuels/videos/), originaux chez Hugo)
- **E-books** (fichiers à fournir, cf. [09-site-funnel.md](09-site-funnel.md#e-books))

---

*Navigation : [← 09 — Site & funnel](09-site-funnel.md) · [README (sommaire)](README.md)*
