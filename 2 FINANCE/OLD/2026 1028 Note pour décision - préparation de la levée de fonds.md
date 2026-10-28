# Note pour décision : préparation de la levée de fonds pour financer la trésorerie

**Date : 28/10/2026** · Fonction : `2 FINANCE` · Destinataire : Direction (@Laetitiarv) · Auteur : assistant IA Finance, à la demande de Vianney (responsable Finance) · Statut : **proposition soumise à décision**. Rien n'est décidé tant que la décision n'est pas inscrite au [[REGISTRE DES DECISIONS]].

Légende (voir [[RULES]]) : **F** = fait constaté dans un fichier du dépôt · **I** = inférence · **P** = proposition · **H** = hypothèse.

> **En bref.**
> - **P** Préparer dès maintenant une levée d'environ **265 000 €** sur 36 mois : un pont de 16 000 € pour l'année 1, puis un tour d'amorçage, dont environ 240 000 € en fonds propres.
> - **I** Le modèle actuel ne demande que 32 140 € à 3 ans. Mais ce chiffre ne résiste pas à une **hausse de 5 % des coûts des soirées** : le besoin de trésorerie passe alors à **96 161 €**.
> - **P** S'y ajoutent une contingence (111 334 €) et une trésorerie de sécurité (56 652 €).
> - **I** Ce dimensionnement suppose les hypothèses du modèle du 28/10 (jauges de 40, 35 et 30 couverts, salle pleine), que les pôles n'ont pas validées. Avec les jauges du Produit, le besoin dépasserait **740 000 €** et les soirées perdraient de l'argent. Lever des fonds ne règlerait pas ce problème.
> - **P** La taille finale de la levée est donc à fixer après la décision D-05 sur le couple prix × jauge.

Fichiers de calcul :
- `2 FINANCE/PREVISIONS/2026 1027 Modèle - Budget, plan financier, prix et marges.xlsx` (version du commit e4b5c06) ;
- `2 FINANCE/TRESORERIE/2026 1027 Modèle - Trésorerie et mois de survie.xlsx` ;
- `2 FINANCE/FINANCEMENT/2026 1027 Modèle - Financement et table de capitalisation.xlsx`.

La simulation à +5 % a été faite par script sur une copie du modèle. Le fichier du dépôt n'est pas modifié.

---

## 1. Point de départ (F, calculé par le modèle)

| | Montant | Source |
|---|---|---|
| Résultat d'exploitation, années 1, 2 et 3 | +15 913 €, +33 878 €, −63 931 € | Plan financier 3 ans, ligne 20 |
| Besoin de financement à 3 ans (flux cumulé, hors apport et hors TVA) | 32 140 € | Plan financier 3 ans, ligne 27 |
| Trésorerie, point bas de l'année 1 | −3 893 € en février 2027 | Modèle Trésorerie |
| Financements envisagés | Apport des associés 7 000 €, prêt d'honneur 20 000 €, subvention 5 000 €, levée 100 000 € sur 400 000 € de valorisation avant levée | Modèle Financement, statut « Envisagé » pour tous. Aucun fonds reçu, aucune pièce |

**I** L'année 3 est en perte parce que les frais généraux passent à 226 606 €, avec les premiers salaires. Avec 84 soirées prévues, la marge des soirées ne les couvre pas : le point mort est à 117 soirées par an.

## 2. Effet d'une hausse de 5 % des coûts de réalisation des soirées

**H** La hausse s'applique à tous les coûts de réalisation : lieu, cachet du chef, matières, boissons, équipe, ménage, assurance de la soirée, décor et autres coûts directs, y compris le surcoût des pilotes. Les frais de paiement et les commissions d'apporteur ne sont pas augmentés, parce qu'ils suivent le prix et non le coût. Les prix de vente ne changent pas.

### 2.1 Par soirée (F, calculé par le modèle)

| | Premier soir | Le Voyage | La Grande Nuit | Privatisation |
|---|---|---|---|---|
| Coûts directs actuels | 8 069 € | 11 461 € | 17 620 € | 8 529 € |
| Coûts directs à +5 % | 8 464 € | 11 991 € | 18 394 € | 8 901 € |
| Marge actuelle | 2 288 € | 1 664 € | 862 € | 2 186 € |
| **Marge à +5 %** | **1 893 €** | **1 134 €** | **88 €** | **1 813 €** |

**I** Le taux de marge du modèle est mince : 14 à 16 % du chiffre d'affaires. Une hausse de 5 % des coûts efface donc une grande partie de la marge. La Grande Nuit devient quasiment blanche.

### 2.2 Sur le plan à 3 ans et la trésorerie (F, calculé par le modèle)

