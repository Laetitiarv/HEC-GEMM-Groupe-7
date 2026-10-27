# Pop-up de chefs renommés dans des restaurants d'exception les soirs de fermeture — description du projet et données pour dimensionner le marché

Date : 27/10/2026 · Production d'assistant IA, à la demande de Serge Muller · Statut : document de travail, nouvelle orientation proposée, non validée par l'équipe

Légende (voir [[RULES]]) : F = fait constaté sur la source citée · I = inférence · P = proposition · H = hypothèse chiffrée à valider. Les chiffres publiés par une entreprise sur elle-même sont des argumentaires.

## 1. Description du projet

À Paris, une large majorité de restaurants ferment au moins un jour par semaine. Parmi eux, certains sont des lieux remarquables : décoration soignée, confort, vue, terrasse ou rooftop, adresse prestigieuse. Ces soirs-là, la salle, la cuisine et le décor sont immobilisés et ne rapportent rien à leur exploitant, qui continue pourtant de payer son loyer et ses charges fixes.

Le projet consiste à transformer ces soirées vides en événements rares. La plateforme sélectionne des restaurants d'exception et convient avec chaque restaurateur des soirs de fermeture qu'il accepte d'ouvrir. Elle loue alors le lieu, pour une ou deux soirées, à un chef à forte notoriété : chef étoilé ou distingué par les guides, ancien des grandes maisons, Meilleur Ouvrier de France, chef médiatisé par la télévision, chef ayant cuisiné pour une clientèle prestigieuse. Le parcours du chef (formation, maisons où il a travaillé, chefs auprès desquels il s'est formé, distinctions, notoriété publique) est l'argument de vente de la soirée.

La plateforme annonce ensuite ce pop-up à son réseau de clients : un chef reconnu, un lieu d'exception, une ou deux soirées seulement, un nombre de couverts limité. La rareté et la combinaison lieu et chef font la valeur de l'expérience.

Le modèle économique de base est un loyer éphémère : le chef paie la location du lieu pour la soirée à la plateforme, qui en reverse un pourcentage au restaurateur et conserve la différence. P D'autres revenus pourront être étudiés plus tard (billetterie, partenariats avec des maisons de vins ou de champagne, privatisations pour des entreprises), mais ils ne sont pas pris en compte dans le dimensionnement ci-dessous.

Ce que chacun y gagne : le restaurateur, un revenu sur une soirée qui ne lui rapporte rien et une visibilité auprès d'une clientèle aisée ; le chef, une scène prestigieuse sans investissement, un test de concept ou une étape de notoriété ; le client, une expérience gastronomique rare dans un lieu qu'il ne connaît pas ou ne fréquente pas sous cet angle.

## 2. Comment se calcule la taille du marché

Revenu de la plateforme = nombre de soirées louées × loyer moyen d'une soirée × part conservée par la plateforme (1 − pourcentage reversé au restaurateur).

Pour l'estimer, il faut quatre familles de données : l'offre de lieux (combien de restaurants d'exception, combien de soirs de fermeture), l'offre de chefs (combien de chefs assez connus pour remplir une salle), la demande des clients finaux (qui paie, combien, à quelle fréquence), et le prix d'une soirée (ce qu'un chef peut payer pour louer un lieu). Les sections 3 à 6 donnent ce qui a été trouvé ; la section 7 fait un premier calcul ; la section 8 liste ce qui manque.

## 3. Offre de lieux : les restaurants et leurs soirs de fermeture

