# Auto_ecole 🚓
Ce dépôt GitHub contient une conception détaillée pour une application d'auto-école. L'objectif principal de cette application est de fournir une plateforme conviviale et efficace pour les auto-écoles, les instructeurs et les étudiants.
## Fonctionnalités prévues ⚙️:

### Gestion des cours :
Permet aux auto-écoles de planifier, organiser et gérer les cours théoriques et pratiques.

### Suivi des progrès des élèves :
Permet aux instructeurs de suivre les progrès individuels des étudiants, y compris les heures de conduite effectuées, les scores aux tests théoriques, etc.

### Planification des leçons :
Permet aux instructeurs de planifier les leçons de conduite et de théorie de manière efficace, en tenant compte des disponibilités des étudiants et des instructeurs.

### Réservation en ligne :
Offre aux étudiants la possibilité de réserver leurs cours et leurs créneaux de conduite en ligne, offrant ainsi une flexibilité accrue.

### Gestion des ressources :
Permet la gestion des véhicules disponibles, des salles de classe, des manuels et des autres ressources nécessaires à l'enseignement.
### Suivi des paiements :
Permet aux auto-écoles de suivre les paiements des étudiants, de générer des factures et de gérer les finances de manière transparente.
### Communication :
Fournit un moyen de communication intégré entre les étudiants, les instructeurs et les administrateurs pour des échanges rapides et efficaces.


## Structure du dépôt :
### Documents de conception :
Comprend des documents détaillant l'architecture logicielle, les diagrammes de flux, les maquettes d'interface utilisateur, etc.


## Contributions :
Les contributions et les commentaires sont les bienvenus ! Si vous avez des idées pour améliorer cette conception ou si vous souhaitez contribuer au développement de l'application, n'hésitez pas à soumettre des pull requests ou à ouvrir des issues.