| | Modèle actuel | Coûts des soirées à +5 % |
|---|---|---|
| Marge sur coûts directs, année 1 | 28 585 € | 20 821 € |
| Résultat, année 1 | +15 913 € | +8 149 € |
| Résultat, année 2 | +33 878 € | +11 340 € |
| Résultat, année 3 | −63 931 € | −102 213 € |
| Besoin de financement à 3 ans (plan) | 32 140 € | **100 725 €** |
| Point mort de l'année 3 | 117 soirées par an | 153 soirées par an |
| Trésorerie, point bas de l'année 1 | −3 893 € (février 2027) | **−5 278 € (février 2027)** |
| Trésorerie, fin octobre 2027 | 18 462 € | 9 712 € |
| Trésorerie, fin octobre 2028 | 47 341 € | 16 052 € |
| **Trésorerie, fin octobre 2029 (point bas sur 36 mois)** | −26 591 € | **−96 161 €** |

Méthode :
- **Année 1** : la trésorerie est calculée mois par mois, comme dans le modèle Trésorerie. Elle inclut l'apport de 7 000 €, la TVA et les investissements de novembre.
- **Années 2 et 3** : **H** les flux sont répartis également sur les 12 mois, avec les investissements en début d'année. La TVA n'est pas modélisée, faute de détail mensuel dans le plan.

**I** Une hausse de 1 % des coûts des soirées coûte environ 15 200 € de trésorerie sur 36 mois. Le coût des soirées est le premier risque financier du projet, avant les frais généraux.

**I** Fin octobre 2029, la société perd encore environ 8 500 € par mois. Elle n'a donc pas atteint son point mort à la fin du plan.

## 3. Contingence proposée (P)

Le projet présente un risque élevé sur les coûts, pour quatre raisons (**I**) :
- c'est une activité nouvelle, sans aucun coût constaté (aucune facture) ;
- chaque soirée est unique (lieu, chef et menu changent à chaque fois), donc on ne profite pas de la répétition ;
- la marge est mince (14 à 16 %) ;
- les coûts clés ne sont pas encore validés : l'indemnité du lieu, le cachet des chefs et le coût de l'équipe (voir la [[2026 1028 Note aux Opérations, au Produit et au Marketing - modifications du modèle de prévisions]]).

**I** Dans l'événementiel, la pratique courante est de prévoir une marge pour imprévus d'environ 10 % du budget de production. La contingence proposée suit ce niveau. Elle se compte **en plus** de la hausse de 5 % déjà simulée :

| Composante | Règle proposée | Montant sur 36 mois | Pourquoi |
|---|---|---|---|
| Contingence sur les coûts des soirées | 5 % des coûts directs à +5 % | 79 898 € | Avec la hausse simulée, les coûts des soirées sont couverts à environ 10 % au-dessus du modèle actuel |
| Contingence sur les frais généraux et les investissements | 10 % de 314 364 € (frais généraux 296 364 € + investissements 18 000 €) | 31 436 € | Ces frais sont engagés même si une soirée est annulée ; la montée des salaires n'est pas encore chiffrée par les pôles |
| Trésorerie de sécurité | 3 mois de frais généraux de l'année 3 (226 606 € ÷ 12 × 3) | 56 652 € | La société brûle encore de la trésorerie à la fin du plan ; une levée suivante prend plusieurs mois (I) |
| **Total contingence et sécurité** | | **167 986 €** | |

**Hors contingence (à décider à part).** La soirée de lancement recommandée par le Marketing coûterait 18 000 à 38 000 € HT. Elle n'est pas au budget (synthèse de la Direction du 28/10, incohérence n° 9). Si elle est retenue, il faut l'**ajouter** à la levée et non la prendre sur la contingence : elle en consommerait de 16 % à 34 %.

## 4. Dimensionnement de la levée (P)

| | Coûts à +5 %, hypothèses du modèle (recommandé) | Coûts à +5 %, jauges du Produit (scénario prudent) |
|---|---|---|
| Besoin de trésorerie au point bas sur 36 mois (apport de 7 000 € inclus) | 96 161 € | 581 958 € |
| Contingence sur les coûts des soirées | 79 898 € | 70 174 € |
| Contingence sur les frais généraux et les investissements | 31 436 € | 31 436 € |
| Trésorerie de sécurité | 56 652 € | 56 652 € |
| **Besoin total à financer** | **264 147 €, soit environ 265 000 €** | **740 220 €** |

**I** Dans le scénario prudent, toutes les soirées perdent de l'argent : de −212 € à −4 240 € par soirée à +5 %. Plus la société en organise, plus elle en perd. Le problème vient du modèle économique et non du financement : il faut d'abord revoir le couple prix × jauge (décision D-05 proposée par la Direction).

### Répartition proposée du besoin recommandé (P)

