# Gestionnaire d'Étudiants - Application Spring Boot

Ce projet est une application web Java basée sur Spring Boot pour gérer un registre d'étudiants. Il propose une API RESTful permettant des opérations CRUD (Créer, Lire, Mettre à jour, Supprimer) et des statistiques liées aux étudiants.

## Fonctionnalités

- **API RESTful complète** : Endpoints pour gérer les étudiants (créer, lire, mettre à jour, supprimer).
- **Persistance des données** : Gestion simplifiée des données avec Spring Data JPA et MySQL.
- **Gestion des erreurs** : Réponses HTTP appropriées pour les cas comme la suppression d'étudiants inexistants.
- **Statistiques** : Nombre total d'étudiants et répartition par année de naissance.
- **Tests unitaires** : Couverture de la logique métier et des contrôleurs avec JUnit et Mockito.

## Technologies Utilisées

- **Spring Boot** : Framework pour créer des applications autonomes prêtes à la production.
- **Spring Data JPA** : Gestion simplifiée des données relationnelles.
- **MySQL** : Base de données relationnelle pour stocker les données.
- **Lombok** : Réduction de la verbosité du code Java.
- **JUnit et Mockito** : Frameworks de test pour assurer la qualité.
- **Maven** : Gestionnaire de dépendances.

## Prérequis

- **Java Development Kit (JDK)** : Version 8 ou supérieure.
- **Maven** : Installé et configuré.
- **MySQL** : Serveur MySQL actif.
- **IDE Java** : IntelliJ IDEA, Eclipse ou autre.

##  Structure du Projet - Gestionnaire d'Étudiants
Voici une description des principaux packages et répertoires :

![image](https://github.com/user-attachments/assets/66dcace2-9135-416b-b909-a94f786a13fd)


###  Packages et Répertoires

### *com.example.student_managments.Controllers*
- Contient les contrôleurs Spring MVC qui gèrent les requêtes HTTP et les opérations liées à l'API RESTful.

### *com.example.student_managments.entities*
- Définit l'entité `Student`, qui représente un étudiant dans la base de données. Cette classe est utilisée pour la persistance des données.

### *com.example.student_managments.Repository*
- Contient l'interface `StudentRepository`, qui étend `JpaRepository` pour interagir avec la base de données de manière simple et efficace.

### *com.example.student_managments.service*
- Contient la classe `StudentService`, qui encapsule la logique métier et agit comme une couche intermédiaire entre les contrôleurs et le repository.

### *src/main/resources*
- Contient les fichiers de configuration, notamment :
  - **application.properties** : Fichier pour la configuration de l'application, comme les paramètres de connexion à la base de données.

### *src/test/java*
- Contient les tests unitaires pour valider le fonctionnement des différents composants du projet, en utilisant des frameworks comme JUnit et Mockito.


Cette structure permet une organisation claire et modulaire, facilitant le développement et la maintenance du projet.

## Installation et Exécution

### Cloner le dépôt

```bash
git clone <URL_DU_REPOSITORY>
