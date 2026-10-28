# Données financières manquantes et hypothèses temporaires

Date : 27/10/2026, mis à jour le 28/10/2026 (frais généraux, puis staffing des Opérations) · Auteur : assistant IA Finance, à la demande de Vianney (responsable Finance) · Statut : document de travail. Les chiffres sont des hypothèses temporaires, pas des décisions (voir [[REGISTRE DES DECISIONS]]).

Légende (voir [[RULES]]) : F = fait constaté dans une source citée · I = inférence · P = proposition · H = hypothèse temporaire, à remplacer.

Fichiers mis à jour, dans lesquels chaque valeur porte sa nature et sa source :
- `PREVISIONS/2026 1027 Modèle - Budget, plan financier, prix et marges.xlsx`
- `FINANCEMENT/2026 1027 Modèle - Financement et table de capitalisation.xlsx`
- `TRESORERIE/2026 1027 Modèle - Trésorerie et mois de survie.xlsx`

## 1. L'essentiel

- **F** Dans le dépôt, les seuls chiffres propres au projet sont les prix et capacités proposés par le Produit (P, établis « sans donnée de coûts ») : `5 PRODUIT/Fou d'un soir le pricing.md` et le plan des deux soirées pilotes. Aucun coût réel, aucun devis, aucun financement, aucune pièce bancaire n'existe encore.
- **F** Depuis le 28/10/2026, les Opérations proposent les effectifs d'une soirée (P) : `6 OPERATIONS/PRODUCTION/2026 1028 Calculateur de staffing par événement.xlsx` et la note « Typologie des événements, process et staffing ». Ils ne donnent ni les heures ni les coûts horaires.
- **I** Hypothèses centrales retenues :
  - lieu payé au prix du marché ;
  - remplissage de 80 % ;
  - TVA moyenne de 12 % ;
  - équipe de chaque soirée selon les effectifs des Opérations, avec des heures et des coûts horaires en hypothèse (onglet « Staffing » du modèle Prévisions).

  Le staffing des Opérations change fortement le résultat :

  | Soirée | Personnes payées (hors chef et fondateurs) | Coût de l'équipe | Hypothèse du 27/10 (cible du Produit) |
  |---|---|---|---|
  | Premier soir | 13 | 3 636 € | 870 € |
  | Le Voyage | 13 | 3 636 € | 1 080 € |
  | La Grande Nuit | 11 | 3 076 € | 1 350 € |
  | Privatisation (table de 10) | 7 | 2 040 € | 950 € |

  Avec ces hypothèses, les trois soirées de l'offre A perdent nettement de l'argent, et la privatisation est à peine à l'équilibre :

  | Soirée | Marge par soirée | Taux | Remplissage d'équilibre | Prix plancher TTC par convive |
  |---|---|---|---|---|
  | Premier soir | −3 620 € | −74 % | 168 % | 507 € (affiché 290 €) |
  | Le Voyage | −3 419 € | −48 % | 139 % | 636 € (affiché 420 €) |
  | La Grande Nuit | −4 078 € | −41 % | 134 % | 1 013 € (affiché 690 €) |
  | Privatisation | +142 € | +2 % | 91 % | 282 € (affiché 300 €) |
- **I** Aucune soirée de l'offre A n'atteint l'équilibre, même salle pleine. Le seuil de confirmation de 70 % proposé par le Produit ne garantit pas l'équilibre.
- **I** Deux postes pèsent le plus : l'équipe de la soirée et le restaurateur.
  - **L'équipe** : si le restaurant fournit le personnel de salle, le coût de notre équipe descend à 2 051 € (Premier soir et Voyage), 1 736 € (Grande Nuit) et 945 € (privatisation). Les marges deviennent −2 035 €, −1 834 €, −2 738 € et +1 237 €. Mais la part du restaurateur augmenterait d'autant, ce que le modèle ne chiffre pas.
  - **Le restaurateur** : le Produit vise 11 à 12 % du prix, soit 750 à 1 350 € par soirée. Les prix de location observés sont plus élevés :
    - **F** Giggster : de 35 à 620 €/h, moyenne d'environ 373 à 386 €/h ;
    - **F** Privateaser : « à partir de 2 916 € ».

    Ces deux sources sont citées dans `3 MARKETING/old project/MARCHE/`. Si le restaurateur accepte la part visée par le Produit et que la salle est pleine, avec le staffing des Opérations, les marges sont de −2 017 € (Premier soir), −1 808 € (Le Voyage), −1 419 € (La Grande Nuit) et +1 178 € (privatisation).