| Source | Montant | Nature | Remarque |
|---|---|---|---|
| Prêt d'honneur | 20 000 € | H | Montant déjà envisagé dans le modèle Financement. Le remboursement (333 € par mois sur 60 mois, simulé) n'est pas dans la trésorerie ci-dessus |
| Subvention ou concours | 5 000 € | H | Déjà envisagé |
| **Levée en fonds propres (business angels, dont l'associé gastronomique envisagé)** | **environ 240 000 €** | P | Au lieu des 100 000 € envisagés : ce montant ne couvrirait plus le besoin dès que les coûts augmentent |
| **Total** | **265 000 €** | | |

**I** Dilution : avec la valorisation de 400 000 € avant levée retenue comme hypothèse dans le modèle Financement, lever 240 000 € donnerait **37,5 %** du capital aux investisseurs, contre 20 % pour 100 000 €. Cette valorisation n'est fondée sur aucune évaluation. Les résultats des pilotes et des premiers mois sont le meilleur moyen de la relever.

## 5. Calendrier proposé (P)

1. **Pont de l'année 1 (novembre 2026 à février 2027), environ 16 000 €.** Ce montant couvre le point bas de −5 278 € et une contingence pour l'année 1 de 10 571 € (5 % des coûts des soirées et 10 % des frais généraux et investissements). Sources possibles : apports en compte courant des associés, prêt d'honneur ou subvention. **I** Ces financements prennent du temps à obtenir : le pont doit être en place avant le premier pilote de janvier 2027.
2. **Préparation de la levée (novembre 2026 à juin 2027).** Il s'agit de réunir les pièces qui transforment les hypothèses en faits :
   - les comptes des deux pilotes ;
   - des devis de lieux, de chefs et d'agences d'extras ;
   - 6 mois de chiffre d'affaires constaté ;
   - une table de capitalisation signée.
3. **Tour d'amorçage (second semestre 2027 à début 2028), environ 240 000 €.** **I** La trésorerie reste positive jusqu'en octobre 2028, puis l'année 3 la fait baisser dès novembre 2028 (premiers salaires, investissements). Les fonds doivent donc être reçus **avant novembre 2028**, et l'embauche ne doit pas démarrer sans eux.

## 6. Préalables avant de contacter un investisseur

| # | Préalable | Qui |
|---|---|---|
| 1 | Décision D-05 : couple prix × jauge de référence. C'est ce qui change le besoin de 265 000 € à plus de 740 000 € | Direction, Produit, Finance |
| 2 | Coûts des soirées confirmés par des devis : lieu, chef, équipe (questions de la note du 28/10 aux pôles) | Opérations, Ventes |
| 3 | Montée de la masse salariale des années 2 et 3, chiffrée par poste et par date | Direction, pôles |
| 4 | Société créée, statuts et pacte d'associés. La valorisation et les droits des investisseurs (préférence de liquidation, anti-dilution) sont à lire avant tout calcul de part | Juridique |
| 5 | Dépôt passé en privé : les chiffres financiers et la table de capitalisation ne doivent pas être publics (synthèse de la Direction, incohérence n° 16) | Direction |
| 6 | Licence et vente d'alcool réglées (synthèse de la Direction, incohérence n° 3) : un investisseur le demandera | Juridique |

## 7. Décisions demandées à la Direction

| # | Décision | Proposition de la Finance |
|---|---|---|
| 1 | Lancer la préparation d'une levée de fonds | Oui, avec la Finance et la Direction comme responsables |
| 2 | Scénario de dimensionnement | Coûts des soirées à +5 %, avec contingence et trésorerie de sécurité : **environ 265 000 € sur 36 mois** |
| 3 | Règle de contingence | Hausse de 5 % des coûts des soirées, plus 5 % des coûts des soirées, plus 10 % des frais généraux et investissements, plus 3 mois de frais généraux de l'année 3 |
| 4 | Montant visé en fonds propres | Environ 240 000 €, au lieu des 100 000 € envisagés, à confirmer après D-05 |
| 5 | Pont de l'année 1 | Environ 16 000 € avant janvier 2027 (comptes courants, prêt d'honneur, subvention) |
| 6 | Soirée de lancement | À inscrire au budget ou à abandonner : elle n'entre pas dans la contingence |

**Rappel (voir [[AGENT]] de la Finance).** Cette note propose un dimensionnement. Elle n'engage personne auprès d'une banque ou d'un investisseur.

**Statut des montants.** Un montant demandé n'est pas un montant obtenu. Tous les montants ci-dessus sont des hypothèses (H) ou des propositions (P) tirées d'un modèle sans aucun coût constaté.

## 8. Limites du calcul (I)

- **Années 2 et 3.** Les flux sont lissés sur l'année : un creux à l'intérieur d'une année n'est pas visible.
- **TVA.** Elle n'est pas modélisée pour les années 2 et 3.
- **Délais de paiement.** Le modèle n'en compte aucun. Or les privatisations B2B sont souvent payées à 30 jours ou plus, ce qui creuserait le besoin.
- **Prêt d'honneur.** Le remboursement n'est pas compté : 333 € par mois en simulation, soit environ 12 000 € sur 36 mois.
- **Hausse de 5 %.** Elle est appliquée sur toute la période. Une hausse progressive coûterait moins cher, une hausse plus forte plus cher (environ 15 200 € par point de hausse).