## Conception 🧑🏻‍🎤: 
![Internaute](https://github.com/jerbi2026/Auto_ecole/assets/116197682/41677b2c-a873-4b01-ba91-0c24833eb5f2)
![Eléve](https://github.com/jerbi2026/Auto_ecole/assets/116197682/0b0e8393-32c5-42c7-96ef-f4e95a0f3298)
![instructeur](https://github.com/jerbi2026/Auto_ecole/assets/116197682/88dde3b9-77b5-41e1-b6e1-ca023bcfb4f1)
![admin](https://github.com/jerbi2026/Auto_ecole/assets/116197682/5787fc00-2e1f-4800-ab2c-be937c75bcaa)


## Planification du premier sprint

### Préconditions :
- L’internaute a accès à une connexion internet
- Le site web de l’auto-école est disponible et accessible

### Postconditions :
- L’internaute a consulté avec succès les différentes offres proposés par l’auto-école
- Le site web de l’auto-école reste accessible pour l’internaute afin de poursuivre sa navigation ou d’effectuer d’autres actions


### Table de décision des tests de validation  :
#### Consulter les informations sur l’auto-école :

| Fonctionnalités                                                      | Test 1 | Test 2 | Test 3  | Test 4|
|----------------------------------------------------------------------|--------|--------|--------|--------|
| Accès à une connexion Internet                                       |   T    |   T    |   T    |   T    |
| Site web de l'auto-école disponible et accessible                    |   T    |   T    |   T    |    T   |
| Consultation des informations sur l'auto-école                       |   T    |   T    |   T    |    F   |
| Consultation des offres et des tarifs                                |   T    |   T    |   F    |   F    |
| Création d'un compte sur le site web de l'auto-école                 |   T    |   F    |   F    |   F    |
|Nombre de jeux de tests                                               | 2      | 2*n    | 1      |   1    |

#### Consulter les offres et les tarifs  :

| Fonctionnalités                                                      | Test 1 | Test 2 | Test 3  | Test 4|
|----------------------------------------------------------------------|--------|--------|--------|--------|
| Accès à une connexion Internet                                       |   T    |   T    |   T    |   T    |
| Site web de l'auto-école disponible et accessible                    |   T    |   T    |   T    |    T   |
| Consultation des informations sur l'auto-école                       |   T    |   T    |   T    |    F   |
| Consultation des offres et des tarifs                                |   T    |   T    |   F    |   F    |
| Création d'un compte sur le site web de l'auto-école                 |   T    |   F    |   F    |   F    |
|Nombre de jeux de tests                                               | 2      | 2*n    | 1      |   1    |

#### Créer un compte  :

| Fonctionnalités                                                      | Test 1 | Test 2 | Test 3  | Test 4|
|----------------------------------------------------------------------|--------|--------|--------|--------|
| Accès à une connexion Internet                                       |   T    |   T    |   T    |   T    |
| Site web de l'auto-école disponible et accessible                    |   T    |   T    |   T    |    T   |
| Consultation des informations sur l'auto-école                       |   T    |   T    |   T    |    F   |
| Consultation des offres et des tarifs                                |   T    |   T    |   F    |   F    |
| Création d'un compte sur le site web de l'auto-école                 |   T    |   F    |   F    |   F    |
|Nombre de jeux de tests                                               | 2      | 2*n    | 1      |   1    |



## Aspect Statique : 
### diagramme de classe : 
![diagramme_classe](https://github.com/jerbi2026/Auto_ecole/assets/116197682/c5239061-3925-47da-bf15-204cf9189d3a)

### Description textuelle du diagramme de classe
Le diagramme de classe représente les classes et les relations d'un système de gestion d'une auto-école. Les classes principales sont les suivantes :

#### Personne :
Représente une personne, qu'il s'agisse d'un élève, d'un instructeur ou d'un administrateur. Elle possède les attributs suivants :
nom : Le nom de la personne.
prenom : Le prénom de la personne.
email : L'adresse e-mail de la personne.
motDePasse : Le mot de passe de la personne.

#### Eleve :
Hérite de la classe Personne. Représente un élève inscrit à l'auto-école. Elle possède l'attribut supplémentaire suivant :
progression : La progression de l'élève dans sa formation.
Instructeur : Hérite de la classe Personne. Représente un instructeur de l'auto-école. Elle ne possède aucun attribut supplémentaire.

#### Admin :
Hérite de la classe Personne. Représente un administrateur de l'auto-école. Elle possède l'attribut supplémentaire suivant :
niveauAcces : Le niveau d'accès de l'administrateur.
Cours : Représente un cours de conduite. Elle possède les attributs suivants :
nom : Le nom du cours.
dateDebut : La date de début du cours.
dateFin : La date de fin du cours.
nombreHeures : Le nombre d'heures de cours.
listeElevesInscrits : La liste des élèves inscrits au cours.
listeEvaluations : La liste des évaluations du cours.

#### Evaluation :
Représente une évaluation d'un cours. Elle possède les attributs suivants :
dateEvaluation : La date de l'évaluation.
description : La description de l'évaluation.
listeElevesEvalues : La liste des élèves évalués.

#### Ressources :
Représente une ressource pédagogique. Elle possède les attributs suivants :

type : Le type de ressource (document, vidéo, etc.).
contenu : Le contenu de la ressource.
AutoEcole : Représente l'auto-école. Elle ne possède aucun attribut.

#### Les relations entre les classes sont les suivantes :

Association entre Personne et Cours : Une personne peut être inscrite à plusieurs cours.
Association entre Instructeur et Cours : Un instructeur peut donner plusieurs cours.
Association entre Eleve et Evaluation : Un élève peut être évalué plusieurs fois.
Association entre Cours et Ressources : Un cours peut utiliser plusieurs ressources pédagogiques.
Les classes GestionnaireEleve, GestionnaireInstructeur, GestionnaireEval et AutoEcole représentent des gestionnaires de classes. Elles fournissent des méthodes pour gérer les instances des classes correspondantes.

#### Exemple d'utilisation

Un administrateur peut créer un nouveau cours, y inscrire des élèves, affecter un instructeur au cours et créer des évaluations pour le cours. Un instructeur peut consulter les informations sur un cours et les élèves inscrits, et saisir les notes des élèves lors des évaluations. Un élève peut consulter les informations sur ses cours et ses évaluations.

## Aspect dynamique
### Diagramme de sequence creer compte
![creer_compte](https://github.com/jerbi2026/Auto_ecole/assets/116197682/3b0a2e17-3c6b-4622-ac85-752a1ad13f04)

### Diagramme de sequence s'authentifier
![s'authentifier](https://github.com/jerbi2026/Auto_ecole/assets/116197682/f6f1d5e7-205c-4064-bcff-b74136ae506b)

### Diagramme de sequence reserver un cours
![reserver_cour](https://github.com/jerbi2026/Auto_ecole/assets/116197682/47347dc4-847f-4a67-af2a-ff9bb50e97e9)






## Nombre de vues 👁️
<img align="left" src = "https://views-counter.vercel.app/badge?pageId=auto_ecole_agl%2FViews-Counter" alt ="Loading">


