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

### Table de décision des tests de validation  :

#### créer un compte  :
##### Préconditions :
- L'utilisateur a accès à une connexion internet.
- Le système d'inscription est disponible et accessible.
- L'utilisateur fournit des informations valides pour créer un compte (nom, adresse e-mail, mot de passe).

##### Postconditions :
- Le compte utilisateur est créé avec succès.
- L'utilisateur reçoit un message de confirmation de création de compte.
- L'utilisateur peut accéder aux fonctionnalités restreintes du système avec les informations d'identification fournies.

##### table de décision

| Préconditions                                                                                            | Test 1 | Test 2 | Test 3 | Test 4 |              
|----------------------------------------------------------------------------------------------------------|--------|--------|--------|--------|
| L'utilisateur a accès à une connexion internet.                                                          |   T    |   T    |   T    |   F    |
| Le système d'inscription est disponible et accessible.                                                   |   T    |   T    |   F    |   F    |  
| L'utilisateur fournit des informations valides pour créer un compte (nom, adresse e-mail, mot de passe). |   T    |   F    |   F    |   F    |

| Postconditions                                                                                                         | Test 1 | Test 2 | Test 3 | Test 4 |              
|------------------------------------------------------------------------------------------------------------------------|--------|--------|--------|--------|
| Le compte utilisateur est créé avec succès.                                                                            |   T    |   F    |   F    |   F    |
| L'utilisateur reçoit un message de confirmation de création de compte.                                                 |   T    |   F    |   F    |   F    |  
| L'utilisateur peut accéder aux fonctionnalités restreintes du système avec les informations d'identification fournies. |   T    |   F    |   F    |   F    |  

