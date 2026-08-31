# compliance — Nomad Labs

> 📅 Dernière mise à jour : 2026-07-15 · Gérant : Ruben

## Claims produit — chiffres canoniques (vérifiés page produit, à ne jamais changer sans revérifier le site)

| Claim | Valeur exacte | Source |
|---|---|---|
| Capacité filtre | **400 litres** par filtre | Page produit — jamais 1500L ni "plus d'un an d'eau potable" (voir incident ci-dessous) |
| Filtration bactéries | "99,999999%" | Page produit + FAQ |
| Filtration parasites/microplastiques | "99,999%" | FAQ |
| Membrane | 0,1 micron | Page produit |
| Alimentation | Sans électricité, sans produit chimique | Page produit |
| Péremption | Aucune si stocké sec | FAQ |
| Garantie | 90 jours, remboursement intégral sans question | Page produit + FAQ |

## ⚠️ Incident de cohérence corrigé (2026-07-15)

D'anciens scripts d'ads utilisaient **1500L / "plus d'un an d'eau potable"**, en contradiction avec la page produit (400L). Corrigé le 2026-07-15 — tous les scripts doivent désormais utiliser **400L**. De même, "60 grammes" et "paille en acier" ont été retirés de scripts en cours car non vérifiés contre la fiche produit réelle.

**Règle à appliquer systématiquement** : avant de valider tout nouveau script/copy, vérifier chaque chiffre produit contre [01-brand.md](01-brand.md) / la page produit live. Une incohérence vérifiable par un spectateur détruit la crédibilité (et peut constituer une publicité trompeuse).

## Zones sensibles santé / claims à manier avec précaution

- **Filtration bactéries/parasites** : toujours citer le pourcentage exact ("99,999999%"), ne jamais dire "élimine 100%" ou "élimine tout"
- **Utilisation enfants** : la FAQ mentionne un usage "dès environ 5 ans avec assistance" — ne pas en faire un argument marketing sans cette nuance
- **Ne pas présenter le produit comme un substitut total et sans réserve à l'eau traitée municipale** — formuler en "solution d'appoint / de secours", pas en remplacement médical généralisé

## Claims à haut risque identifiés dans les scripts en développement

- **"Autorité militaire"** (script court #1 "Ce que les militaires savent", claim "unités opérationnelles militaires US") : affiliation/adoption militaire **non vérifiée/non sourcée** dans nos documents. Risque de claim trompeur (endorsement implicite non prouvé) si présenté comme un fait plutôt qu'une comparaison. À valider avant diffusion — vérifier s'il existe une preuve réelle (contrat, certification) ou reformuler en registre plus prudent.
- **Anti-contrefaçon / "uniquement disponible sur le site officiel"** : acceptable si vrai, mais ne pas sur-jouer la peur de la contrefaçon sans base factuelle.
- **Scripts narratifs façon "actualité"** (angle László, cascade géopolitique/crise eau) : le script est un **récit fictif à la 1ère personne** ("mon voisin m'a confié que..."), pas une annonce factuelle. Point de vigilance : formulé tel quel ("La Hongrie va connaître sa plus grosse crise d'eau potable"), la phrase peut se lire comme une affirmation factuelle plutôt qu'un ressenti narratif — à garder clairement dans le registre du témoignage/récit, jamais présenté comme une info vérifiée, pour rester dans les règles pub Meta (pas de désinformation, pas de fear-mongering non qualifié).

## Règles de production (visuel/IA)

- Si le rendu B-Roll IA est identifiable comme IA → rejet du plan, à refaire
- Mix obligatoire B-Roll IA + vrais B-Roll pour les séquences d'actualité (ex : Texas 2021, Espagne/Portugal) — ces références doivent être des images réelles, pas générées

## Mots/éléments à éviter (règle générale)

- Tout chiffre produit non recoupé avec [01-brand.md](01-brand.md)
- "Élimine 100%" / "garanti sans risque à 100%"
- Affirmation d'un partenariat ou d'une adoption militaire officielle sans preuve
- Formulations d'actualité/crise présentées comme un fait vérifié plutôt qu'un récit

---
Sources : page produit live (fetch 2026-07-15), notes de session Ruben du 2026-07-15 ([source complète](data/notes-sessions/2026-07-15-session-scripts-video.md))
