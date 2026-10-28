# Pop Tables : données financières manquantes et hypothèses

**Date : 28/10/2026 (soir)** · Fonction : `2 FINANCE` · Auteur : assistant IA Finance, à la demande de Vianney (responsable Finance) · Statut : document de travail.

Cette fiche remplace [[2026 1027 Données financières manquantes et hypothèses temporaires]], rangée dans `2 FINANCE/OLD/`. Elle suit les décisions D-02 à D-20 de la Direction ([[2026 1028 Relevé de décisions du 28 octobre (soir)]], [[2026 1028 Pop Tables - Cadre de référence]], [[REGISTRE DES DECISIONS]]) et le **budget sur 36 mois revu par le responsable Finance le 28/10/2026 (soir)**, qui fait référence.

Légende (voir [[RULES]]) : **F** = fait constaté dans un fichier du dépôt ou décision inscrite au registre · **I** = inférence · **P** = proposition · **H** = hypothèse temporaire.

## 1. L'essentiel

> - **F** Le budget est **détaillé mois par mois sur 36 mois**, de novembre 2026 à octobre 2029. Le responsable Finance l'a revu le 28/10 (soir) : nouvelles villes actives dès novembre, 40 privatisations par ville et par an dès l'année 2, équipe calculée à partir de l'activité, prix et coûts revus.
> - **F** Les jauges des places à l'unité, l'enveloppe d'équipe et la suppression du photographe sont des **décisions** (D-05, D-06, D-08). Le reste des montants est encore **hypothétique** : aucun devis, aucune facture, aucune soirée réalisée.
> - **F** Résultat d'exploitation, avant impôt : **−36 232 €** en année 1, **387 758 €** en année 2, **378 857 €** en année 3.
> - **F** Trésorerie avant levée : point bas de **−52 929 € en mars 2027**, puis trésorerie positive dès novembre 2027. Point bas de −54 729 € si les coûts des soirées augmentent de 5 %.
> - **P** Levée proposée : environ 135 000 € avant février 2027, et une tranche 2 conditionnelle ([[2026 1028 Note pour décision - levée de fonds Pop Tables]]).
> - **I** Les données qui pèsent le plus sont, dans l'ordre :
>   1. le nombre de privatisations (78 % du chiffre d'affaires des années 2 et 3) ;
>   2. la jauge de la privatisation (30 couverts dans le budget, 20 dans D-05) ;
>   3. l'indemnité des restaurants et le cachet des chefs ;
>   4. le coût réel de l'équipe.

Fichiers :

| Modèle | Fichier |
|---|---|
| Prévisions (référence) | `PREVISIONS/2026 1028 Modèle Pop Tables - Budget sur 36 mois, plan financier, prix et marges.xlsx` |
| Trésorerie | `TRESORERIE/2026 1028 Modèle Pop Tables - Trésorerie et mois de survie sur 36 mois.xlsx` |
| Financement | `FINANCEMENT/2026 1028 Modèle Pop Tables - Financement et table de capitalisation.xlsx` |
| Tableau de bord | `PREVISIONS/2026 1028 Pop Tables - Tableau de bord financier.html` |

### Ce que contient le modèle Prévisions

| Onglet | Contenu |
|---|---|
| Prix et marges | L'économie d'une soirée par offre ; privatisation à 500 € TTC par convive |
| Budget 36 mois | Villes et soirées (lignes 7 à 19), effectifs nécessaires (lignes 20 à 22), chiffre d'affaires et coûts directs (24 à 31), ressources humaines (33 à 37), 17 postes de fonctionnement, marketing et ventes (39 à 55), investissements (62 à 64), TVA (66 à 75), pré-vente et trésorerie avant levée (77 à 80), un mois par colonne ; paramètres (lignes 84 à 93) et calendrier des villes (96 à 101) |
| Ressources humaines | Règles d'effectif (1 coordinateur par événement hebdomadaire, 1 commercial par ville active), postes, salaires et premier mois payé |
| TVA | Taux et règles. Le calcul mois par mois est dans « Budget 36 mois » |
| Plan financier 3 ans | Totaux annuels, point mort, besoin de financement, point bas de trésorerie |
| Prévu et réel | Suivi de l'année 1 |
| Staffing | Sert seulement au surcoût des pilotes |

## 2. Décisions et choix intégrés

| Décision ou choix | Dans le modèle (onglet « Budget 36 mois », sauf mention) | Nature |
|---|---|---|
| D-05 jauges, D-06 enveloppe d'équipe, D-08 photographe | Prix et marges, lignes 7, 26 et 33. **La privatisation y est à 30 couverts, alors que D-05 en fixe 20** | F, sauf la jauge de la privatisation |
| D-14 soirée de lancement | Ligne 43 : 28 000 € en mars 2027 | H pour le montant |
| D-15 villes : 1 soirée « place à l'unité » par mois et par ville ; 1, 3 puis 6 villes | Lignes 7 à 17 et 52 ; calendrier lignes 96 à 101 ; nouvelles villes actives dès novembre 2027 et novembre 2028 | F pour le rythme, H pour les mois d'ouverture |
| D-16 privatisations | Ligne 12 : 7 en année 1, puis 40 par ville active et par an (paramètre B90) | H, fixé par le responsable Finance, à caler avec les Ventes |
| D-19 site internet | Ligne 62 : 15 000 € en novembre 2026 | F pour le montant |
| D-09 licence propre | Ligne 53 : 1 000 € | H |
| D-04 pré-vente | Ligne 77 : places encaissées le mois qui précède la soirée | H pour le délai |
| D-17 associé gastronomique | Modèle Financement : apport en industrie, 5 % proposés | P |
| D-20 Business Model Canvas V5 | Fait foi ; ses éléments financiers doivent être ajustés après le travail de la Finance | F |
| Campagne de lancement de 10 000 € (influenceurs, assets) | Ligne 42 : février et mars 2027 | Montant fixé par le responsable Finance |
| Protection juridique et assurance de la société : 2 % du CA | Ligne 48 | Taux fixé par le responsable Finance |
| Budget des ventes et de la prospection | Lignes 44 à 47 : 8 065 €, 17 405 € puis 29 210 € | H |
| Équipe calculée à partir de l'activité | Lignes 20 à 22 et 33 à 36 : 3 coordinateurs dès novembre 2027, puis 6 ; 6 commerciaux, 1 manager et 2 fondateurs payés dès novembre 2028 (15 postes) | H, règles fixées par le responsable Finance |

## 3. Données manquantes, hypothèses et qui peut les fournir

| # | Donnée manquante | Où elle sert | Hypothèse actuelle (H) | Qui peut la fournir | Priorité |
|---|---|---|---|---|---|
| 1 | Nombre de privatisations vendables par ville et par mois (D-16), et qui les vend en année 2 | Budget 36 mois, ligne 12 et paramètre B90 | 7 en année 1, puis 40 par ville et par an : 120, puis 240 ; aucun commercial payé avant novembre 2028 | Ventes (@xavierjuraflo-ship-it), avec la Finance | 1 |
| 2 | Jauge de la privatisation | Prix et marges, ligne 7, colonne F | 30 couverts ; D-05 en fixe 20. À 20 couverts, l'année 3 perd 216 858 € | Direction (@Laetitiarv) | 1 |
| 3 | Indemnité d'un restaurant pour un soir de fermeture, minimum garanti, ce que couvre la mise à disposition | Prix et marges, ligne 19 | 1 000 € pour toutes les offres | Ventes, par le démarchage des restaurants (D-18) | 1 |
| 4 | Cachet des chefs par niveau, déplacement, accord de la maison d'origine | Ligne 20 | 950 €, 2 000 €, 3 500 € et 1 800 €, entièrement fixes | Produit (@Fredlay26), sélection des chefs (D-18) | 1 |
| 5 | Coût de l'équipe dans l'enveloppe de D-06 | Ligne 26 | 15 % ou 20 % du CA (D-06). Les Opérations proposent 2 516, 2 516, 2 201 et 1 935 € (branche `ops/jauges-finance-equipe-fixe`, non fusionnée) | Opérations (@jonathanstarke-hec) ; arbitrage de la Direction | 1 |
| 6 | Grille de prix fixes par offre et par créneau (D-10) | Lignes 10 et 11 | 290 €, 420 € et 690 € TTC ; privatisation à 500 € TTC par convive, sans forfait | Produit | 1 |
| 7 | Option et montant de la soirée de lancement (D-14) | Budget 36 mois, ligne 43 | 28 000 € HT en mars 2027 | Marketing (@serge2309) | 1 |
| 8 | Taux de remplissage réel | Ligne 8 | Salle pleine (100 %), alors que l'équilibre demande 59 %, 73,5 %, 68,1 % et 54,1 % | Marketing (liste privée, drops) ; mesure aux pilotes | 1 |
| 9 | Coût des matières par menu ; prix des vins d'AdVini ; accord mets-jus | Lignes 23 et 24 | Matières et boissons : 85 €, 112 €, 150 € et 100 € par convive | Opérations, avec le chef ; accord écrit avec AdVini | 1 |
| 10 | Salaires et dates d'embauche : coordinateurs, commerciaux, manager, fondateurs | Onglet Ressources humaines | SMIC pour les coordinateurs, 2 800 € brut pour les commerciaux, 4 000 € pour le manager, 2 500 € pour chaque fondateur ; charges à 45 % | Direction | 2 |
| 11 | Villes 2 à 6, mois d'ouverture, coût d'ouverture (modèle d'ouverture d'une ville) | Lignes 7, 14 à 17 et 52 ; paramètres lignes 84 à 87 | 2 villes actives dès novembre 2027, 3 de plus dès novembre 2028 ; 15 000 € par ville ; déplacements de 300 € et 700 € par soirée « place à l'unité » | Direction, sur proposition du Marketing et des Ventes ; Opérations pour le coût | 2 |
| 12 | Coût de la licence et du permis d'exploitation (D-09), et règles à l'étranger | Ligne 53 | 1 000 € | Juridique (@alexanderzhelev-dev) | 2 |
| 13 | Devis d'assurance (RC professionnelle, multirisque, protection juridique) : les 2 % du CA sont-ils réalistes ? | Ligne 48 ; Prix et marges, ligne 28 | 2 % du CA (82 750 € en année 3), plus 150 € par soirée | Juridique (récapitulatif des assurances du 28/10) | 2 |
| 14 | Conditions de la pré-vente : paiement complet ou acompte, délai entre le drop et la soirée, remboursement | Ligne 77 ; trésorerie | Paiement complet le mois qui précède la soirée, sans remboursement | Juridique (CGV) ; Produit | 2 |
| 15 | Budget des ventes : outils, rendez-vous, places offertes aux prescripteurs, supports et salons | Lignes 44 à 47 | 8 065 €, 17 405 € puis 29 210 € | Ventes, pour validation | 2 |
| 16 | Part des ventes via les concierges et commission | Ligne 31 | 0 % (Premier soir), 5 % (Le Voyage, La Grande Nuit, privatisation) | Marketing ; Ventes | 2 |
| 17 | TVA : taux, exigibilité sur la pré-vente, TVA à l'étranger, crédit de TVA | Onglet TVA ; lignes 66 à 75 | 12 % sur les ventes ; taux par poste ; TVA à l'étranger supposée identique | Expert-comptable | 2 |
| 18 | Impôt sur les sociétés, désormais dû dans le plan | Non modélisé | Environ 83 600 € au titre de l'année 2 et 90 500 € au titre de l'année 3 (I, taux de 15 % puis 25 %) | Expert-comptable | 2 |
| 19 | Part et forme de l'entrée de l'associé gastronomique (D-17) | Modèle Financement, « Après levée » | Apport en industrie, 5 % avant la levée | Direction ; Juridique | 2 |
| 20 | Marketing courant des années 2 et 3, communication des villes | Ligne 41 | 15 000 € puis 30 000 € | Marketing | 3 |
| 21 | Valorisation de la société, plafond des BSA AIR | Modèle Financement | 400 000 € avant levée, sans aucune évaluation | Finance, après les pilotes | 3 |
| 22 | Création de la société, capital, compte bancaire | Financement ; trésorerie | 7 associés à 1 000 € au 01/11/2026, sans pièce | Juridique ; Finance | 3 |
| 23 | Revenus de partenariats (AdVini, maisons de champagne) | Prix et marges, ligne 16 | 0 € | Ventes ; Opérations | 3 |

## 4. Points signalés (I)

1. **Tout repose sur les privatisations.** Avec les coûts à +5 %, à 20 privatisations par ville et par an, l'année 3 perd 136 371 €. À 8 (le rythme du plan précédent), la trésorerie descend à −352 323 € en octobre 2029.
2. **Jauge de la privatisation.** Le budget compte 30 couverts, mais la ligne cite toujours D-05, qui en fixe 20. À décider par la Direction.
3. **Pas de commercial en année 2**, alors que les privatisations passent de 7 à 120.
4. **Équipe.** L'enveloppe de D-06, calculée en % du CA, sous-budgète le Premier soir de 962 € et sur-budgète La Grande Nuit de 1 495 €, d'après les Opérations.
5. **Salle pleine.** C'est une hypothèse de la Finance, que D-05 ne couvre pas. Le seuil de confirmation à J-14 (70 %) reste en dessous de l'équilibre du Voyage (73,5 %).
6. **Sommelier.** Les Opérations remplacent le sommelier par un vigneron d'AdVini non payé, sans accord écrit. Sans lui, il faudrait environ 420 € de plus par soirée.
7. **Pré-vente.** Elle améliore la trésorerie, mais c'est un argent dû aux clients tant que la soirée n'a pas eu lieu.
8. **Prix non publics (D-11).** Les colonnes « Prix affiché » du modèle désignent le prix communiqué à la réservation, pas un prix publié.
9. **Notes du modèle à corriger.** Dans « Budget 36 mois », certaines explications citent d'anciennes cellules :
   - ligne 12 : « paramètre B86 », au lieu de B90 ;
   - ligne 52 : « B82 », « B83 » et « C90:C94 », au lieu de B86, B87 et C97:C101 ;
   - ligne 16 : « B86 », au lieu de B90.

   Dans « Plan financier 3 ans », les privatisations des années 2 et 3 (D12 et E12) sont saisies en dur (3 × 40 et 6 × 40) au lieu d'être reprises du budget. Les calculs sont justes aujourd'hui. Ils ne suivront pas un changement du paramètre B90.

## 5. Prochaines étapes proposées (P)

1. La Direction tranche la jauge de la privatisation (n° 2).
2. Les Ventes confirment le nombre de privatisations et disent qui les vend en année 2 (n° 1), puis fournissent l'indemnité des restaurants (n° 3).
3. Le Produit fournit les cachets des chefs et la grille de prix par créneau (n° 4 et 6).
4. La Direction arbitre entre l'enveloppe de D-06 et le staffing par effectif des Opérations (n° 5), et valide les salaires (n° 10).
5. Le Marketing choisit l'option de la soirée de lancement (n° 7).
6. La Finance met à jour le modèle à chaque réponse et recalcule la levée.
