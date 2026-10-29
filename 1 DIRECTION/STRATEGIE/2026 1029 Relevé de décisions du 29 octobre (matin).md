# Relevé de décisions — 29 octobre 2026 (matin)

Date : 29/10/2026, matin · Décidé par : Direction ([@Laetitiarv](https://github.com/Laetitiarv)) · Mise en forme : assistant IA Direction · Statut : **décisions de la Direction**, inscrites au [[REGISTRE DES DECISIONS]] sous les numéros D-25 et D-26 ; **un point reste à trancher** (§ 3).

Objet, selon la Direction : « Décision de ce matin pour cadrer les derniers éléments du projet ».

Légende (voir [[RULES]]) : **Décision** = mots de la Direction du 29/10 au matin · **F** = fait constaté dans un fichier du dépôt · **I** = inférence · **P** = proposition de l'assistant, non décidée.

---

## 1. Les décisions

| ID | Sujet | Décision (mots de la Direction) | Ce que cela veut dire concrètement | Remplace |
|---|---|---|---|---|
| D-25 | Ouverture des villes | « Changement d'ouvertures - Fin 2027 - lancement de 2 villes en France ; Fin de 2028 - lancement de 3 villes à l'étranger » | Année 2 : **2 nouvelles villes en France** (3 villes actives, toutes françaises). Année 3 : **3 villes à l'étranger** (6 villes actives). Le nombre total de villes ne change pas ; seule la répartition entre France et étranger change | La répartition des villes de D-15 (+1 France et +1 étranger en année 2 ; +1 France et +2 étranger en année 3). Le rythme d'une soirée à la place par mois et par ville (D-15) et les dates de D-21 (novembre 2027, novembre 2028) restent valables |
| D-26 | Financement initial | « Mise de fonds initial - 70K€ en love money » | La mise de départ est de **70 000 € apportés par les proches** des fondateurs (love money). La forme (capital, compte courant d'associés, BSA AIR) n'est pas précisée par la Direction | L'apport de 7 000 € retenu dans le budget de D-21. D-23 (levée de 135 000 € en tranche 1) **n'est pas remplacée** : elle est à recalculer (§ 2) |

## 2. Ce que montre le modèle Finance

F Le responsable Finance a déjà reporté D-25 et D-26 dans le modèle Prévisions (commit eae5c88, 29/10/2026, 10 h 25), onglet « Budget 36 mois » :
- lignes 97 à 101 : villes 2 et 3 en France, actives en novembre 2027 ; villes 4 à 6 à l'étranger, actives en novembre 2028 ;
- ligne 78 : apport des associés de 70 000 €, en novembre 2026.

F Recalcul du modèle (LibreOffice, 29/10/2026) :

| | Avant (D-21, apport 7 000 €) | Après (D-25, D-26) |
|---|---|---|
| Villes actives, années 1 / 2 / 3 | 1 / 3 / 6 | 1 / 3 / 6 |
| Résultat d'exploitation, années 1 / 2 / 3 | −36 232 / 387 758 / 378 857 € | inchangé |
| Point bas de la trésorerie sur 36 mois, avant levée | −52 929 € (mars 2027) | **+10 071 € (mars 2027)** |
| Trésorerie en fin d'année 1, avant levée | −8 551 € | 54 449 € |

I Le changement de villes n'a pas d'effet sur le résultat, car le modèle donne le même coût d'ouverture (15 000 €) et les mêmes prix aux villes françaises et étrangères.

I Avec 70 000 €, la trésorerie ne passe plus sous zéro dans le budget de base. Le trou d'environ 17 800 € en novembre 2026 (site et matériel payés au départ) est couvert.

I La note de levée (`2 FINANCE/FINANCEMENT/2026 1028 Note pour décision - levée de fonds Pop Tables.md`, § 5) chiffrait un besoin total de 133 174 € avec un apport de 7 000 €. Avec 63 000 € de plus, le besoin restant serait de l'ordre de 70 000 €, contingence et trésorerie de sécurité comprises. **À recalculer par la Finance** ; le montant de la tranche 1 reste à décider par la Direction.

## 3. Point à trancher : privatisation pour moins de 30 convives

Mots de la Direction : « Privatisation pour moins de 30 convives : Fixer un minimum facturé de 30 couverts (15 000 € TTC), comme le propose le Marketing, ou réintroduire un forfait ».

La formulation laisse deux options ouvertes. **Aucune n'est inscrite au registre** tant que la Direction n'a pas choisi.

| Option | Ce qu'elle donne | Effet sur le plan |
|---|---|---|
| A. Minimum facturé de 30 couverts (proposition du Marketing, [[2026 1029 Note du Marketing à la Finance et au Produit]], § 1) | Le groupe paie 15 000 € TTC (13 393 € HT) quelle que soit sa taille ; au-delà de 30, 500 € TTC par convive (D-22) | I Garantit le chiffre d'affaires par privatisation que suppose le budget (13 393 € HT). F Le modèle prévoit déjà une ligne « Minimum facturé » (Prix et marges, ligne 15), aujourd'hui à 0 |
| B. Retour d'un forfait | Un forfait fixe (lieu, chef, équipe, conception) plus un prix par convive, comme avant D-22 (6 000 € + 300 € TTC par convive) | I À 30 convives, l'ancien forfait donnait 15 000 € TTC, comme l'option A. En dessous, il rapporte moins (9 000 € TTC à 10 convives) ; le forfait et le prix par convive seraient à recalibrer par le Produit et la Finance |

Décision à prendre par : la Direction.

## 4. Ce que chaque pôle met à jour dans son dossier

**Finance (@Vianney-wind)** — Corriger le libellé de la ligne 36 du « Plan financier 3 ans » (« apport de 7 000 € » → 70 000 €) et les colonnes « Source » des lignes 78 et 97 à 101 (D-25, D-26). Recalculer la levée (tranche 1, contingence, trésorerie de sécurité) et la table de capitalisation avec la love money. Mettre à jour la note de levée.

**Marketing (@serge2309)** — Revoir la proposition des villes : 2 villes françaises pour l'année 2, 3 villes étrangères pour l'année 3 ([[2026 1028 Lieux et villes - Villes des années 2 et 3]] proposait Lyon et Londres en année 2). Revoir le rythme saisonnier si la Côte d'Azur passe en année 2.

**Ventes (@xavierjuraflo-ship-it)** — Vérifier que 40 privatisations par an sont tenables dans les 2 villes françaises de l'année 2.

**Juridique (@alexanderzhelev-dev)** — Forme de la love money (capital, compte courant, BSA AIR) et clauses avec les proches. I La structure à l'étranger n'est plus nécessaire avant fin 2028.

**Produit (@Fredlay26)** — Selon le choix du § 3 : inscrire le minimum facturé ou recalibrer le forfait dans la grille de prix.

**Direction** — Trancher le § 3 ; décider du montant de la tranche 1 après le recalcul de la Finance. Le Business Model Canvas V6 (D-24) mentionne encore la tranche 1 de 135 000 € et le trou de trésorerie de novembre 2026 (onglet « Hypothèses et owners », B15) : une V7 serait à prévoir.

Décisions prises par : la Direction (@Laetitiarv), le 29/10/2026 au matin. Mode de décision (vote ou non) : non précisé.
