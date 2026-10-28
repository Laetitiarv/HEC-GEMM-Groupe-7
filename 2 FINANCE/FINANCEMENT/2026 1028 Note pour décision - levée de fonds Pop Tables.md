# Note pour décision : levée de fonds Pop Tables

**Date : 28/10/2026 (soir)** · Fonction : `2 FINANCE` · Destinataire : Direction (@Laetitiarv) · Auteur : assistant IA Finance, à la demande de Vianney (responsable Finance) · Statut : **proposition soumise à décision**. Rien n'est décidé tant que la décision n'est pas inscrite au [[REGISTRE DES DECISIONS]].

Cette note remplace la note pour décision du 28/10/2026 (après-midi), rangée dans `2 FINANCE/OLD/`. Elle repose sur le **budget sur 36 mois revu par le responsable Finance le 28/10/2026 (soir)**, qui fait référence. Elle tient compte :
- des décisions D-02 à D-20 de la Direction ([[2026 1028 Relevé de décisions du 28 octobre (soir)]], [[REGISTRE DES DECISIONS]]) ;
- des choix du responsable Finance : campagne de lancement de 10 000 €, protection juridique et assurance de la société à 2 % du chiffre d'affaires, budget des ventes et de la prospection, 40 privatisations par ville et par an dès l'année 2, équipe calculée à partir de l'activité, nouvelles villes actives dès novembre.

Légende (voir [[RULES]]) : **F** = fait constaté dans un fichier du dépôt ou décision inscrite au registre · **I** = inférence · **P** = proposition · **H** = hypothèse.

> **En bref.**
> - **P** Lever environ **135 000 € avant février 2027** : 20 000 € de prêt d'honneur, 5 000 € de subvention et **110 000 € de BSA AIR**.
> - **P** Prévoir une **tranche 2 conditionnelle**, à décider en mai 2028 au vu des privatisations réellement vendues. Elle n'est pas nécessaire dans le plan.
> - **I** Dans le budget revu, la société consomme de la trésorerie pendant l'année 1 seulement. Le point bas est de **−52 929 € en mars 2027** (−54 729 € si les coûts des soirées augmentent de 5 %). La trésorerie redevient positive en novembre 2027.
> - **I** Ce résultat repose sur **deux hypothèses fragiles** :
>   - **120 privatisations en année 2 et 240 en année 3**, contre 7 en année 1. Elles font 78 % du chiffre d'affaires des années 2 et 3, et les Ventes ne les ont pas encore confirmées (D-16) ;
>   - **une privatisation à 30 couverts**, alors que la décision D-05 en fixe 20. À 20 couverts, l'année 3 perd 216 858 € et la trésorerie descend à −137 660 €.
> - **I** Le plan ne compte pas l'impôt sur les sociétés : environ 174 000 € sur les années 2 et 3 (§ 8).

Fichiers de calcul (versions du 28/10/2026, soir) :
- `2 FINANCE/PREVISIONS/2026 1028 Modèle Pop Tables - Budget sur 36 mois, plan financier, prix et marges.xlsx` (la référence) ;
- `2 FINANCE/TRESORERIE/2026 1028 Modèle Pop Tables - Trésorerie et mois de survie sur 36 mois.xlsx` ;
- `2 FINANCE/FINANCEMENT/2026 1028 Modèle Pop Tables - Financement et table de capitalisation.xlsx`.

Les simulations (coûts à +5 %, nombre de privatisations, jauge de 20 couverts) ont été faites par script sur des copies du modèle. Le fichier du dépôt n'est pas modifié.

---

## 1. Ce qui change dans le budget revu