##### diagramme de test 
![creer_compte](https://github.com/jerbi2026/Auto_ecole/assets/116197682/b81dda59-1d98-4037-b085-9c33a0b5dc4b)








#### S'authentifier  :
##### Préconditions :
- L'utilisateur a accès à une connexion internet.
- L'utilisateur a un compte enregistré dans le système.
- L'utilisateur fournit des informations d'identification valides (adresse e-mail et mot de passe).

##### Postconditions :
- L'utilisateur est authentifié avec succès.
- L'utilisateur reçoit un message de bienvenue ou est redirigé vers une page d'accueil après l'authentification.


##### table de décision

| Préconditions                                                                                     | Test 1 | Test 2 | Test 3 | Test 4 |              
|---------------------------------------------------------------------------------------------------|--------|--------|--------|--------|
| L'utilisateur a accès à une connexion internet.                                                   |   T    |   T    |   T    |   F    |
| L'utilisateur a un compte enregistré dans le système.                                             |   T    |   T    |   F    |   F    |  
| L'utilisateur fournit des informations d'identification valides (adresse e-mail et mot de passe). |   T    |   F    |   F    |   F    |

| Postconditions                                                                                                  | Test 1 | Test 2 | Test 3 | Test 4 |              
|-----------------------------------------------------------------------------------------------------------------|--------|--------|--------|--------|
| L'utilisateur est authentifié avec succès.                                                                      |   T    |   T    |   T    |   F    |
| L'utilisateur reçoit un message de bienvenue ou est redirigé vers une page d'accueil après l'authentification.  |   T    |   T    |   F    |   F    |  


##### diagramme de test 
![authentifier](https://github.com/jerbi2026/Auto_ecole/assets/116197682/04ea3321-c0a2-44f9-b577-d6ece9bac0c6)




#### Réserver un cours:
##### Préconditions :
- Le client est inscrit auprès de l'auto-école.
- Le cours est disponible à la réservation.
- Il y a des places disponibles dans le cours.

##### Postconditions :
- La réservation du cours est effectuée avec succès.
- Une confirmation de réservation est envoyée au client.
- Le nombre de places disponibles dans le cours est mis à jour.

##### table de décision

| Préconditions                                                        | Test 1 | Test 2 | Test 3 | Test 4 |              
|----------------------------------------------------------------------|--------|--------|--------|--------|
| Le client est inscrit                                                |   T    |   T    |   T    |   F    |
| Le cours est disponible à la réservation.                            |   T    |   T    |   F    |   F    |  
| Il y a des places disponibles dans le cours.                         |   T    |   F    |   F    |   F    |

| Postconditions                                                       | Test 1 | Test 2 | Test 3 | Test 4 |                          
|----------------------------------------------------------------------|--------|--------|--------|--------|
| Réservation effectuée                                                |   T    |   F    |   F    |   F    |
| Confirmation envoyée au client.                                      |   T    |   F    |   F    |   F    |
| Mise à jour des places disponibles.                                  |   T    |   F    |   F    |   F    | 

##### diagramme de test 
![reserver_cours](https://github.com/jerbi2026/Auto_ecole/assets/116197682/a9863611-1c84-4765-9716-1ff9f3ea2cc8)





## Aspect Statique : 
### diagramme de classe Raffiné (Conception Detaillé): 
![diagramme_classe_raffine](https://github.com/jerbi2026/Auto_ecole/assets/116197682/51bd6c7d-810e-407e-8427-25db0f1ea843)


### Description textuelle du diagramme de classe
#### Classes:

##### Reservation:
id: Identifiant unique de la réservation
dateReservation: Date de la réservation
cours: Cours réservé
eleve: Élève qui a effectué la réservation
message: Message optionnel associé à la réservation
annulerReservation(): Annule la réservation
envoyerMessage(): Envoie un message à l'élève
consulterInformations(): Consulte les informations de la réservation
reinitialiserMotDePasse(): Réinitialise le mot de passe de l'élève (si applicable)
modifierInformations(): Modifie les informations de la réservation

##### Cours:
id: Identifiant unique du cours
nomCours: Nom du cours
dateDebut: Date de début du cours
dateFin: Date de fin du cours
oidInstructeur: Identifiant de l'instructeur qui dispense le cours
listeEleves: Liste des élèves inscrits au cours
listeEvaluations: Liste des évaluations du cours
horraires: Horaires du cours
annulerCours(): Annule le cours
modifierCours(): Modifie les informations du cours

##### Eleve:
oid: Identifiant unique de l'élève
nom: Nom de l'élève
prenom: Prénom de l'élève
email: Adresse email de l'élève
connexionDemande: Demande de connexion (si applicable)
cours: Liste des cours auxquels l'élève est inscrit
inscriptions: Liste des inscriptions de l'élève
consulterInformations(): Consulte les informations de l'élève
modifierInformations(): Modifie les informations de l'élève

##### Instructeur:
id: Identifiant unique de l'instructeur
nom: Nom de l'instructeur
prenom: Prénom de l'instructeur
oidEleve: Identifiant de l'élève responsable de l'instructeur (si applicable)
progression: Progression de l'instructeur
listeCours: Liste des cours dispensés par l'instructeur
consulterInformations(): Consulte les informations de l'instructeur
modifierInformations(): Modifie les informations de l'instructeur
sinscrireCours(cours: Cours): S'inscrit à un cours
suivreCours(cours: Cours): Suit un cours
creerHorraire(jour: String, heureDebut: String, heureFin: String): Crée un horaire
modifierHorraire(id: Int, jour: String, heureDebut: String, heureFin: String): Modifie un horaire
supprimerHorraire(id: Int): Supprime un horaire

##### Admin:
idManager: Identifiant unique du manager
consulterEleves(): Consulte la liste des élèves
creerEleve(eleve: Eleve): Crée un nouvel élève
modifierEleve(eleve: Eleve): Modifie les informations d'un élève
supprimerEleve(eleve: Eleve): Supprime un élève
consulterInstructeurs(): Consulte la liste des instructeurs
creerInstructeur(instructeur: Instructeur): Crée un nouvel instructeur
modifierInstructeur(instructeur: Instructeur): Modifie les informations d'un instructeur
supprimerInstructeur(instructeur: Instructeur): Supprime un instructeur
consulterCours(): Consulte la liste des cours
gererCours(): Gère les cours
evaluerEleve(eleve: Eleve, note: int): Évalue un élève

#### Relations:
- Une réservation est associée à un cours, un élève et un instructeur.
- Un cours est dispensé par un instructeur et peut avoir plusieurs élèves inscrits.
- Un élève peut être inscrit à plusieurs cours et peut avoir un instructeur responsable.
- Un instructeur peut dispenser plusieurs cours et peut avoir un élève responsable.
- Un administrateur peut gérer les élèves, les instructeurs et les cours.


#### Exemple d'utilisation

Un administrateur peut créer un nouveau cours, y inscrire des élèves, affecter un instructeur au cours et créer des évaluations pour le cours. Un instructeur peut consulter les informations sur un cours et les élèves inscrits, et saisir les notes des élèves lors des évaluations. Un élève peut consulter les informations sur ses cours et ses évaluations.

## Aspect dynamique
### Diagramme de sequence creer compte
![creer_compte](https://github.com/jerbi2026/Auto_ecole/assets/116197682/6b8932ce-3fc9-4200-ae0c-d9e5a2f35795)

### Diagramme de sequence s'authentifier
![s'authentifier](https://github.com/jerbi2026/Auto_ecole/assets/116197682/ba9dfc1f-02f9-4762-ba57-f3a0a6d8aa13)

### Diagramme de sequence reserver un cours
![reserver_cour](https://github.com/jerbi2026/Auto_ecole/assets/116197682/162ab706-aba2-4ee9-99f2-36e40f3b82d1)


## Conception Detaillé : 
### un diagramme de machine à états de la classe Evaluation:
![diagramme_evaluation](https://github.com/jerbi2026/Auto_ecole/assets/116197682/800d1c4f-5089-4d8b-9417-0f26344b7853)

* EnAttente : L’état initial lorsque l’évaluation est créée. Le système attend que l’évaluation soit effectuée.
   - Transition vers EnCours : Le paiement est accepté.
   - Transition vers Annulee : L’utilisateur demande l’annulation de l’évaluation.
* EnCours : L’évaluation est en cours. Des actions telles que la saisie des notes et la rédaction de la description peuvent être effectuées.
   - Transition vers EnAttente : L’utilisateur annule l’évaluation.
   - Transition vers Terminee : L’évaluation est terminée.
* Terminee : L’évaluation est terminée. Une nouvelle évaluation peut être initiée.
* Annulee : L’évaluation a été annulée. Une nouvelle évaluation peut être initiée.

### un diagramme de machine à états de la classe Reservation:
![diagramme_reservations](https://github.com/jerbi2026/Auto_ecole/assets/116197682/2ceeb9aa-0435-4bf0-aab9-4e36ff3b8788)

* EnAttente : L’état initial lorsque la réservation est créée. Le système attend le paiement.
  - Transition vers EnCours : Le paiement est accepté.
  - Transition vers Annulee : L’utilisateur demande l’annulation de la réservation.
* EnCours : La réservation est active, le paiement a été accepté. Des actions telles que la modification ou l’annulation peuvent être effectuées.
  - Transition vers EnAttente : L’utilisateur annule la réservation.
  - Transition vers Terminee : Le séjour est terminé.
* Terminee : Le séjour est terminé, la réservation est close. Une nouvelle réservation peut être initiée.
* Annulee : La réservation a été annulée. Une nouvelle réservation peut être initiée.









## Nombre de vues 👁️
<img align="left" src = "https://views-counter.vercel.app/badge?pageId=auto_ecole_agl%2FViews-Counter" alt ="Loading">


