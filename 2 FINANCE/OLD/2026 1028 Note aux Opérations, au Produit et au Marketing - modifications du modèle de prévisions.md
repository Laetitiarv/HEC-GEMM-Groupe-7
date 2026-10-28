# Note aux Opérations, au Produit et au Marketing : modifications du modèle de prévisions

**Date : 28/10/2026** · Fonction : `2 FINANCE` · Destinataires : Opérations (@jonathanstarke-hec), Produit (@Fredlay26), Marketing (@serge2309) · Auteur : assistant IA Finance, à la demande de Vianney (responsable Finance) · Statut : document de travail. Rien n'est décidé (voir [[REGISTRE DES DECISIONS]]).

Légende (voir [[RULES]]) : **F** = fait constaté dans le fichier · **I** = inférence · **P** = proposition · **H** = hypothèse.

> **En bref.** Le 28/10/2026, le responsable Finance a modifié quatre hypothèses du modèle Prévisions :
> - la capacité des soirées ;
> - le taux de remplissage ;
> - le coût de l'équipe ;
> - le photographe.
>
> Avec ces hypothèses, toutes les soirées deviennent rentables et l'année 1 passe d'une perte de 40 620 € à un bénéfice de 15 913 €. Le besoin de financement à 3 ans passe de 517 330 € à 32 140 €.
>
> Ces nouvelles valeurs sont des **hypothèses (H)**. Elles diffèrent des propositions du Produit et des Opérations, et chaque pôle doit dire si elles sont tenables (§ 4).

Fichier : `2 FINANCE/PREVISIONS/2026 1027 Modèle - Budget, plan financier, prix et marges.xlsx`, onglet « Prix et marges ». Comparaison faite avec la version du commit c592e3c.

---

## 1. Les modifications (F)

14 cellules ont changé, toutes dans l'onglet « Prix et marges ». Les autres onglets ne sont pas modifiés.

| Ligne | Hypothèse | Premier soir | Le Voyage | La Grande Nuit | Privatisation |
|---|---|---|---|---|---|
| 7 | Capacité (couverts) | 24 → **40** | 24 → **35** | 20 → **30** | 10 → **20** |
| 8 | Taux de remplissage | 80 % → **100 %** | 80 % → **100 %** | 80 % → **100 %** | 100 % (inchangé) |
| 26 | Coût de l'équipe de la soirée | Onglet Staffing (S3) → **15 % du CA HT** | Staffing (S3) → **20 % du CA HT** | Staffing (S3) → **20 % du CA HT** | Staffing → **15 % du CA HT** |
| 33 | Photographe | 260 € → **0 €** | 260 € → **0 €** | 260 € → **0 €** | 0 € (inchangé) |

**Les prix restent ceux du Produit** : 290 €, 420 € et 690 € TTC par convive, et pour la privatisation 6 000 € de forfait plus 300 € par convive. Les coûts du lieu et du chef ne changent pas non plus.

## 2. Effet par soirée (F, calculé par le modèle)

| | Premier soir | Le Voyage | La Grande Nuit | Privatisation |
|---|---|---|---|---|
| Convives payants | 19 → 40 | 19 → 35 | 16 → 30 | 10 → 20 |
| Chiffre d'affaires HT | 4 920 € → 10 357 € | 7 125 € → 13 125 € | 9 857 € → 18 482 € | 8 036 € → 10 714 € |
| Coût de l'équipe | 2 936 € → 1 554 € | 2 936 € → 2 625 € | 2 621 € → 3 696 € | 2 040 € → 1 607 € |
| Matières et boissons | 1 615 € → 3 400 € | 2 128 € → 3 920 € | 2 656 € → 4 980 € | 800 € → 1 600 € |
| **Marge de la soirée** | −2 920 € → **+2 288 €** | −2 719 € → **+1 664 €** | −3 623 € → **+862 €** | +142 € → **+2 186 €** |
| Taux de marge | −59 % → 22 % | −38 % → 13 % | −37 % → 5 % | +2 % → 20 % |
| Prix plancher TTC par convive | 465 € → 225 € | 592 € → 363 € | 977 € → 654 € | 282 € → 164 € |
| Remplissage d'équilibre | 151 % → **66 %** | 127 % → **80 %** | 128 % → **92 %** | 91 % → **32 %** |

## 3. Effet sur le budget et le plan (F, calculé par le modèle)