| Poste | Budget revu | Avant la revue | Nature |
|---|---|---|---|
| Villes | Paris, puis 3 villes dès novembre 2027, puis 6 dès novembre 2028 (D-15) | Villes 2 à 6 ouvertes entre janvier 2028 et juin 2029 | F pour le nombre, H pour les mois |
| Ouverture d'une ville | 15 000 € en France comme à l'étranger, sur les 3 mois qui précèdent : 30 000 € en année 1, 45 000 € en année 2 | 8 000 € en France, 15 000 € à l'étranger | H |
| Privatisations (D-16) | 7 en année 1, puis 40 par ville active et par an : 120, puis 240. Pas de déplacement de production pour les privatisations hors Paris | 7, 24 puis 48 | H, à caler avec les Ventes |
| Privatisation : prix et jauge | 500 € TTC par convive, 30 couverts : 13 393 € HT de CA et 4 464 € de marge par soirée | Forfait de 6 000 € + 300 € par convive, 20 couverts | P (Produit) pour le prix ; **la jauge de 30 couverts s'écarte de D-05 (20 couverts)** |
| Lieu | 1 000 € pour toutes les offres | 1 500 à 2 500 € | H |
| Coûts de La Grande Nuit | Chef 3 500 €, matières 90 € et vins 60 € par convive | Chef 3 700 €, matières 100 €, vins 66 € | H |
| Commission d'apporteur | 5 % (Le Voyage, La Grande Nuit, privatisation) | 10 % | H |
| Coordinateurs d'événements | 1 par événement hebdomadaire, dès novembre 2027 : 3, puis 6 | 1 dès novembre 2027 | H (règle du responsable Finance) |
| Commerciaux | 1 par ville active, dès novembre 2028 : 6 | 1 dès novembre 2028 | H (règle du responsable Finance) |
| Manager | 1 dès novembre 2028, 4 000 € brut par mois | — | H, salaire à valider par la Direction |
| Locaux et logiciels | 300 € de coworking par poste payé ; 80 € de socle et 50 € par poste | Montants forfaitaires | H |
| Places offertes aux prescripteurs | 1 par soirée « place à l'unité » | 2 | H |

Postes inchangés : soirée de lancement de 28 000 € en mars 2027 (D-14, montant H), campagne de lancement de 10 000 €, site de 15 000 € (D-19), protection juridique et assurance à 2 % du CA, licence de 1 000 € (D-09), pré-vente le mois qui précède la soirée (D-04), associé gastronomique en apport en industrie (D-17).

**Budget des ventes et de la prospection (H).**

| | Année 1 | Année 2 | Année 3 |
|---|---|---|---|
| Outils de prospection (1, 2 puis 3 licences) | 1 200 € | 2 400 € | 3 600 € |
| Rendez-vous et repas de prospection | 3 600 € | 7 200 € | 12 000 € |
| Places offertes aux prescripteurs | 765 € | 2 805 € | 5 610 € |
| Supports commerciaux et salons | 2 500 € | 5 000 € | 8 000 € |
| **Budget des ventes (frais généraux)** | **8 065 €** | **17 405 €** | **29 210 €** |
| Pour mémoire : salaires chargés des 6 commerciaux (année 3) | — | — | 292 320 € |
| Pour mémoire : commissions d'apporteur (5 %, dans les coûts directs) | 9 429 € | 97 741 € | 195 482 € |

**I** L'effort commercial total de l'année 3 atteint environ 517 000 €, soit 12,5 % du chiffre d'affaires. **I** En année 2, aucun commercial n'est payé, alors que les privatisations passent de 7 à 120. Qui les vend ?

## 2. Résultats du budget revu (F, calculés par le modèle)

