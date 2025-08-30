# Application Gestion Bibliothèque

## Installation de l'application
1. Cloner le projet sur votre machine locale  
   ```bash
   git clone <URL_DU_PROJET>
Ouvrir le projet dans votre IDE préféré (IntelliJ IDEA, Eclipse, NetBeans, etc.)

## Installer les dépendances Maven :

bash
Copier le code
mvn clean install
Lancer la base de données via Docker :

bash
Copier le code
docker-compose up
Exécuter le script SQL pour créer la base de données :

bash
Copier le code
./database.sql
Lancer l'application Spring Boot :

bash
Copier le code
mvn spring-boot:run
L'application est accessible via la console.

## Prérequis
Java 17 ou supérieur

Maven 3.6.3

Docker

Git 2.25.1

IDE (IntelliJ IDEA, Eclipse, NetBeans, etc.)

## Diagramme de classes


## Contexte
La bibliothèque de l’université virtuelle rencontre des défis liés à une gestion manuelle des livres :

Gestion inefficace : tâches manuelles chronophages, erreurs fréquentes et suivi difficile de l’état des livres

Recherche laborieuse : absence d’un système de recherche efficace, rendant l’accès aux livres complexe

Manque de statistiques : pas de suivi clair des livres disponibles, empruntés ou perdus, limitant l’optimisation des collections

## Fonctionnalités
Gestion des livres : ajout, mise à jour et suppression des livres via titre, auteur et ISBN

Recherche efficace : recherche de livres par titre ou auteur

Gestion des emprunts/retours : suivi des emprunts et retours avec mise à jour automatique de l’état des livres

Rapports statistiques : génération de rapports sur les livres disponibles, empruntés et perdus

## Histoires Utilisateurs
Ajouter un livre : saisir titre, auteur et ISBN (statut initial : disponible)

Lister les livres disponibles : afficher la liste des livres avec titre, auteur et statut

Rechercher un livre : rechercher par titre ou auteur et afficher les résultats

Emprunter un livre : saisir l’ISBN pour enregistrer un emprunt, mettre à jour le statut en « emprunté » et enregistrer les informations de l’emprunteur (nom, numéro d’étudiant, etc.)

Retourner un livre : saisir l’ISBN pour marquer le livre comme « disponible » et supprimer les informations d’emprunt

Lister les livres empruntés : afficher les livres empruntés avec leurs informations (titre, auteur, emprunteur, date d’emprunt)

Supprimer un livre : supprimer un livre via son ISBN

Modifier un livre : mettre à jour les informations (titre, auteur) d’un livre via son ISBN

Générer un rapport : produire un rapport statistique sur les livres disponibles, empruntés et perdus

