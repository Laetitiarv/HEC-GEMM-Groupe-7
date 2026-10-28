# Points juridiques à revoir

**Date : 28/10/2026** · Fonction : `7 JURIDIQUE` · Production d'assistant IA, à la demande du responsable Juridique · Statut : liste de travail, rien n'est décidé

> **Aucune analyse ici ne vaut avis juridique.** Les règles de droit citées viennent des connaissances de l'assistant, pas d'une pièce de `sources/` : chacune est **à faire confirmer** (avocat, mairie, douanes, DDPP, assureur) avant d'entrer dans un contrat.

Cadre : [[REGISTRE DES DECISIONS]] D-01 (27/10/2026) et [[2026 1027 Descriptif du projet - Cadre de référence]] : une société d'événementiel qui réunit un restaurant ou un lieu avec cuisine, sur ses moments de vacance, et un chef d'exception ; cibles : communautés de foodies et organisation d'événements (corporate, éventuellement privés).

Documents relus : [[2026 1027 Schéma opérationnel d'un événement]] (`6 OPERATIONS/PRODUCTION/`, présent le 27/10 sur la branche `claude/github-access-confirmation-shlozm`, **pas encore sur `main`**) ; projets 2 et 3 (`PRODUCTIONS ASSISTANTS/`).

Légende (voir [[RULES]]) : **F** = fait constaté dans le dépôt · **I** = inférence · **P** = proposition. Hors champ : les questions RH (statut des chefs et des extras, recrutement), traitées à part.

---

## 0. Priorités avant tout pilote

| # | Point | Pourquoi bloquant | Statut |
|---|---|---|---|
| P1 | Montage de la licence de débit de boissons (§ 2) | Sans montage clair, pas de vente d'alcool possible | à revoir |
| P2 | Qui est l'exploitant alimentaire et porte la responsabilité sanitaire (§ 1.2) | Responsabilité en cas d'intoxication | en cours : orientation retenue le 28/10/2026, Pop Tables est l'exploitant alimentaire ; actions avant le pilote à mener ([[2026 1028 Responsabilité sanitaire - orientations retenues]]) |
| P3 | Assurance des biens confiés et RC organisateur (§ 1.6) | Le matériel du restaurateur est souvent exclu des RC standard | en cours : questionnaire et grille prêts le 28/10/2026, devis à demander ([[2026 1028 Questionnaire pour les courtiers d'assurance]]) |
| P4 | Dépôt GitHub public alors que `RULES.md` le dit privé (§ 4) | Toute pièce versée est lisible par tous | à revoir |

---

## 1. Schéma opérationnel d'un événement : points critiques

| # | Point du schéma (§ 4) | Ce qui reste à revoir (I / P) | Statut |
|---|---|---|---|
| 1.1 | Respect du lieu prêté | Clauses du contrat de mise à disposition : inventaire et état des lieux photographiés à l'entrée et à la sortie, stocks interdits sauf achat facturé, liste des équipements autorisés, caution ou franchise. Éviter la requalification en location-gérance ou en sous-location ; vérifier que le bail du restaurateur autorise ce prêt | à revoir |
| 1.2 | Hygiène et sécurité alimentaire | Si la start-up vend le repas, partir du principe qu'elle est l'exploitant alimentaire : plan de maîtrise sanitaire, traçabilité, au moins une personne formée à l'hygiène. Vérifier l'obligation de déclaration d'activité (DDPP) pour la start-up et pour le labo externe | en cours ([[2026 1028 Responsabilité sanitaire - orientations retenues]]) ; adresse de déclaration et plats témoins non confirmés par la DDPP |
| 1.3 | Chaîne du froid | Production à l'avance + transport = liaison froide : températures, délais, relevés conservés comme preuve | à revoir |
| 1.4 | Équipement du lieu | Liste d'équipements minimum en annexe du contrat avec le lieu | à revoir |
| 1.5 | Alcool | Voir § 2 : une licence est attachée à l'établissement et à son exploitant ; elle ne se prête pas pour une soirée | à revoir |
| 1.6 | Sécurité des personnes | Effectif maximal autorisé du lieu (établissement recevant du public) dans le contrat et dans la jauge vendue ; un lieu non autorisé à recevoir du public est à exclure pour un événement payant. Assurance : RC organisateur + extension **biens confiés** | à revoir |
| 1.7 | Déchets et voisinage | Tri obligatoire des biodéchets pour les professionnels ; clause d'horaires et de bruit répartissant la responsabilité entre la start-up et le restaurateur | à revoir |
| 1.8 | Plan de secours | Clause de remplacement du chef « par un chef de niveau équivalent » ou remboursement (risque de pratique commerciale trompeuse si le chef annoncé change) ; force majeure ; annulation par le lieu ; obligations du chef en cas de désistement | à revoir |

**Points absents du schéma**

| # | Point | Ce qui reste à revoir | Statut |
|---|---|---|---|
| 1.9 | Allergies des convives (étape 2 « Brief ») | Données de santé au sens du RGPD : consentement, transmission au seul chef, suppression après l'événement | à revoir |
| 1.10 | Information sur les allergènes | Les 14 allergènes réglementaires, par écrit, pour chaque plat servi | à revoir |
| 1.11 | Vente de places aux foodies (étape 1) | Conditions générales de vente ; droit de rétractation probablement exclu pour un loisir à date fixe (à vérifier) ; choisir entre **acompte** et **arrhes** | à revoir |
| 1.12 | Musique | Déclaration à la SACEM pour un événement payant | à revoir |
| 1.13 | Droit à l'image | Accord des convives (et du lieu pour un décor caractéristique) avant toute photo utilisée en communication | à revoir |
| 1.14 | Responsabilité face au client | La start-up, vendeur, répond face au client et se retourne contre le chef ou le fournisseur : à prévoir dans leurs contrats et dans l'assurance | à revoir |

**Corrections proposées au tableau « qui fait quoi » du schéma (§ 3)** — à proposer au pôle Opérations : ajouter, dans la ligne « Lieu », la vérification du bail, de la licence et de l'effectif autorisé ; dans la ligne « Incident », la responsabilité de la start-up face au client puis le recours ; une ligne « Alcool » (montage de licence tranché par le Juridique avant toute vente) ; une ligne « Données des convives » (politique de confidentialité, consentement pour les allergies).

---

## 2. Alcool : mariages et autres événements

**I** Principe : c'est la **vente** d'alcool à consommer sur place qui exige une licence. **Offrir** de l'alcool à des invités lors d'un événement privé n'en demande pas. La question est donc : qui vend l'alcool, et à qui ?

| Montage | Qui fournit | Licence pour la start-up ? | Appréciation (P) |
|---|---|---|---|
| 1. Le client apporte ses boissons, la start-up facture le service (« droit de bouchon ») | Le client | Probablement non | **Recommandé** pour mariages et événements privés ; écrire au devis que les boissons appartiennent au client |
| 2. Le restaurateur vend sous sa licence | Le restaurant hôte | Non ; le restaurateur devient vendeur et responsable de cette partie | Option dans les restaurants licenciés ; à prévoir au contrat de mise à disposition |
| 3. La start-up achète et revend dans son forfait | La start-up | Oui (modèle traiteur : licence à emporter et formation, à vérifier, notamment après 22 h) | À éviter pour le pilote |
| 4. Bar payant pour les invités | Les invités paient | Oui, licence de débit de boissons | **À exclure** : les buvettes temporaires visent surtout les associations |

**Par format d'événement**

| Format | Nature | Montages possibles |
|---|---|---|
| Mariage, anniversaire, communion, bar-mitsva | Événement privé, invités non payants | 1 (recommandé), 2 |
| Soirée d'entreprise | Événement privé, l'entreprise offre | 1, 2 |
| Communauté de foodies | **Vente au public** : chaque convive paie sa place, boissons comprises | 2, ou licence propre à la start-up |

**Risques à couvrir quel que soit le montage**

| # | Point | Ce qui reste à revoir | Statut |
|---|---|---|---|
| 2.1 | Mineurs (fréquents aux mariages, communions, bar-mitsva) | Interdiction de vendre ou d'offrir de l'alcool aux moins de 18 ans dans les débits de boissons et lieux publics ; un restaurant privatisé est-il un « lieu public » ? Par prudence : consigne de ne jamais servir de mineurs, au personnel et au contrat | à revoir |
| 2.2 | Ivresse | Ne pas servir une personne manifestement ivre ; responsabilité civile de l'organisateur en cas d'accident ; question à poser à l'assureur | à revoir |
| 2.3 | Horaires | Clause d'heure de fin avec le lieu (les mariages finissent tard) | à revoir |
| 2.4 | Devis client | Séparer repas, service et boissons, et dire qui est propriétaire des boissons | à revoir |
| 2.5 | Partenariats vins et champagne | Encadrement de la publicité pour l'alcool | à revoir |

---

## 3. Contrats types demandés par le cadre (D-01, § 4)

| # | Contrat | Points à revoir | Statut |
|---|---|---|---|
| 3.1 | Mise à disposition avec le lieu | Voir 1.1, 1.4, 1.6, 1.7, 2 ; confidentialité des créneaux de fermeture | à revoir |
| 3.2 | Prestation avec le chef | Rémunération fixe ou variable ; droit d'utiliser son nom, son image et son parcours ; accord de sa maison d'origine s'il est second ; obligations en cas de désistement (statut du chef : hors champ, RH) | à revoir |
| 3.3 | Contrat client entreprise | Devis forfaitaire, minimum de convives, acompte, annulation | à revoir |
| 3.4 | CGV particuliers (foodies, événements privés) | Voir 1.11 ; remboursement | à revoir |
| 3.5 | Données personnelles | Politique de confidentialité pour le fichier des communautés de foodies (RGPD) | à revoir |
| 3.6 | Nom et marque | Disponibilité du nom choisi par le Marketing | à revoir |

---

## 4. Société et dépôt

| # | Point | Ce qui reste à revoir | Statut |
|---|---|---|---|
| 4.1 | Gouvernance | **F** D-01 indique « mode de décision (vote ou non) non précisé par la source ». **P** Une règle de décision provisoire, puis les statuts de la SAS | à revoir |
| 4.2 | Noms cités dans le cadre | **F** Les lieux cités (Le Coste, Paris Society, Le Jeu de Paume, Les Chandelles) « ne valent ni accord, ni contact établi ». **P** Ne les utiliser dans aucun support public sans accord écrit | à revoir |
| 4.3 | Confidentialité du dépôt | **F** Le dépôt GitHub est public alors que `RULES.md` et `README.md` le disent privé. **P** Le passer en privé (responsable `1 DIRECTION`) avant d'y verser contrats ou échanges avec des tiers | à revoir |

Cette note recense des questions et ne décide rien (voir [[REGISTRE DES DECISIONS]]).