| | Année 1 | Année 2 | Année 3 |
|---|---|---|---|
| Villes actives | 1 | 3 | 6 |
| Soirées (places à l'unité + privatisations) | 16 (9 + 7) | 153 (33 + 120) | 306 (66 + 240) |
| Chiffre d'affaires | 219 643 € | 2 068 750 € | 4 137 500 € |
| dont privatisations | 93 750 € | 1 607 143 € | 3 214 286 € |
| Marge sur coûts directs | 57 297 € | 624 457 € | 1 241 214 € |
| Frais généraux | 93 530 € | 236 698 € | 862 357 € |
| dont ressources humaines | — | 97 458 € (3 postes) | 643 837 € (15 postes) |
| **Résultat d'exploitation, avant impôt** | **−36 232 €** | **387 758 €** | **378 857 €** |
| Point mort | 26 soirées | 58 soirées | 213 soirées |
| Trésorerie en fin d'année, avant levée | −8 551 € | 433 353 € | 808 460 € |

- **Point bas de la trésorerie sur 36 mois, avant levée : −52 929 € en mars 2027.** L'apport de 7 000 €, la TVA et la pré-vente sont compris.
- **I** Pourquoi mars 2027 : la soirée de lancement (28 000 €) et la campagne (5 000 €) tombent ce mois-là. La trésorerie reste négative jusqu'en octobre 2027, puis devient positive en novembre 2027 avec les 10 privatisations par mois de l'année 2.
- **F** Le modèle de trésorerie reprend ces flux et concorde avec le budget sur les 36 mois.

## 3. Avec une hausse de 5 % des coûts de réalisation des soirées (F, simulation)

**H** La hausse s'applique au lieu, au chef, aux matières, aux boissons, à l'équipe, au ménage, à l'assurance de la soirée, au décor, au surcoût des pilotes et aux déplacements de production. Les frais de paiement et les commissions suivent le prix et ne sont pas augmentés.

| | Budget revu | Coûts des soirées à +5 % |
|---|---|---|
| Marge par soirée : Premier soir / Le Voyage / La Grande Nuit / Privatisation | 2 788 / 2 214 / 4 066 / 4 464 € | 2 418 / 1 711 / 3 406 / 4 051 € |
| Résultat, années 1 / 2 / 3 | −36 232 / 387 758 / 378 857 € | −43 816 / 320 660 / 244 275 € |
| Point mort de l'année 3 | 213 soirées | 239 soirées, pour 306 prévues |
| **Point bas sur 36 mois** | −52 929 € (mars 2027) | **−54 729 € (mars 2027)** |
| Trésorerie en fin d'année 3 | 808 460 € | 597 855 € |

## 4. Ce qui peut faire dérailler le plan (F, simulations)

**Nombre de privatisations**, avec les coûts des soirées à +5 % :

| Privatisations par ville et par an, dès l'année 2 | Résultat, années 2 / 3 | Point bas de la trésorerie | Trésorerie en fin d'année 3 |
|---|---|---|---|
| 40 (budget revu) | 320 660 / 244 275 € | −54 729 € (mars 2027) | 597 855 € |
| 20 | 130 337 / −136 371 € | −54 729 € (mars 2027) ; −30 000 € environ en juillet 2029 | 22 346 € |
| 8 (le rythme du plan précédent) | −5 868 / −372 096 € | **−352 323 € (octobre 2029)**, et la baisse continue | −352 323 € |

**Jauge de la privatisation**, sans hausse des coûts :

| Couverts par privatisation | Marge par privatisation | Résultat, années 2 / 3 | Point bas de la trésorerie |
|---|---|---|---|
| 30 (budget revu) | 4 464 € | 387 758 / 378 857 € | −52 929 € (mars 2027) |
| 20 (décision D-05) | 1 893 € | 89 901 / −216 858 € | **−137 660 € (juillet 2029)** |

**I** Ce qui pèse le plus, ce sont les frais de l'année 3 : 862 357 €, dont 15 postes payés. Ils sont engagés en novembre 2028, avec l'ouverture de 3 villes et 12 postes payés de plus (3 coordinateurs, 6 commerciaux, le manager et 2 fondateurs). Si les privatisations ou la jauge ne suivent pas, c'est cette étape qui crée le besoin de financement.

## 5. Contingence et besoin à financer (P)

La règle reste celle de la note de l'après-midi : point bas avec les coûts à +5 %, contingence sur les coûts, trésorerie de sécurité. **Elle s'applique ici à l'année 1**, la seule période où la société consomme de la trésorerie dans le plan. Le risque des années 2 et 3 est traité par la tranche 2 conditionnelle (§ 6).

| Composante | Règle | Montant |
|---|---|---|
| Besoin de trésorerie (point bas, coûts des soirées à +5 %) | Calcul du modèle | 54 729 € |
| Contingence sur les coûts des soirées | 5 % des coûts directs de l'année 1 (162 345 €) | 8 117 € |
| Contingence sur les frais généraux et les investissements | 10 % de ceux de l'année 1 (93 530 € + 18 000 €) | 11 153 € |
| Trésorerie de sécurité | 3 mois de frais généraux de l'année 2 (236 698 € ÷ 4), quand les 3 coordinateurs sont recrutés et avant que les privatisations soient prouvées | 59 175 € |
| **Besoin total à financer** | | **133 174 €, soit environ 135 000 €** |

## 6. Plan de financement proposé (P)

| Tranche | Quand | Montant | Sources | Pourquoi |
|---|---|---|---|---|
| **Tranche 1 (pré-amorçage)** | Avant février 2027 | **135 000 €** | Prêt d'honneur 20 000 € (H) ; subvention 5 000 € (H) ; **BSA AIR 110 000 €** (business angels, dont des proches de l'associé gastronomique) | Couvre le point bas de mars 2027 (−54 729 € à +5 %), la contingence et 3 mois de frais de l'année 2. Le BSA AIR ne fixe pas de valorisation tout de suite |
| **Tranche 2 (conditionnelle)** | Décision en mai 2028 | 0 € dans le plan | Business angels et investisseurs financiers (D-17) | **I** Elle devient nécessaire si les privatisations restent loin de 40 par ville et par an. À 8 par ville et par an, il faudrait environ 220 000 € de plus que la tranche 1, avant contingence, ou renoncer à l'expansion de l'année 3 |
| Associé gastronomique | À l'entrée au capital | 0 € de trésorerie | Apport en industrie (D-17), 5 % proposés avant la levée | Réseau, sélection, image |
| **Total demandé** | | **135 000 €**, plus l'apport de 7 000 € | | |