- **I** Budget de l'année 1 (novembre 2026 à octobre 2027, H : 16 soirées dont 7 privatisations) :
  - chiffre d'affaires : 121 955 € HT ;
  - marge sur coûts directs : −32 358 € ;
  - frais généraux : 12 672 €, dont 0 € de ressources humaines (fondateurs non rémunérés) et 12 672 € de frais matériels et de fonctionnement ;
  - résultat : −45 030 €.

  Simulation de trésorerie, avec un apport de 7 000 € et 3 000 € d'investissements en novembre : le compte passerait sous zéro dès décembre 2026 et finirait à −41 030 € en octobre 2027.
- **I** Plan à 3 ans (frais généraux détaillés poste par poste le 28/10/2026) :

  | Frais généraux | Année 1 | Année 2 | Année 3 |
  |---|---|---|---|
  | Ressources humaines | 0 € | 32 486 € | 168 206 € |
  | Frais matériels et de fonctionnement | 12 672 € | 24 300 € | 57 800 € |
  | **Total** | **12 672 €** | **56 786 €** | **226 006 €** |

  Les ressources humaines comprennent :
  - un coordinateur ou une coordinatrice au SMIC dès l'année 2 ;
  - deux fondateurs rémunérés et un commercial ou une commerciale en année 3 ;
  - des charges patronales de 45 % (H).

  Avec le staffing des Opérations, le besoin de financement est de 557 940 € en hypothèses centrales (309 726 € avant le staffing). Il est d'environ 341 000 € avec la part du restaurateur visée par le Produit et la salle pleine.
- **P** Quatre chiffres décident du modèle :
  1. qui assure le service de salle (le restaurant ou nous) et à quel coût horaire ;
  2. ce que le restaurateur accepte pour un soir de fermeture ;
  3. le cachet des chefs ;
  4. le remplissage réel.

  Ce sont les premières données à obtenir, avant d'arrêter les prix. Avec les effectifs proposés, les prix de l'offre A ne couvrent pas les coûts : il faudra revoir soit les prix, soit le format (par exemple moins de services, ou une équipe plus réduite en criticité C1).

## 2. Données disponibles reprises