| | Avant | Après |
|---|---|---|
| Chiffre d'affaires, année 1 | 121 955 € | 200 893 € |
| Marge sur coûts directs, année 1 | −27 948 € | +28 585 € |
| **Résultat, année 1** | **−40 620 €** | **+15 913 €** |
| Résultat, années 2 et 3 | −127 776 € et −330 935 € | +33 878 € et −63 931 € |
| **Besoin de financement à 3 ans** | **517 330 €** | **32 140 €** |
| Crédit de TVA en fin d'année 1 | 8 741 € | 1 451 € |

**I** L'année 3 reste en perte (−63 931 €). La marge des soirées ne couvre pas encore les frais généraux prévus cette année-là (226 606 €, dont les premiers salaires des fondateurs). Le point mort serait atteint vers 117 soirées par an, pour 84 soirées prévues (36 soirées de l'offre A et 48 privatisations).

**I** Le nombre de soirées par mois n'a pas changé (16 en année 1). Toute l'amélioration vient donc du chiffre d'affaires par soirée et du coût de l'équipe.

---

## 4. Ce que chaque pôle doit confirmer

### Opérations
1. **Coût de l'équipe.** Le modèle ne calcule plus ce coût à partir des effectifs : il le fixe à 15 % ou 20 % du chiffre d'affaires. **I** Pour le Premier soir, cela donne 1 554 € pour 40 couverts, contre 2 936 € pour 24 couverts dans votre scénario S3. Avec votre règle d'un serveur pour 9 couverts, 40 couverts demandent 5 serveurs, contre 3 en S3. **Une équipe pour 40 couverts tient-elle dans 1 554 € ?**
2. **Capacité des lieux et des cuisines.** Des restaurants vacants peuvent-ils accueillir 40, 35 et 30 couverts pour un dîner à 6 services avec accords ? Une brigade de 2 ou 3 personnes peut-elle les envoyer ?
3. **Pilotes.** Le surcoût d'équipe des deux pilotes (1 155 €) est encore calculé avec l'onglet Staffing pour 24 et 20 couverts. Faut-il le recalculer pour les nouvelles jauges ?

### Produit
1. **Jauges.** L'offre et le pricing prévoient 24, 24 et 20 couverts, et une table de 10 pour la privatisation. Le modèle retient maintenant 40, 35, 30 et 20. **Le format « intime » de l'offre reste-t-il compatible avec ces jauges ?**
2. **Part de l'équipe dans le prix.** Votre répartition cible prévoyait 14 %, 12 % et 11 % du prix HT. Le modèle retient 15 %, 20 % et 20 %, et 15 % pour la privatisation. La répartition cible est-elle à mettre à jour ?
3. **Seuil de confirmation.** Avec ces hypothèses, le remplissage d'équilibre est de 66 %, 80 % et 92 %. Votre seuil de 70 % à J-14 ne couvre donc l'équilibre que pour le Premier soir.

### Marketing
1. **Demande.** Le modèle suppose que chaque soirée est **pleine** : 40, 35 ou 30 places vendues. Pour l'offre A, cela fait 315 places en année 1 (9 soirées), 840 en année 2 (24 soirées) et 1 260 en année 3 (36 soirées). **Les personas et la liste privée peuvent-ils remplir ces jauges au prix affiché ?** La rentabilité dépend désormais de ce chiffre.
2. **Photographe supprimé.** Le modèle ne prévoit plus de photographe par soirée (260 € auparavant). Les contenus des soirées sont-ils prévus autrement, par exemple dans le budget de communication, qui reste de 300 € par mois ?

---

## 5. Points à régulariser dans le fichier (I)

- **Sources à jour.** Les colonnes « Nature » et « Source » des lignes 7, 8, 26 et 33 décrivent encore les anciennes valeurs : capacités du Produit, scénario S3 des Opérations, photographe à 260 €. Il faut y indiquer « H, modification du responsable Finance du 28/10/2026 » et la raison de chaque choix.
- **Onglet Staffing déconnecté.** Il ne sert plus qu'au surcoût des pilotes. Ses effectifs restent ceux de 24 et 20 couverts.
- **Trésorerie et tableau de bord mis à jour le 28/10/2026.** La trésorerie finit à 18 462 € en octobre 2027, avec un point bas de −3 893 € en février 2027 et 1 451 € de crédit de TVA. Fichiers : `TRESORERIE/2026 1027 Modèle - Trésorerie et mois de survie.xlsx` et `PREVISIONS/2026 1028 Tableau de bord financier.html`. La fiche des données manquantes signale le changement d'hypothèses en tête de son § 1.