**Dès novembre 2026.** **I** Il manque environ 17 800 € dès le premier mois, avant toute subvention : le site (15 000 €) et le matériel (3 000 €) sont payés au départ, et l'apport n'est que de 7 000 €. Deux solutions possibles (P) :
- les associés avancent cet argent en compte courant ;
- le paiement du site est étalé (acompte, puis solde à la livraison).

**Dilution (I, modèle Financement, onglet « Après levée »).** Calcul illustratif, car les BSA AIR se convertiront au prix d'une levée ultérieure. À la valorisation de 400 000 € avant levée, qui reste une hypothèse non justifiée, les 110 000 € donneraient **21,6 %** du capital aux investisseurs. Chaque fondateur garderait 10,6 % et l'associé gastronomique 3,9 %. Le plafond de valorisation des BSA AIR est à négocier : le budget revu montre un résultat de 387 758 € en année 2, mais il n'est appuyé par aucune soirée réalisée.

## 7. Décisions demandées à la Direction

| # | Décision | Proposition de la Finance |
|---|---|---|
| 1 | Montant de la levée | Environ 135 000 € avant février 2027, dont 110 000 € en BSA AIR |
| 2 | Tranche 2 | Point de décision en mai 2028 : ouvrir les villes 4 à 6 et payer les 12 postes ajoutés en novembre 2028 seulement si les privatisations vendues sont proches du plan ; sinon lever environ 220 000 € de plus ou décaler l'expansion |
| 3 | Jauge de la privatisation | Confirmer 30 couverts (budget revu) ou garder 20 (D-05) : l'écart change la trésorerie de fin d'année 3 de plus de 900 000 € |
| 4 | Volume de privatisations (D-16) | Demander aux Ventes de confirmer 40 par ville et par an, et de dire qui les vend en année 2 |
| 5 | Trésorerie de novembre 2026 | Compte courant d'associés, ou paiement du site étalé |
| 6 | Part de l'associé gastronomique | 5 % avant la levée, acquis par jalons (forme à définir par le Juridique) |
| 7 | Soirée de lancement | Choisir l'option et le montant (28 000 € H dans le modèle) |
| 8 | Salaires du manager et des fondateurs | Valider 4 000 € brut par mois pour le manager et 2 500 € pour chaque fondateur, en année 3 |

**Préalables inchangés** (note de l'après-midi) :
- société créée, statuts et pacte d'associés signés ;
- dépôt passé en privé ;
- licence obtenue (D-09) ;
- coûts des lieux et des chefs confirmés par des devis.

**Rappel (voir [[AGENT]] de la Finance).** Cette note propose un dimensionnement. Elle n'engage personne auprès d'une banque ou d'un investisseur. Un montant demandé n'est pas un montant obtenu.

## 8. Limites du calcul (I)

- **Impôt sur les sociétés non compté.** Ordre de grandeur, au taux réduit de 15 % jusqu'à 42 500 € et au taux normal de 25 % au-delà, après imputation de la perte de l'année 1 : environ 83 600 € au titre de l'année 2 et 90 500 € au titre de l'année 3. Les taux et les conditions du taux réduit sont à confirmer par l'expert-comptable. L'impôt ne change pas le point bas de mars 2027, mais il réduit la trésorerie des années 2 et 3.
- Les villes ne sont pas nommées. Prix, coûts et TVA y sont supposés identiques à Paris, et le change n'est pas pris en compte.
- Les privatisations sont réparties également sur les 12 mois, août compris.
- La TVA sur la pré-vente est comptée le mois de la soirée, pas le mois de l'encaissement.
- Le remboursement du prêt d'honneur n'est pas compté.
- Les délais de paiement des entreprises ne sont pas modélisés : avec 240 privatisations par an, dont une partie en B2B, ils peuvent peser sur la trésorerie.
- Les remboursements en cas de soirée annulée ne sont pas modélisés : la pré-vente est un argent dû tant que la soirée n'a pas eu lieu.