| Donnée | Valeur | Source (date) |
|---|---|---|
| Établissements de restauration actifs à Paris (périmètre large, incluant débits de boissons et traiteurs) | F 38 319 | [Kouizine, observatoire des restaurants à Paris](https://kouizine.com/observatoire/restaurants/paris), données SIRENE, édition de juin 2026 |
| dont restaurants traditionnels | F 17 858 (46,6 %) | Même source |
| dont restauration rapide | F 12 586 | Même source |
| Commerces de toute nature à Paris | F 60 846 ; taux de vacance des rez-de-chaussée 10,9 % | [APUR, les commerces à Paris en 2023](https://www.apur.org/en/economy-employment/business/retailers-paris-2023) |
| Jours d'ouverture par semaine des restaurants | F 6 jours sur 7 : 46 % ; 5 jours sur 7 : 27 % ; 7 jours sur 7 : 26 % | [Auvergne-Rhône-Alpes Tourisme, fiche ratios restaurant](https://archives-pro.auvergnerhonealpes-tourisme.com/wp-content/uploads/2021/11/FicheRatio_restaurant.pdf), données 2018-2019, périmètre non limité à Paris |
| Restaurants étoilés à Paris | F 127 (9 trois étoiles, 20 deux étoiles, 98 une étoile) | [Paris Gourmand, palmarès Michelin 2026](https://www.parisgourmand.com/dernieres-news/le-guide-michelin-2026-est-paru-paris-brille-encore-le-palmares-complet.html), mars 2026 |
| Autorisations de terrasses et étalages à Paris | F 23 070 (un même établissement peut en avoir plusieurs ; inclut des commerces non alimentaires) | [Données Ville de Paris, compilation F. Geerolf](https://fgeerolf.com/data/paris/terrasses-autorisations.html), mise à jour du 25/10/2026 |
| Restaurants privatisables listés à Paris sur Giggster | F 134 | [Giggster, restaurants à Paris](https://giggster.com/fr/find/paris--fr/restaurant), consulté le 27/10/2026 |

I D'après la répartition des jours d'ouverture, environ 73 % des restaurants ferment au moins un jour par semaine, soit en moyenne un jour de fermeture hebdomadaire par restaurant (46 % × 1 jour + 27 % × 2 jours). Ce ratio date d'avant 2020 et ne porte pas spécifiquement sur Paris ni sur les soirs ; il doit être vérifié sur un échantillon de lieux ciblés.

Non établi par les sources : le nombre de restaurants parisiens qui répondent au critère « lieu d'exception » (décor, confort, vue, terrasse, rooftop). Aucun recensement n'existe ; il faudra le construire (voir section 8).

## 4. Offre de chefs : le vivier de notoriété

| Donnée | Valeur | Source (date) |
|---|---|---|
| Restaurants étoilés en France et à Monaco | F 668 (31 trois étoiles, 84 deux étoiles, 553 une étoile) | [Les Meilleurs Restaurants, Michelin 2026](https://www.lesmeilleursrestaurants.fr/restaurants-etoiles-france/) |
| Tables trois étoiles en France et à Monaco, et nombre de chefs | F 31 tables, tenues par 29 chefs | [Au cœur du CHR, Observatoire de la Haute Cuisine](https://aucoeurduchr.fr/article/conjoncture/le-marche-haute-gastronomie-france-pese-plus-de-600-millions-deuros/), 16/03/2026 |
| Restaurants 4 toques Gault&Millau en France | F 63 | [Gault&Millau](https://fr.gaultmillau.com/fr/news/quelles-sont-les-nouvelles-tables-4-toques-du-guide-gault-millau-en-2026), 2026 |
| Meilleurs Ouvriers de France, tous métiers confondus | F 9 006 diplômés depuis 1925, près de 200 lauréats par promotion ; le nombre propre à la cuisine n'est pas donné | [Journal des Palaces](https://www.journaldespalaces.com/communique-53398-le-concours-un-des-meilleurs-ouvriers-de-france-la-valorisation-des-savoir-faire-d-excellence.html) |
| Top Chef (M6), saison 17 | F 16 candidats ; audience moyenne de 1,47 million puis 1,25 million de téléspectateurs selon la partie de la saison | [Ozap, candidats](https://www.ozap.com/actu/top-chef-2026-decouvrez-les-visages-des-16-candidats-de-la-saison-17/653738), 04/03/2026 ; [Ozap, audiences](https://www.ozap.com/actu/audiences-pire-bilan-historique-pour-la-saison-17-de-top-chef-sur-m6/655511), 11/06/2026 |

I Les chefs étoilés en exercice ont déjà leur propre maison et un calendrier chargé ; le vivier le plus accessible est probablement celui des anciens seconds de grandes maisons, des chefs en transition entre deux projets, des candidats et finalistes de concours télévisés, et des chefs étrangers de passage à Paris. À vérifier par entretiens.

## 5. Demande des clients finaux et prix des dîners

| Donnée | Valeur | Source (date) |
|---|---|---|
| Prix des menus de pop-up et résidences de chefs à Paris, automne 2025 | F 70 € à 250 € par personne selon le chef et le lieu (exemples : 70 €, 75 €, 175 €, 250 € hors boissons) | [Fine Dining Lovers](https://www.finedininglovers.fr/explorer/articles/pop-up-food-automne-2025), 20/09/2025 |
| Prix des menus des pop-up d'hiver dans les palaces parisiens | F 120 € à 225 € par personne (Plaza Athénée, La Réserve, Park Hyatt) | [Guide Michelin](https://guide.michelin.com/fr/fr/article/news-and-views/paris-2026-5-restaurants-et-bars-ephemeres-a-ne-pas-rater), 07/01/2026 |
| Ticket moyen des tables trois étoiles | F environ 380 € par personne à Paris, 310 € en région, hors boissons | [Au cœur du CHR, Observatoire de la Haute Cuisine](https://aucoeurduchr.fr/article/conjoncture/le-marche-haute-gastronomie-france-pese-plus-de-600-millions-deuros/), 16/03/2026 |
| Marché de la haute gastronomie (écosystème des trois étoiles) | F 608 M€ HT, dont 185 M€ d'activité de restauration ; Paris pèse 51 %, soit environ 94 M€ de restauration ; croissance annuelle moyenne de 5,9 % sur cinq ans | Même source |
| Prix observés par gamme à Paris (échantillon d'un blog, plus de 200 restaurants) | F menus gastronomiques 80 à 180 € ; dîner une étoile 90 à 160 € ; deux et trois étoiles 180 à 500 € | [FoodyParis](https://www.foodyparis.com/blog/combien-coute-repas-paris-2026-etude-quartier), 29/03/2026 (argumentaire, méthode peu détaillée) |
| Réservations en ligne : poids de Paris | F 41 % des réservations de TheFork en France ; 70 % des réservations sont des dîners ; 71 millions de couverts et 2,1 Md€ de dépenses sur un an | [TheFork Manager, bilan 2024](https://www.theforkmanager.com/fr/blog/nouvelles-et-evenements/thefork-dresse-le-bilan-annuel-2024-du-secteur-de-la-restauration-la) |
| Fréquentation touristique de Paris Île-de-France | F près de 50 millions de visiteurs et près de 24 Md€ de retombées en 2025 ; clientèle internationale en hausse de 3 % | [Visit Paris Region](https://pro.visitparisregion.com/offre-loisirs-et-affaires/evenements/actualites2/communique-de-presse-bilan-annuel-2025-frequentation-touristique-a-paris-ile-de-france), 24/03/2026 |
| Ménages aisés (indicateur : redevables de l'impôt sur la fortune immobilière) | F 193 625 foyers en France en 2025 ; Paris représentait 26 % des déclarants en 2022 | [MoneyVox, DGFiP](https://www.moneyvox.fr/impot/actualites/108493/impots-sur-immobilier-le-top-10-des-villes-ou-se-nichent-les-plus-riches-proprietaires) ; [Linxea, DGFiP](https://www.linxea.com/actualites/toutes-les-actualites/paris-hauts-de-seine-et-yvelines-en-tete-des-redevables-de-lifi/) |

I Les palaces parisiens organisent déjà eux-mêmes des pop-up et des résidences de chefs, à 120 à 250 € par personne (Mandarin Oriental Lutetia, Plaza Athénée, Park Hyatt, La Réserve, Ducasse Baccarat). Cela prouve qu'une clientèle paie ces prix pour ce type d'expérience ; c'est aussi le premier concurrent du projet.

## 6. Prix d'une soirée : ce qu'un chef peut payer pour un lieu

| Donnée | Valeur | Source (date) |
|---|---|---|
| Location de restaurants à l'heure à Paris (Giggster) | F de 35 €/h à 620 €/h selon les annonces ; coût moyen tous lieux confondus de 373 à 386 €/h selon les pages | [Giggster, restaurants](https://giggster.com/fr/find/paris--fr/restaurant) ; [Giggster, dîners d'anniversaire](https://giggster.com/fr/find/paris--fr/birthday-dinner), consultés le 27/10/2026 |
| Privatisation d'une table d'hôtes parisienne (Privateaser) | F un exemple affiché « à partir de 2 916 € » ; la plupart des lieux sont sur devis | [Privateaser](https://www.privateaser.com/fete/top-restaurants-privatisation-mariage-paris), consulté le 27/10/2026 |
| Restaurants éphémères à Londres (Appear Here) | F à partir de 150 £ par jour | Fiche du 26/10, § 1.2 |
| Couverts moyens par restaurant en France | F 63 en 2019 (57 en 2014) ; 2 à 3 m² par place en restauration traditionnelle | [Auvergne-Rhône-Alpes Tourisme](https://archives-pro.auvergnerhonealpes-tourisme.com/wp-content/uploads/2021/11/FicheRatio_restaurant.pdf) |
| Modèles de résidence de chef existants | F à Paris, Fulgurances accueille un chef en résidence tous les 3 à 6 mois, salarié en CDD ; ailleurs, des chefs indépendants sont rémunérés par une part des bénéfices | [L'Hôtellerie Restauration](https://www.lhotellerie-restauration.fr/actualite/chefs-en-residence-un-enrichissement-mutuel), 16/05/2018 |

Contrôle de cohérence par l'économie du chef (H) : une soirée de 30 couverts à 150 € rapporte 4 500 € au chef ; 40 couverts à 175 € rapportent 7 000 € ; 50 couverts à 250 € rapportent 12 500 €. Si le loyer du lieu représente 20 à 30 % de ces recettes, il se situe entre environ 900 € et 3 750 € la soirée, soit, pour la soirée centrale, 1 400 à 2 100 €. Cette fourchette est compatible avec les prix de location observés (environ 300 à 400 €/h sur une soirée de cinq heures).

## 7. Premier dimensionnement (calculs illustratifs)

Toutes les lignes marquées H sont des hypothèses à remplacer par des données de terrain.

Marché théorique des soirées disponibles (offre de lieux) :

| Étape | Bas | Haut |
|---|---|---|
| Restaurants traditionnels à Paris (F) | 17 858 | 17 858 |
| Part jugée « d'exception » (H) | 3 % | 5 % |
| Lieux d'exception | environ 536 | environ 893 |
| Jours de fermeture moyens par semaine (I, section 3) | 1,0 | 1,0 |
| Semaines exploitables par an, hors fermeture annuelle (H) | 48 | 48 |
| Soirées disponibles par an | environ 25 700 | environ 42 900 |
| Loyer moyen d'une soirée (H, section 6) | 1 500 € | 2 500 € |
| Valeur théorique des loyers | environ 39 M€ | environ 107 M€ |

I Ce chiffre est un plafond : il suppose que chaque soir de fermeture de chaque lieu d'exception trouve preneur. La vraie limite est la demande, c'est-à-dire le nombre de chefs capables de remplir une salle à ces prix et le nombre de clients prêts à payer.

Ordre de grandeur atteignable par la plateforme (part de marché réaliste) :

| Rythme de pop-up | Soirées par an | Loyers encaissés (1 500 à 2 500 € la soirée) | Revenu de la plateforme si elle conserve 30 % | si elle conserve 40 % |
|---|---|---|---|---|
| 1 soirée par semaine | 52 | 78 000 à 130 000 € | 23 400 à 39 000 € | 31 200 à 52 000 € |
| 2 soirées par semaine (un pop-up de 2 soirs) | 104 | 156 000 à 260 000 € | 46 800 à 78 000 € | 62 400 à 104 000 € |
| 4 soirées par semaine (deux pop-up de 2 soirs) | 208 | 312 000 à 520 000 € | 93 600 à 156 000 € | 124 800 à 208 000 € |

I Avec un modèle fondé uniquement sur le loyer, le revenu de la plateforme reste modeste, même à un rythme soutenu. Pour mémoire, 104 soirées de 40 couverts à 175 € représentent environ 728 000 € de dîners vendus : la valeur se crée surtout dans la billetterie et l'expérience, que le modèle actuel laisse au chef. P C'est le premier arbitrage à poser : loyer seul, ou loyer plus commission sur les places vendues au réseau de clients de la plateforme.

## 8. Données manquantes et comment les obtenir

Le nombre de restaurants d'exception à Paris : constituer une liste à partir des sélections des guides (Michelin, Gault&Millau, Le Fooding), des classements de rooftops et de terrasses, et des restaurants privatisables sur Privateaser et Giggster, puis la croiser. Les jours de fermeture réels de ces lieux : relevé sur leurs fiches en ligne (Google, TheFork) pour un échantillon d'une centaine d'adresses. La part de restaurateurs prêts à confier leur lieu un soir de fermeture, et le pourcentage du loyer qu'ils attendent : entretiens avec dix à vingt restaurateurs (pôle Ventes). Ce qu'un chef connu accepterait de payer pour une soirée, et combien de chefs sont disponibles : entretiens avec des chefs et des agents de chefs. La taille et la fréquence d'achat du réseau de clients : questionnaire auprès d'une clientèle cible, et données des programmes de fidélité existants. Les contraintes pratiques : assurance, licence de débit de boissons, règles d'hygiène, accès à la cuisine et aux stocks du restaurateur, responsabilité en cas de dommage (pôle Juridique).

Décision à prendre par : l'équipe (voir [[REGISTRE DES DECISIONS]]). Ce document décrit une nouvelle orientation et rassemble des données ; il ne décide rien.
