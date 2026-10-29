# Note pour décision : levée de fonds Pop Tables

**Date : 28/10/2026 (soir), recalculée le 29/10/2026** · Fonction : `2 FINANCE` · Destinataire : Direction (@Laetitiarv) · Auteur : assistant IA Finance, à la demande de Vianney (responsable Finance) · Statut : **proposition soumise à décision**. Rien n'est décidé tant que la décision n'est pas inscrite au [[REGISTRE DES DECISIONS]].

La Direction a retenu la première version de cette note le 28/10 au soir (D-23 : tranche 1 d'environ 135 000 €). Le 29/10 au matin, elle a décidé une mise de fonds initiale de 70 000 € en love money (D-26) et demandé à la Finance de recalculer la levée ([[2026 1029 Relevé de décisions du 29 octobre (matin)]], § 4). Cette version fait ce recalcul. Elle tient compte de toutes les décisions D-02 à D-26, notamment :
- D-21 et D-22 : le budget sur 36 mois revu par le responsable Finance est la référence ; privatisation à 500 € TTC par convive, 30 couverts ;
- D-25 : 2 villes en France en novembre 2027, 3 villes à l'étranger en novembre 2028 ;
- D-26 : 70 000 € de mise de fonds initiale en novembre 2026. Le responsable Finance a précisé le 29/10 sa forme : **capital initial de la SAS, apporté à parts égales par les 7 fondateurs (10 000 € chacun), dont 2 fondateurs exécutifs**, et **pas de BSA AIR** dans le financement.

Légende (voir [[RULES]]) : **F** = fait constaté dans un fichier du dépôt ou décision inscrite au registre · **I** = inférence · **P** = proposition · **H** = hypothèse.

> **En bref.**
> - **I** Avec le capital initial de 70 000 €, la trésorerie ne devient jamais négative dans le plan. Son point bas est de **+10 071 € en mars 2027**, et de **+8 271 €** si les coûts des soirées augmentent de 5 %.
> - **P** La tranche 1 décidée le 28/10 (D-23 : environ 135 000 €) peut être ramenée à **environ 70 000 € avant février 2027**, **sans BSA AIR** : 20 000 € de prêt d'honneur, 5 000 € de subvention et **45 000 € de complément à décider** (prêt bancaire ou apport complémentaire des fondateurs). Ce montant ne couvre plus un trou de trésorerie, mais la contingence et une trésorerie de sécurité de 3 mois.
> - **I** Sans levée en fonds propres, les 7 fondateurs gardent tout le capital : 14,3 % chacun, 13,6 % après l'entrée de l'associé gastronomique (5 % proposés).
> - **P** La **tranche 2 reste conditionnelle** (D-23), avec un point de décision en mai 2028. Elle serait d'environ 215 000 € si les privatisations restaient proches de 8 par ville et par an.
> - **I** Le risque principal reste le **volume de privatisations** : 120 en année 2 et 240 en année 3, contre 7 en année 1. Elles font 78 % du chiffre d'affaires des années 2 et 3, et les Ventes ne l'ont pas encore confirmé (D-16).
> - **I** Le plan ne compte pas l'impôt sur les sociétés : environ 175 000 € sur les années 2 et 3 (§ 8).

Fichiers de calcul (versions du 29/10/2026) :
- `2 FINANCE/PREVISIONS/2026 1028 Modèle Pop Tables - Budget sur 36 mois, plan financier, prix et marges.xlsx` (la référence, D-21) ;
- `2 FINANCE/TRESORERIE/2026 1028 Modèle Pop Tables - Trésorerie et mois de survie sur 36 mois.xlsx` ;
- `2 FINANCE/FINANCEMENT/2026 1028 Modèle Pop Tables - Financement et table de capitalisation.xlsx` ;
- `2 FINANCE/PREVISIONS/2026 1029 Pop Tables - Tableau de bord financier.html`.

Les simulations (coûts à +5 %, nombre de privatisations) ont été faites par script sur des copies du modèle. Le fichier du dépôt n'est pas modifié par ces simulations.

---

## 1. Ce qui a changé depuis la première version

| Décision | Effet dans le modèle | Nature |
|---|---|---|
| D-26 : mise de fonds initiale de 70 000 € | Capital initial de 70 000 € en novembre 2026, au lieu de 7 000 € (Budget 36 mois, ligne 78). Le manque d'environ 17 800 € de novembre 2026 (site et matériel payés au départ) disparaît | F pour le montant ; H pour le mois ; forme (capital des 7 fondateurs à parts égales) précisée par le responsable Finance |
| Pas de BSA AIR (responsable Finance, 29/10) | Les 45 000 € de BSA AIR de la tranche 1 deviennent un complément à décider ; la table de capitalisation ne compte que les 7 fondateurs et l'associé gastronomique | Choix du responsable Finance, à inscrire au registre par la Direction (modifie D-23) |
| D-25 : villes 2 et 3 en France, villes 4 à 6 à l'étranger | Lignes 14 à 17 désormais calculées à partir du calendrier des villes. En année 2, les deux nouvelles villes sont françaises : les déplacements de production passent de 11 000 € à 6 600 €. Le résultat de l'année 2 gagne 4 400 € | F |
| D-21 et D-22 | Le budget revu et la privatisation à 30 couverts sont des décisions ; la simulation à 20 couverts de la première version n'a plus lieu d'être | F |

Le reste du budget est inchangé :
- soirée de lancement à 28 000 € et campagne à 10 000 € ;
- site à 15 000 € (D-19) ;
- protection juridique et assurance à 2 % du chiffre d'affaires ;
- licence à 1 000 € ;
- budget des ventes et équipe calculée à partir de l'activité.

**Budget des ventes et de la prospection (H, inchangé).**

| | Année 1 | Année 2 | Année 3 |
|---|---|---|---|
| Outils de prospection (1, 2 puis 3 licences) | 1 200 € | 2 400 € | 3 600 € |
| Rendez-vous et repas de prospection | 3 600 € | 7 200 € | 12 000 € |
| Places offertes aux prescripteurs | 765 € | 2 805 € | 5 610 € |
| Supports commerciaux et salons | 2 500 € | 5 000 € | 8 000 € |
| **Budget des ventes (frais généraux)** | **8 065 €** | **17 405 €** | **29 210 €** |
| Pour mémoire : salaires chargés des 6 commerciaux (année 3) | — | — | 292 320 € |
| Pour mémoire : commissions d'apporteur (5 %, dans les coûts directs) | 9 429 € | 97 741 € | 195 482 € |

**I** L'effort commercial total de l'année 3 atteint environ 517 000 €, soit 12,5 % du chiffre d'affaires. En année 2, aucun commercial n'est payé, alors que les privatisations passent de 7 à 120.

## 2. Résultats (F, calculés par le modèle)

| | Année 1 | Année 2 | Année 3 |
|---|---|---|---|
| Villes actives | 1 (Paris) | 3 (France) | 6 (3 en France, 3 à l'étranger) |
| Soirées (places à l'unité + privatisations) | 16 (9 + 7) | 153 (33 + 120) | 306 (66 + 240) |
| Chiffre d'affaires | 219 643 € | 2 068 750 € | 4 137 500 € |
| Marge sur coûts directs | 57 297 € | 628 857 € | 1 241 214 € |
| Frais généraux | 93 530 € | 236 698 € | 862 357 € |
| dont ressources humaines | — | 97 458 € (3 postes) | 643 837 € (15 postes) |
| **Résultat d'exploitation, avant impôt** | **−36 232 €** | **392 158 €** | **378 857 €** |
| Point mort | 26 soirées | 58 soirées | 213 soirées |
| Trésorerie en fin d'année, avant levée | 54 449 € | 500 793 € | 875 860 € |

- **Point bas de la trésorerie sur 36 mois, avant levée : +10 071 € en mars 2027.** Le capital initial, la TVA et la pré-vente sont compris.
- **I** Pourquoi mars 2027 : la soirée de lancement (28 000 €) et la campagne (5 000 €) tombent ce mois-là. Avant les privatisations de l'année 2, la trésorerie reste mince : entre 10 000 € et 60 000 € de novembre 2026 à octobre 2027.
- **F** Le modèle de trésorerie reprend ces flux et concorde avec le budget sur les 36 mois.

## 3. Avec une hausse de 5 % des coûts de réalisation des soirées (F, simulation)

**H** La hausse s'applique au lieu, au chef, aux matières, aux boissons, à l'équipe, au ménage, à l'assurance de la soirée, au décor, au surcoût des pilotes et aux déplacements de production. Les frais de paiement et les commissions suivent le prix et ne sont pas augmentés.

| | Budget | Coûts des soirées à +5 % |
|---|---|---|
| Marge par soirée : Premier soir / Le Voyage / La Grande Nuit / Privatisation | 2 788 / 2 214 / 4 066 / 4 464 € | 2 418 / 1 711 / 3 406 / 4 051 € |
| Résultat, années 1 / 2 / 3 | −36 232 / 392 158 / 378 857 € | −43 816 / 325 280 / 244 275 € |
| Point mort de l'année 3 | 213 soirées | 239 soirées, pour 306 prévues |
| **Point bas sur 36 mois** | +10 071 € (mars 2027) | **+8 271 € (mars 2027)** |
| Trésorerie en fin d'année 3 | 875 860 € | 665 475 € |

## 4. Ce qui peut faire dérailler le plan : le nombre de privatisations (F, simulation)

Avec les coûts des soirées à +5 % et le capital initial de 70 000 € :

| Privatisations par ville et par an, dès l'année 2 | Résultat, années 2 / 3 | Point bas de la trésorerie | Trésorerie en fin d'année 3 |
|---|---|---|---|
| 40 (budget, D-21) | 325 280 / 244 275 € | +8 271 € (mars 2027) | 665 475 € |
| 20 | 134 957 / −136 371 € | +8 271 € (mars 2027) ; environ +37 000 € en juillet 2029 | 89 966 € |
| 8 (le rythme du plan du 27/10) | −1 248 / −372 096 € | **−284 703 € (octobre 2029)**, et la baisse continue | −284 703 € |

**I** Ce qui pèse le plus, ce sont les frais de l'année 3 : 862 357 €. Ils sont engagés en novembre 2028, avec l'ouverture de 3 villes à l'étranger et 12 postes payés de plus (3 coordinateurs, 6 commerciaux, le manager et 2 fondateurs). Si les privatisations ne suivent pas, c'est cette étape qui crée le besoin de financement.

## 5. Contingence et besoin à financer (P)

La règle reste celle de la première version. Elle s'applique à l'année 1, avant que les privatisations soient prouvées :
- le point bas avec les coûts à +5 % ;
- une contingence sur les coûts ;
- une trésorerie de sécurité.

| Composante | Règle | Montant |
|---|---|---|
| Contingence sur les coûts des soirées | 5 % des coûts directs de l'année 1 (162 345 €) | 8 117 € |
| Contingence sur les frais généraux et les investissements | 10 % de ceux de l'année 1 (93 530 € + 18 000 €) | 11 153 € |
| Trésorerie de sécurité | 3 mois de frais généraux de l'année 2 (236 698 € ÷ 4), quand les 3 coordinateurs sont recrutés et avant que les privatisations soient prouvées | 59 175 € |
| **Réserve à constituer** | | **78 445 €** |
| Moins : trésorerie déjà disponible au point bas (coûts à +5 %, capital initial compris) | Calcul du modèle | −8 271 € |
| **Besoin total à financer** | | **70 174 €, soit environ 70 000 €** |

**I** C'est l'ordre de grandeur annoncé par le relevé du 29/10. Avec un apport de 7 000 €, le même calcul donnait 133 174 €.

## 6. Plan de financement proposé (P)

| Source | Quand | Montant | Statut | Remarque |
|---|---|---|---|---|
| Capital initial de la SAS (D-26) | Novembre 2026, à la création | 70 000 € | Montant décidé (D-26) ; forme choisie par le responsable Finance ; non versé | 7 fondateurs à parts égales : 10 000 € chacun |
| **Tranche 1** | Avant février 2027 | **environ 70 000 €** | Proposition : D-23 (135 000 €, dont 110 000 € de BSA AIR) à modifier par la Direction | Prêt d'honneur 20 000 € (H) ; subvention 5 000 € (H) ; **complément de 45 000 € à décider** : prêt bancaire, ou apport complémentaire des fondateurs (environ 6 400 € chacun). Pas de BSA AIR. Contingence et trésorerie de sécurité |
| **Tranche 2 (conditionnelle, D-23)** | Décision en mai 2028 | 0 € dans le plan | Décidée dans son principe | **I** Si les privatisations restent proches de 8 par ville et par an, il faudrait environ 215 000 € de plus que la tranche 1, avant contingence, ou renoncer à l'expansion de l'année 3. Sans BSA AIR, ce serait une augmentation de capital ou un prêt |
| Associé gastronomique (D-17) | À l'entrée au capital | 0 € de trésorerie | Proposition | Apport en industrie, 5 % proposés |
| **Total** | | **environ 140 000 €**, dont 70 000 € de capital des fondateurs | | |

**Capital (I, modèle Financement).** Sans levée en fonds propres :
- la SAS compte 70 000 actions de 1 €, 10 000 par fondateur, soit 14,3 % chacun ;
- avec l'associé gastronomique à 5 %, chaque fondateur garde 13,6 %.

Deux des 7 fondateurs sont exécutifs. Ce sont les 2 fondateurs rémunérés à partir de novembre 2028 dans le budget ; les 5 autres sont associés sans rémunération.

**I** Points à régler avec le Juridique :
- le pacte d'associés : rôle des fondateurs exécutifs et non exécutifs, sortie d'un associé, actions de l'associé gastronomique acquises par jalons ;
- la libération du capital : en SAS, la moitié des apports en numéraire au moins doit être versée à la création, et le reste dans les 5 ans (règle générale, à confirmer par le Juridique).

## 7. Décisions demandées à la Direction

| # | Décision | Proposition de la Finance |
|---|---|---|
| 1 | Montant de la tranche 1 (modifie D-23) | Environ 70 000 € avant février 2027, sans BSA AIR |
| 2 | Source du complément de 45 000 € | Prêt bancaire, ou apport complémentaire des 7 fondateurs (environ 6 400 € chacun) |
| 2 bis | Forme de la mise de fonds de D-26 | Inscrire au registre : capital initial de 70 000 € de la SAS, 7 fondateurs à parts égales, dont 2 exécutifs ; pas de BSA AIR |
| 3 | Tranche 2 | Point de décision en mai 2028 : ouvrir les villes 4 à 6 et payer les 12 postes ajoutés en novembre 2028 seulement si les privatisations vendues sont proches du plan ; sinon lever environ 215 000 € de plus ou décaler l'expansion |
| 4 | Privatisation à moins de 30 convives (relevé du 29/10, § 3) | **I** Le budget suppose 13 393 € HT par privatisation : un minimum facturé de 30 couverts le garantit ; un forfait devrait être recalibré pour donner le même montant |
| 5 | Volume de privatisations (D-16) | Demander aux Ventes de confirmer 40 par ville et par an dans les 2 villes françaises de l'année 2, et de dire qui les vend avant novembre 2028 |
| 6 | Part de l'associé gastronomique | 5 % avant la levée, acquis par jalons (forme à définir par le Juridique) |
| 7 | Salaires du manager et des fondateurs | Valider 4 000 € brut par mois pour le manager et 2 500 € pour chaque fondateur, en année 3 |

**Préalables inchangés** :
- société créée, statuts et pacte d'associés signés ;
- dépôt passé en privé ;
- licence obtenue (D-09) ;
- coûts des lieux et des chefs confirmés par des devis.

**Rappel (voir [[AGENT]] de la Finance).** Cette note propose un dimensionnement. Elle n'engage personne auprès d'une banque ou d'un investisseur. Un montant demandé n'est pas un montant obtenu.

## 8. Limites du calcul (I)

- **Impôt sur les sociétés non compté.** Ordre de grandeur, au taux réduit de 15 % jusqu'à 42 500 € et au taux normal de 25 % au-delà, après imputation de la perte de l'année 1 : environ 84 700 € au titre de l'année 2 et 90 500 € au titre de l'année 3. Les taux et les conditions du taux réduit sont à confirmer par l'expert-comptable. L'impôt ne change pas le point bas de mars 2027, mais il réduit la trésorerie des années 2 et 3.
- **Logiciels.** Le Marketing estime que 80 € par mois ne suffisent pas pour le site, la billetterie et l'agent conversationnel ([[2026 1029 Note du Marketing à la Finance et au Produit]], § 3). Le montant sera revu avec les devis.
- Les villes ne sont pas nommées. Prix, coûts et TVA y sont supposés identiques à Paris, et le change n'est pas pris en compte.
- Les privatisations sont réparties également sur les 12 mois, août compris. Le Marketing propose un rythme saisonnier si la Côte d'Azur est retenue.
- La TVA sur la pré-vente est comptée le mois de la soirée, pas le mois de l'encaissement.
- Le remboursement du prêt d'honneur, ou d'un éventuel prêt bancaire, n'est pas compté.
- Les délais de paiement des entreprises ne sont pas modélisés : avec 240 privatisations par an, dont une partie en B2B, ils peuvent peser sur la trésorerie.
- Les remboursements en cas de soirée annulée ne sont pas modélisés : la pré-vente est un argent dû tant que la soirée n'a pas eu lieu.