| Donnée | Valeur | Nature | Source |
|---|---|---|---|
| Prix TTC par convive des soirées | 290 € / 420 € / 690 € | P | `5 PRODUIT/Fou d'un soir le pricing.md` |
| Couverts par soirée | 24 / 24 / 20 | P | idem et `5 PRODUIT/Fou d'un soir l'offre.md` |
| Privatisation chef confirmé | Forfait 6 000 € + 300 € par convive ; exemple d'une table de 10 | P | `5 PRODUIT/Fou d'un soir le pricing.md` |
| Répartition cible du prix HT | Matières et vins 33 / 30 / 27 % ; chef 15 / 22 / 30 % ; restaurateur 12 / 12 / 11 % ; service 14 / 12 / 11 % ; frais 8 / 6 / 5 % ; marge 18 / 18 / 16 % | P | idem, « La logique de pricing » |
| Rythme | Une soirée par mois au lancement ; pilotes à environ cinq semaines d'écart ; seuil de 70 % à J-14 | P | `5 PRODUIT/Fou d'un soir l'offre.md` ; plan des deux soirées pilotes |
| Chef privé à domicile | 500 à 1 400 € par jour et par chef, hors matières | F | Chefs Talents 2026, cité dans `3 MARKETING/new project/3 Concurrence/` |
| Location de restaurants à Paris | 35 à 620 €/h, moyenne environ 373 à 386 €/h ; privatisation à partir de 2 916 € | F | Giggster, Privateaser, cités dans `3 MARKETING/old project/MARCHE/` |
| Ratio matières et boissons | Idéalement sous 35 % du prix | F | Keobiz, cité dans le descriptif du projet 3 (`PRODUCTIONS ASSISTANTS/`) |
| Honoraires d'agence événementielle | 10 à 20 % du budget | F | BlackTrombone 2026, idem |
| Frais de carte bancaire | 1,5 % + 0,25 € par carte européenne | F | Stripe, page tarifs, consultée le 27/10/2026 |
| Création d'une SAS | 252 € | F | LegalPlace, 06/08/2026, cité dans [[2026 1027 Synthèse marketing, étude de marché et coûts de lancement]] |
| Assurance RC pro d'une start-up en amorçage | 200 à 300 € par an | F | Coover 2026, idem |
| SMIC | 1 867,02 € brut par mois au 01/06/2026 | F | Éditions Tissot, idem |
| Photographe indépendant | 410 à 520 € par jour | F | Malt, via Modèles de Business Plan, 15/09/2026, idem |
| Nombre de membres de l'équipe | 7 (un responsable par fonction) | F | `README.md` |
| Effectifs d'une soirée (hors chef) | Premier soir et Le Voyage 15, La Grande Nuit 13, table de 10 : 9, dont 2 assurés par nous (production, interlocuteur client) | P | `6 OPERATIONS/PRODUCTION/2026 1028 Calculateur de staffing par événement.xlsx` (catégorie C2) |

## 3. Données manquantes, hypothèses temporaires et qui peut les fournir

Priorité : 1 = elle change le modèle, à obtenir avant les pilotes · 2 = utile pour le budget · 3 = utile pour le financement.

| # | Donnée manquante | Où elle sert | Hypothèse temporaire (H) | Qui peut la fournir | Priorité |
|---|---|---|---|---|---|
| 1 | Indemnité demandée par un restaurateur pour un soir de fermeture, minimum garanti, ce que couvre la mise à disposition (cuisine, vaisselle, personnel) | Prévisions, Prix et marges, ligne 19 | 1 500 € (Premier soir, Voyage), 2 500 € (Grande Nuit), 2 000 € (privatisation) | Ventes (@xavierjuraflo-ship-it), lors des premiers échanges avec des restaurateurs ; Opérations (@jonathanstarke-hec) pour le périmètre | 1 |
| 2 | Cachet des chefs par niveau (montant, confirmé, étoilé, étranger), déplacement et hébergement, accord de la maison d'origine | Ligne 20 | 950 € / 2 000 € / 3 700 € / 1 800 €, entièrement fixes | Ventes et Opérations (carnet de chefs) ; Direction (@Laetitiarv) pour l'associé gastronomique | 1 |
| 3 | Taux de remplissage réaliste et disposition à payer de chaque persona | Ligne 8 ; budget | 80 % pour l'offre A ; 100 % pour la privatisation | Marketing (@serge2309), par des entretiens et la liste privée ; mesure réelle aux pilotes | 1 |
| 4 | Coût matières par menu et coût des accords mets-vins et mets-jus | Lignes 23 et 24 | 85 € / 112 € / 166 € / 80 € par convive (cible du Produit) | Opérations, avec le chef et le sommelier ; devis fournisseurs et cavistes | 1 |
| 5 | Qui assure le service (équipe du restaurant ou la nôtre), heures par poste, coût horaire chargé de chaque poste, cachet du sommelier invité. **Effectifs reçus le 28/10/2026** (Opérations, P) | Onglet « Staffing » ; Prix et marges, ligne 26 | Heures : brigade 9 h, maître d'hôtel 8 h, salle, sommellerie et plonge 7 h. Coûts horaires : 35 €/h (brigade, serveurs), 45 € (maître d'hôtel), 60 € (sommelier invité), 38 € (aide sommelier), 30 € (plonge). Postes internes non rémunérés en année 1. Résultat : 3 636 € / 3 636 € / 3 076 € / 2 040 € par soirée | Opérations (@jonathanstarke-hec), devis d'agences d'extras (action n° 4 de leur note) ; Produit (@Fredlay26) et Direction pour la décision sur le service de salle | 1 |
| 6 | Taux de TVA applicables : repas, boissons alcoolisées, forfait de privatisation, bons cadeaux | Ligne 12 ; tous les HT | 12 % de taux moyen | Expert-comptable, sollicité par la Finance ; Juridique (@alexanderzhelev-dev) pour les bons cadeaux | 1 |
| 7 | Part des ventes passant par des concierges ou des agences, et commission demandée | Ligne 31 | 0 % / 5 % / 10 % / 10 % | Marketing (stratégie des concierges) ; Ventes | 2 |
| 8 | Nombre de soirées par an que le carnet de lieux et de chefs permet, et calendrier | Budget mensuel ; plan à 3 ans | 9 soirées A et 7 privatisations en année 1 ; 24 et 24 en année 2 ; 36 et 48 en année 3 | Produit et Opérations ; décision de la Direction | 2 |
| 9 | Demande de privatisations et de contrats cadres (maisons de luxe, hôtes d'affaires) | Budget ; plan | Première privatisation en avril 2027, 2 par mois en septembre et octobre | Ventes (pipeline, premiers rendez-vous) | 2 |
| 10 | Assurance de la soirée et RC professionnelle d'une société d'événementiel | Ligne 28 ; budget | 150 € par soirée ; 50 € par mois | Juridique, par des devis d'assureurs | 2 |
| 11 | Budget de communication, coût des dîners de concierges, coût du photographe | Budget mensuel, ligne 25 ; Prix et marges, ligne 33 | 300 € par mois + 3 dîners à 1 200 € ; 260 € par soirée | Marketing | 2 |
| 12 | Outils : site, billetterie, fichier clients | Budget mensuel, ligne 24 ; investissements | 80 € par mois ; 3 000 € d'investissement | Produit | 2 |
| 13 | Honoraires de l'expert-comptable et des contrats types | Budget mensuel, ligne 27 | 100 € par mois ; 1 500 € en novembre | Juridique ; devis d'expert-comptable | 2 |
| 14 | Revenus de partenariats (maisons de vins et de champagne, co-signature) | Ligne 16 | 0 € | Ventes | 2 |
| 15 | Règles d'encaissement : paiement à la réservation, acomptes des contrats cadres, délais de paiement des entreprises, remboursements | Trésorerie | Encaissement le mois de la soirée, sans remboursement | Produit (règles de vente) ; Ventes (conditions des entreprises) | 2 |
| 16 | Rémunération des fondateurs, recrutements des années 2 et 3, taux de charges patronales | Onglet « Frais généraux 3 ans », partie Ressources humaines ; budget mensuel, lignes 17 à 21 | 0 € en année 1 ; un coordinateur ou une coordinatrice au SMIC dès l'année 2 ; deux fondateurs à 2 500 € brut et un commercial ou une commerciale à 2 800 € brut en année 3 ; charges de 45 % | Direction ; Juridique (`7 JURIDIQUE/EQUIPE/`) ; expert-comptable pour le taux de charges | 2 |
| 16 bis | Frais matériels et de fonctionnement des années 2 et 3 (locaux, outils, marketing, assurance, honoraires, banque, déplacements) | Onglet « Frais généraux 3 ans », partie Frais matériels | 24 300 € en année 2, 57 800 € en année 3, dont un coworking en année 3 | Marketing (budget de communication) ; Produit (outils) ; Juridique (assurance, honoraires) | 2 |
| 17 | Associés, capital social, répartition des titres, date de création de la société | Financement, table de capitalisation ; trésorerie de départ | 7 associés à 1 000 € chacun, création au 01/11/2026 | Direction ; Juridique (`STATUTS ET PACTE/`) | 3 |
| 18 | Financements possibles : prêt d'honneur, subventions, concours, levée, associé gastronomique | Financement, suivi | Statut « Envisagé » pour tous : 20 000 € de prêt d'honneur, 5 000 € de subvention, 100 000 € de levée sur 400 000 € de valorisation | Finance (dossiers à identifier) ; Direction (associé gastronomique) | 3 |
| 19 | Ouverture du compte bancaire et premier relevé | Trésorerie, états | Solde de 7 000 € au 01/11/2026, sans pièce | Finance, après l'immatriculation (Juridique) | 3 |

## 4. Contradictions et points signalés

- **I** La part du restaurateur visée par le Produit (11 à 12 % du prix HT) est inférieure aux prix de location observés sur le marché (voir § 1). Le Produit le signale lui-même : « il faudra un chiffre clair et, sans doute, un minimum garanti ». Les fichiers retiennent le prix du marché (H). Ce choix est à trancher par la donnée n° 1.
- **I** Le seuil de confirmation de 70 % est un seuil de vente, pas un seuil de rentabilité. Avec les hypothèses centrales et le staffing des Opérations, aucune soirée de l'offre A n'est rentable, même salle pleine (remplissage d'équilibre de 134 à 168 %).
- **I** Les effectifs des Opérations (13 personnes payées pour 24 couverts) et la répartition cible du Produit (équipe de service = 11 à 14 % du prix) ne sont pas compatibles aux prix affichés : l'équipe coûterait 31 à 74 % du chiffre d'affaires d'une soirée de l'offre A. Les deux pôles doivent en parler avant les pilotes.
- **I** Les prix du Produit sont TTC, tout compris. Avec une TVA moyenne de 12 %, le prix HT est inférieur de 11 % au prix affiché : la répartition cible du Produit doit s'appliquer au prix HT.
- **I** Le budget de l'année 1 repose sur la première année d'activité de pilotes. Il n'est pas comparable au plan du descriptif du projet 3 (30 événements de 40 convives), qui portait sur un autre format.

## 5. Prochaines étapes proposées

1. **P** Obtenir de deux ou trois restaurateurs une fourchette d'indemnité pour un soir de fermeture (Ventes), et de deux chefs par niveau un cachet indicatif (Ventes, Opérations).
2. **P** Faire confirmer les taux de TVA par un expert-comptable.
3. **P** Recalculer alors les prix planchers (onglet Prix et marges, lignes 42 et 43), puis proposer à l'équipe un ajustement de prix ou de format : moins de couverts mais plus chers, ou un minimum par soirée. La décision revient à l'équipe et va au registre des décisions.
4. **P** Remplacer chaque H par le chiffre obtenu, en passant la colonne Nature à F et en citant la pièce. Après les pilotes, remplir l'onglet « Prévu et réel ».
