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
![diagramme_classe_raffine](https://github.com/jerbi2026/Auto_ecole/assets/116197682/621a47d7-f532-46d6-a10e-25680054c6fc)


### Description textuelle du diagramme de classe
#### Classes:
##### Auto ecole:
La classe AutoEcole représente l'entité principale qui gère toutes les opérations liées à une auto-école. Elle agit comme une interface centrale pour interagir avec les différentes entités de l'auto-école, telles que les élèves, les instructeurs, les réservations, les demandes de connexion, et les contacts.

###### consulterInformations(): String
Cette méthode permet de consulter les informations générales de l'auto-école, telles que son nom, son adresse et ses coordonnées.
###### gererCours(): void
Cette méthode permet de gérer les cours proposés par l'auto-école, y compris la création, la modification et l'annulation des cours.
###### consulterEleves(): List<Eleve>
Cette méthode renvoie la liste de tous les élèves inscrits à l'auto-école.
###### creerEleve(eleve: Eleve): void
Cette méthode permet de créer un nouveau profil d'élève dans le système de l'auto-école.
###### modifierEleve(eleve: Eleve): void
Cette méthode permet de modifier les informations d'un élève existant dans le système de l'auto-école.
###### supprimerEleve(eleve: Eleve): void
Cette méthode permet de supprimer le profil d'un élève du système de l'auto-école.
###### consulterInstructeur(): List<Instructeur>
Cette méthode renvoie la liste de tous les instructeurs travaillant pour l'auto-école.
###### creerInstructeur(instructeur: Instructeur): void
Cette méthode permet de créer un nouveau profil d'instructeur dans le système de l'auto-école.
###### modifierInstructeur(instructeur: Instructeur): void
Cette méthode permet de modifier les informations d'un instructeur existant dans le système de l'auto-école.
###### supprimerInstructeur(instructeur: Instructeur): void
Cette méthode permet de supprimer le profil d'un instructeur du système de l'auto-école.
###### consulterReservations(): List<Reservation>
Cette méthode renvoie la liste de toutes les réservations de cours effectuées par les élèves.
###### annulerReservation(reservation: Reservation): void
Cette méthode permet d'annuler une réservation de cours effectuée par un élève.
###### consulterConnexionsDemandes(): List<ConnexionDemande>
Cette méthode renvoie la liste de toutes les demandes de connexion au système de l'auto-école.
###### reinitialiserMotDePasse(demande: ConnexionDemande): boolean
Cette méthode permet de réinitialiser le mot de passe d'un utilisateur en fonction d'une demande de réinitialisation.
###### consulterContacts(): List<Contact>
Cette méthode renvoie la liste de tous les contacts reçus par l'auto-école via son site web ou d'autres canaux de communication.
###### envoyerMessage(contact: Contact): void
Cette méthode permet d'envoyer une réponse à un contact spécifié, par exemple pour répondre à une demande d'information ou de support.
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
![creer_compte](https://github.com/jerbi2026/Auto_ecole/assets/116197682/36dacc11-cee8-47ff-8a2c-2d13f36d45d6)

### Diagramme de sequence s'authentifier
![s'authentifier](https://github.com/jerbi2026/Auto_ecole/assets/116197682/eca20094-9a36-4910-aed0-6a7dd268b541)

### Diagramme de sequence reserver un cours
![reserver_cour](https://github.com/jerbi2026/Auto_ecole/assets/116197682/7cd2c89c-3bed-4230-b253-8b734430924e)


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


## Raffinement de digramme de classe : 
![diagramme_de_classe](https://github.com/jerbi2026/Auto_ecole/assets/116197682/14ec76ca-41de-4335-8ad8-9f86fc480d65)

- Modification de visibilité
- Ajout de commentaires
- Ajout des invariants
- Modification des associations

### Les attributs et opérations de chaque classe :
##### Personne :
Attributs: nom (string), prenom (string), email (string), mop (string)
Operations: s’authentifier (nom: string, mop: string), consulterinformations (), modifierinformations ()
##### Elève :
Attributs: id_eleve (int), progression(string), listeCours (List<Cours>)
Operations : consulterinformations (), modifierinformations (), sinscrireCours (cours : Cours), suivreCours (cours : Cours)

##### Instructeur :
Attributs : id_instructeur (int)
Operations : consulterinformations (), modifierinformations (), consulterCours (List<Cours>), creerCours (cours : Cours), modifierCours (Cours : cours), supprimerCours (Cours : cours)
##### Admin :
Attributs : id_manager (int)
Operations : consulterEleves (), creerEleve (eleve : Eleve), modifierEleve (eleve : Eleve), supprimerEleve (eleve : Eleve), consulerinstructeur (List<Instructeur>), creeinstructeur (Instructeur : instructeur), modifierinstructeur (Instructeur : instructeur), supprimerinstructeur (Instructeur : instructeur)

##### Cours :
Attributs : id (int), dateDebut (date), datefin (date) , nomCours (string), id_instructeur (int), listeEleves (List<Eleve>), listeEvaluations (List<Evaluation>), horraires (Horraire)
Operations : annulerCours (), modifierCours ()
##### Evaluation :
Attributs : idEval (int), dateEval (date), description (string), note (int), id_eleve (int)
Operations: ajouterNote (eleve: Eleve, note: int), consulterNotes (List<int>)
##### Horaire :
Attributs: id (int), jour (string), heureDebut (string), heurefin (string)
Operations: creerHorraire (jour: string, heureDebut: string, heureFin: string), lireHorraire (id: int), mettreAjourHorraire (id: int, jour: string, heureDebut: string, heureFin: string), supprimerHorraire (id: int)
##### Réservation :
Attributs : id (int), eleve (Eleve), cours (Cours), dateReservation (date)
Operations : ajouterReservation (Reservation : Reservation), supprimerReservation (Reservation : Reservation), modifierReservation (Reservation : Reservation), annulerReservation ()
##### Contact :
Attributs: nom (string), prenom (string), email (string), message (string)
Operations : envoyerMessage (Contact : Contact), ConsulterMessage (List<Contact>)


##### ConnexionDemande :
Attributs: email (string), motDePasse (string)
Operations: authentifier (email: string, motDePasse: string), reinitialiserMotDePasse ()

### Traduction des relations:
- Admin->Reservation (Association) : admin gère les réservations
- Admin->Contact (Association) : contact est gérer par admin
- Admin->Personne (Héritage) : admin hérite de la classe personne
- ConnexionDemande->Personne (Association) : la classe Personne possède ConnexionDemande
- Instructeur->Personne (Héritage) : Instructeur hérite de la classe Personne
- Evaluation->Eleve (Association) : Eleve est évalué par Evaluation
- Eleve->Cours (Association) : Eleve suit un Cours
- Evaluation->Cours (Association) : Evaluation appartient à un Cours
- Instructeur->Cours (Association) : Instructeur enseigne Cours
- Horraire->Cours (Association) : Horraire appartient à Cours
- Admin->Cours (Association) : Admin gère Cours
- Admin->Instructeur (Association) : Admin consulte Instructeur
- Admin->Eleve (Association): Admin consulte Eleve

### Définition de la visibilité, du type et des valeurs par défaut des attributs : 
- Les attributs de la classe Personne sont « protected »
- Les attributs des classes restantes sont « private »
- Les méthodes de toutes les classes sont « public »
- Les types des attributs sont : int, string, date, List<>
- Les valeurs par défaut ne sont pas spécifiées dans le diagramme, mais peuvent être définies selon les besoins du système
##### Définition d’un invariant pour la classe Eleve :
Un invariant pour la classe Eleve pourrait être que la progression d’un élève ne doit pas dépasser 100 
En logique propositionnelle, nous pouvons le formuler comme suit :
* Si P représente la progression de l’élève, alors 0 <= P <= 100 


## Invariants
### Table de décision des tests :
#### Table de décision de tests pour l’opération s’authentifier (nom : string, mop : string) :
| TC  | nom   | mop      | Résultat attendu        |
| --- | ----- | -------- | ----------------------- |
| TC1 | Ahmed | Ahmed8795| Connexion réussie       |
| TC2 |       | Aziz789  | Connexion échouée (nom d'utilisateur vide) |
| TC3 | Rami  |          | Connexion échouée (mot de passe vide) |

* TC1 : authentification réussie avec un nom d’utilisateur valide et un mot de passe valide
* TC2 : Echec de l’authentification en raison d’un mot d’utilisateur vide, même avec un mot de passe valide
* TC3 : Echec de l’authentification en raison d’un mot de passe vide, même avec un nom d’utilisateur valide 

#### Table de décision de tests pour l’opération ajouter_reservation () :
| TC  | Condition1 : Date de réservation valide | Condition2 : Place disponible | Condition : Client valide | Résultat attendu                                 |
| --- | --------------------------------------- | ----------------------------- | -------------------------- | ------------------------------------------------ |
| TC1 | Oui                                     | Oui                           | Oui                        | Réservation ajoutée avec succès                  |
| TC2 | Oui                                     | Oui                           | Non                        | Echec de l’ajout de réservation (client invalide) |
| TC3 | Oui                                     | Non                           | Oui                        | Echec de l’ajout de réservation (place non disponible) |
| TC4 | Non                                     | Oui                           | Oui                        | Echec de l’ajout de réservation (date de réservation invalide) |
| TC5 | Non                                     | Non                           | Oui                        | Echec de l’ajout de réservation (date de réservation invalide et place non disponible) |
| TC6 | Oui                                     | Non                           | Non                        | Echec de l’ajout de réservation (place non disponible et client invalide) |
| TC7 | Non                                     | Oui                           | Non                        | Echec de l’ajout de réservation (date de réservation invalide et client invalide) |
| TC8 | Non                                     | Non                           | Non                        | Echec de l’ajout de réservation                   |

* TC1 : La date de réservation est valide, une place est disponible, et le client est valide. Dans ce cas, la réservation devrait être ajoutée avec succès.
* TC2 : La date de réservation est valide et une place est disponible, mais le client n'est pas valide. L'ajout de réservation devrait échouer en raison d'un client invalide.
* TC3 : La date de réservation est valide, mais aucune place n'est disponible. L'ajout de réservation devrait échouer en raison de l'indisponibilité de places.
* TC4 : La date de réservation n'est pas valide, mais une place est disponible et le client est valide. L'ajout de réservation devrait échouer en raison d'une date de réservation invalide.
* TC5 : La date de réservation n'est pas valide et aucune place n'est disponible, mais le client est valide. L'ajout de réservation devrait échouer en raison d'une date de réservation invalide et de l'indisponibilité de places.
* TC6 : La date de réservation est valide, mais aucune place n'est disponible et le client n'est pas valide. L'ajout de réservation devrait échouer en raison de l'indisponibilité de places et d'un client invalide.
* TC7 : La date de réservation n'est pas valide, une place est disponible, mais le client n'est pas valide. L'ajout de réservation devrait échouer en raison d'une date de réservation invalide et d'un client invalide.
* TC8 : La date de réservation n'est pas valide, aucune place n'est disponible, et le client n'est pas valide. L'ajout de réservation devrait échouer en raison d'une date de réservation invalide, de l'indisponibilité de places et d'un client invalide.

#### Table de décision de tests pour l’opération supprimer Eleve () : 
| TC  | Condition1 : Eleve existant | Condition2 : Eleve sélectionné pour la suppression | Résultat attendu                                |
| --- | ---------------------------- | ----------------------------------------------- | ---------------------------------------------- |
| TC1 | OUI                          | OUI                                           | Eleve supprimé avec succès                    |
| TC2 | Non                          | N/A                                           | Echec de suppression de l’élève (élève inexistant) |
| TC3 | Oui                          | Non                                           | Echec de suppression de l’élève (élève non sélectionné pour la suppression) |
| TC4 | Non                          | N/A                                           | Echec de suppression de l’élève (élève inexistant) |


* TC1 : L'élève existe dans le système et a été sélectionné pour suppression. Dans ce cas, l'élève devrait être supprimé avec succès.
* TC2 : L'élève n'existe pas dans le système. Par conséquent, la suppression de l'élève échoue car il n'y a aucun élève à supprimer.
* TC3 : L'élève existe dans le système, mais il n'a pas été sélectionné pour suppression. Par conséquent, la suppression de l'élève échoue car l'administrateur n'a pas spécifiquement sélectionné cet élève pour suppression.
* TC4 : Comme dans le cas du TC2, l'élève n'existe pas dans le système. La suppression de l'élève échoue pour la même raison que dans le TC2, à savoir qu'il n'y a aucun élève à supprimer.












## Nombre de vues 👁️
<img align="left" src = "https://views-counter.vercel.app/badge?pageId=auto_ecole_agl%2FViews-Counter" alt ="Loading">


