# Pop Tables : données financières manquantes et hypothèses

**Date : 28/10/2026 (soir), mise à jour le 29/10/2026** · Fonction : `2 FINANCE` · Auteur : assistant IA Finance, à la demande de Vianney (responsable Finance) · Statut : document de travail.

Cette fiche remplace [[2026 1027 Données financières manquantes et hypothèses temporaires]], rangée dans `2 FINANCE/OLD/`. Elle suit les décisions D-02 à D-26 de la Direction ([[2026 1028 Relevé de décisions du 28 octobre (soir)]], [[2026 1029 Relevé de décisions du 29 octobre (matin)]], [[REGISTRE DES DECISIONS]]). Le budget sur 36 mois revu par le responsable Finance est la référence décidée (D-21).

Légende (voir [[RULES]]) : **F** = fait constaté dans un fichier du dépôt ou décision inscrite au registre · **I** = inférence · **P** = proposition · **H** = hypothèse temporaire.

## 1. L'essentiel

> - **F** Le budget est **détaillé mois par mois sur 36 mois**, de novembre 2026 à octobre 2029. C'est la référence décidée par la Direction (D-21), avec la privatisation à 500 € TTC par convive et 30 couverts (D-22).
> - **F** Le 29/10, la Direction a décidé 2 villes en France en novembre 2027 et 3 villes à l'étranger en novembre 2028 (D-25), ainsi qu'une mise de fonds initiale de 70 000 € en love money (D-26). Les deux sont intégrées au modèle.
> - **F** Résultat d'exploitation, avant impôt : **−36 232 €** en année 1, **392 158 €** en année 2, **378 857 €** en année 3.
> - **F** Trésorerie avant levée : point bas de **+10 071 € en mars 2027** ; elle ne devient jamais négative. Point bas de +8 271 € si les coûts des soirées augmentent de 5 %.
> - **P** Levée recalculée : environ 70 000 € avant février 2027, au lieu de 135 000 € (D-23 à modifier), et une tranche 2 conditionnelle ([[2026 1028 Note pour décision - levée de fonds Pop Tables]]).
> - **F** La plupart des montants restent des **hypothèses** : aucun devis, aucune facture, aucune soirée réalisée.
> - **I** Les données qui pèsent le plus sont, dans l'ordre :
>   1. le nombre de privatisations (78 % du chiffre d'affaires des années 2 et 3) ;
>   2. le prix facturé quand une privatisation compte moins de 30 convives ;
>   3. l'indemnité des restaurants et le cachet des chefs ;
>   4. le coût réel de l'équipe.

Fichiers :

| Modèle | Fichier |
|---|---|
| Prévisions (référence) | `PREVISIONS/2026 1028 Modèle Pop Tables - Budget sur 36 mois, plan financier, prix et marges.xlsx` |
| Trésorerie | `TRESORERIE/2026 1028 Modèle Pop Tables - Trésorerie et mois de survie sur 36 mois.xlsx` |
| Financement | `FINANCEMENT/2026 1028 Modèle Pop Tables - Financement et table de capitalisation.xlsx` |
| Tableau de bord | `PREVISIONS/2026 1029 Pop Tables - Tableau de bord financier.html` |

### Ce que contient le modèle Prévisions

| Onglet | Contenu |
|---|---|
| Prix et marges | L'économie d'une soirée par offre ; privatisation à 500 € TTC par convive (D-22) |
| Budget 36 mois | Villes et soirées (lignes 7 à 19), effectifs nécessaires (lignes 20 à 22), chiffre d'affaires et coûts directs (24 à 31), ressources humaines (33 à 37), 17 postes de fonctionnement, marketing et ventes (39 à 55), investissements (62 à 64), TVA (66 à 75), pré-vente, love money et trésorerie avant levée (77 à 80), un mois par colonne ; paramètres (lignes 84 à 93) et calendrier des villes (96 à 101) |
| Ressources humaines | Règles d'effectif (1 coordinateur par événement hebdomadaire, 1 commercial par ville active), postes, salaires et premier mois payé |
| TVA | Taux et règles. Le calcul mois par mois est dans « Budget 36 mois » |
| Plan financier 3 ans | Totaux annuels, point mort, besoin de financement, point bas de trésorerie |
| Prévu et réel | Suivi de l'année 1 |
| Staffing | Sert seulement au surcoût des pilotes |

## 2. Décisions intégrées

| Décision | Dans le modèle (onglet « Budget 36 mois », sauf mention) | Nature |
|---|---|---|
| D-05 jauges des places à l'unité, D-06 enveloppe d'équipe, D-08 photographe | Prix et marges, lignes 7, 26 et 33 | F |
| D-21 budget revu par le responsable Finance | Tout l'onglet : 40 privatisations par ville et par an dès l'année 2, équipe calculée à partir de l'activité, lieu à 1 000 €, commission de 5 %, campagne de 10 000 €, protection juridique et assurance à 2 % du CA, budget des ventes | F pour la décision ; montants en hypothèse (H) |
| D-22 privatisation | Prix et marges, colonne F : 500 € TTC par convive, 30 couverts, sans forfait | F |
| D-23 levée | Modèle Financement et note de levée : tranche 1 recalculée à environ 70 000 € avec la love money ; tranche 2 conditionnelle | F pour le principe ; montant de la tranche 1 à confirmer |
| D-24 Business Model Canvas V6 | Fait foi pour l'ensemble du projet. Il mentionne encore la tranche 1 de 135 000 € : une V7 est prévue par la Direction | F |
| D-25 villes | Lignes 7, 14 à 17 et 52 ; calendrier lignes 96 à 101 : villes 2 et 3 en France dès novembre 2027, villes 4 à 6 à l'étranger dès novembre 2028. Les lignes 14 à 17 se calculent à partir du pays et de la date de chaque ville | F |
| D-26 love money | Ligne 78 : 70 000 € en novembre 2026 ; modèle Financement, ligne 6 | F pour le montant ; H pour le mois ; forme non décidée |
| D-14 soirée de lancement | Ligne 43 : 28 000 € en mars 2027 (option 2 du Marketing) | H pour le montant |
| D-16 privatisations | Ligne 12 et paramètre B90 | Volume à confirmer par les Ventes |
| D-19 site internet | Ligne 62 : 15 000 € en novembre 2026 | F pour le montant |
| D-09 licence propre | Ligne 53 : 1 000 € ; le Juridique estime 600 à 1 200 € (formation au permis d'exploitation) | H |
| D-04 pré-vente | Ligne 77 : places encaissées le mois qui précède la soirée | H pour le délai |
| D-17 associé gastronomique | Modèle Financement : apport en industrie, 5 % proposés | P |

## 3. Données manquantes, hypothèses et qui peut les fournir

| # | Donnée manquante | Où elle sert | Hypothèse actuelle (H) | Qui peut la fournir | Priorité |
|---|---|---|---|---|---|
| 1 | Nombre de privatisations vendables par ville et par mois (D-16), et qui les vend en année 2 | Budget 36 mois, ligne 12 et paramètre B90 | 7 en année 1, puis 40 par ville et par an : 120, puis 240 ; aucun commercial payé avant novembre 2028 | Ventes (@xavierjuraflo-ship-it), avec la Finance | 1 |
| 2 | Prix d'une privatisation à moins de 30 convives : minimum facturé de 30 couverts ou forfait | Prix et marges, ligne 15 (minimum facturé, à 0 aujourd'hui) | Chaque privatisation est pleine (30 convives) | Direction (relevé du 29/10, § 3) ; Produit (@Fredlay26) | 1 |
| 3 | Indemnité d'un restaurant pour un soir de fermeture, minimum garanti, ce que couvre la mise à disposition | Prix et marges, ligne 19 | 1 000 € pour toutes les offres | Ventes, par le démarchage des restaurants (D-18) | 1 |
| 4 | Cachet des chefs par niveau, déplacement, accord de la maison d'origine | Ligne 20 | 950 €, 2 000 €, 3 500 € et 1 800 €, entièrement fixes | Produit, sélection des chefs (D-18) | 1 |
| 5 | Coût de l'équipe dans l'enveloppe de D-06 | Ligne 26 | 15 % ou 20 % du CA (D-06). Les Opérations proposent 2 516, 2 516, 2 201 et 1 935 € (branche `ops/jauges-finance-equipe-fixe`, non fusionnée) | Opérations (@jonathanstarke-hec) ; arbitrage de la Direction | 1 |
| 6 | Grille de prix fixes par offre et par créneau (D-10) | Lignes 10 et 11 | 290 €, 420 € et 690 € TTC ; privatisation à 500 € TTC par convive (D-22) | Produit | 1 |
| 7 | Forme de la love money (D-26) : capital, compte courant d'associés ou BSA AIR, et clauses avec les proches | Modèle Financement ; table de capitalisation | Non comptée dans la table de capitalisation tant que la forme n'est pas décidée | Juridique (@alexanderzhelev-dev) ; Direction | 1 |
| 8 | Taux de remplissage réel | Ligne 8 | Salle pleine (100 %), alors que l'équilibre demande 59 %, 73,5 %, 68,1 % et 54,1 % | Marketing (liste privée, drops) ; mesure aux pilotes | 1 |
| 9 | Coût des matières par menu ; prix des vins d'AdVini ; accord mets-jus | Lignes 23 et 24 | Matières et boissons : 85 €, 112 €, 150 € et 100 € par convive | Opérations, avec le chef ; accord écrit avec AdVini | 1 |
| 10 | Salaires et dates d'embauche : coordinateurs, commerciaux, manager, fondateurs | Onglet Ressources humaines | SMIC pour les coordinateurs, 2 800 € brut pour les commerciaux, 4 000 € pour le manager, 2 500 € pour chaque fondateur ; charges à 45 % | Direction | 2 |
| 11 | Villes 2 à 6 et coût d'ouverture (modèle d'ouverture d'une ville) | Paramètres lignes 84 à 87 ; calendrier lignes 96 à 101 | 2 villes en France dès novembre 2027, 3 à l'étranger dès novembre 2028 (D-25) ; 15 000 € par ville ; déplacements de 300 € et 700 € par soirée « place à l'unité » | Direction, sur proposition du Marketing et des Ventes ; Opérations pour le coût | 2 |
| 12 | Coût des logiciels du site (Shopify, billetterie ou drop, agent conversationnel) | Paramètres B92 et B93 | 80 € par mois de socle, plus 50 € par poste payé | Devis des prestataires ; Marketing ([[2026 1029 Note du Marketing à la Finance et au Produit]], § 3) | 2 |
| 13 | Coût de la licence et du permis d'exploitation (D-09), et règles à l'étranger | Ligne 53 | 1 000 € ; le Juridique estime 600 à 1 200 € | Juridique | 2 |
| 14 | Devis d'assurance : les 2 % du CA sont-ils réalistes ? | Ligne 48 ; Prix et marges, ligne 28 | 2 % du CA (82 750 € en année 3), plus 150 € par soirée ; repris par le Juridique dans son récapitulatif des assurances | Juridique, avec les devis | 2 |
| 15 | Conditions de la pré-vente : paiement complet ou acompte, délai entre le drop et la soirée, remboursement | Ligne 77 ; trésorerie | Paiement complet le mois qui précède la soirée, sans remboursement | Juridique (CGV) ; Produit | 2 |
| 16 | Budget des ventes : outils, rendez-vous, places offertes aux prescripteurs, supports et salons | Lignes 44 à 47 | 8 065 €, 17 405 € puis 29 210 € | Ventes, pour validation | 2 |
| 17 | Part des ventes via les concierges et commission | Ligne 31 | 0 % (Premier soir), 5 % (Le Voyage, La Grande Nuit, privatisation) | Marketing ; Ventes | 2 |
| 18 | TVA : taux, exigibilité sur la pré-vente, TVA à l'étranger, crédit de TVA | Onglet TVA ; lignes 66 à 75 | 12 % sur les ventes ; taux par poste ; TVA à l'étranger supposée identique | Expert-comptable | 2 |
| 19 | Impôt sur les sociétés, dû dans le plan | Non modélisé | Environ 84 700 € au titre de l'année 2 et 90 500 € au titre de l'année 3 (I, taux de 15 % puis 25 %) | Expert-comptable | 2 |
| 20 | Part et forme de l'entrée de l'associé gastronomique (D-17) | Modèle Financement, « Après levée » | Apport en industrie, 5 % avant la levée | Direction ; Juridique | 2 |
| 21 | Rythme saisonnier des villes de bord de mer (Côte d'Azur) | Lignes 8 à 12 de la ville concernée | Activité répartie également sur l'année | Marketing ; Direction (choix des villes) | 3 |
| 22 | Marketing courant des années 2 et 3, communication des villes | Ligne 41 | 15 000 € puis 30 000 € | Marketing | 3 |
| 23 | Valorisation de la société, plafond des BSA AIR | Modèle Financement | 400 000 € avant levée, sans aucune évaluation | Finance, après les pilotes | 3 |
| 24 | Revenus de partenariats (AdVini, maisons de champagne) | Prix et marges, ligne 16 | 0 € | Ventes ; Opérations | 3 |

## 4. Points signalés (I)

1. **Tout repose sur les privatisations.** Avec les coûts à +5 %, à 20 privatisations par ville et par an, l'année 3 perd 136 371 €. À 8 (le rythme du plan du 27/10), la trésorerie descend à −284 703 € en octobre 2029, malgré la love money.
2. **Pas de commercial en année 2**, alors que les privatisations passent de 7 à 120.
3. **Trésorerie mince en année 1.** Elle reste entre 10 000 € et 60 000 € de novembre 2026 à octobre 2027 : un retard de pilote ou un dépassement de la soirée de lancement suffit à la faire passer sous zéro. D'où la tranche 1 proposée.
4. **Équipe.** L'enveloppe de D-06, calculée en % du CA, sous-budgète le Premier soir de 962 € et sur-budgète La Grande Nuit de 1 495 €, d'après les Opérations.
5. **Salle pleine.** C'est une hypothèse de la Finance, que D-05 ne couvre pas. Le seuil de confirmation à J-14 (70 %) reste en dessous de l'équilibre du Voyage (73,5 %).
6. **Sommelier.** Les Opérations remplacent le sommelier par un vigneron d'AdVini non payé, sans accord écrit. Sans lui, il faudrait environ 420 € de plus par soirée.
7. **Pré-vente.** Elle améliore la trésorerie, mais c'est un argent dû aux clients tant que la soirée n'a pas eu lieu.
8. **Prix non publics (D-11).** Les colonnes « Prix affiché » du modèle désignent le prix communiqué à la réservation. Le Marketing propose de lire D-11 comme un prix discret, visible sur le site au moment de réserver : à confirmer par la Direction.

## 5. Prochaines étapes proposées (P)

1. La Direction fixe le montant de la tranche 1 (environ 70 000 € proposés) et tranche la privatisation à moins de 30 convives (n° 2).
2. Le Juridique propose la forme de la love money (n° 7).
3. Les Ventes confirment le nombre de privatisations dans les 2 villes françaises de l'année 2 et disent qui les vend (n° 1), puis fournissent l'indemnité des restaurants (n° 3).
4. Le Produit fournit les cachets des chefs et la grille de prix par créneau (n° 4 et 6).
5. La Direction arbitre entre l'enveloppe de D-06 et le staffing par effectif des Opérations (n° 5), et valide les salaires (n° 10).
6. La Finance met à jour le modèle à chaque réponse et recalcule la levée.
