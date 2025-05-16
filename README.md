# App-Gestion-Patient

## 🩺 Overview

`App-Gestion-Patient` est une application web Java construite avec **Spring MVC**, **Thymeleaf** et **Spring Data JPA**, conçue pour la gestion des dossiers patients dans un établissement médical. Elle offre une interface conviviale permettant aux professionnels de santé de consulter, créer et supprimer des fiches patients facilement.

---

## ✨ Fonctionnalités

- **📋 Liste des Patients** : Tableau avec détails essentiels (ID, nom, date de naissance, état de santé, score), recherche et filtres intégrés.
- **🔄 Pagination** : Navigation fluide entre les pages avec boutons « Précédent » et « Suivant ».
- **➕ Création de Patient** : Formulaire avec champs obligatoires et validation côté serveur. Le patient ajouté s'affiche immédiatement.
- **🗑️ Suppression de Patient** : Bouton de suppression avec confirmation. Les patients sont supprimés de la base de données et de l'affichage.

---

## 🛠️ Technologies Utilisées

- **Spring MVC** : Architecture Modèle-Vue-Contrôleur.
- **Spring Data JPA** : Accès aux données avec MySQL.
- **Thymeleaf** : Moteur de templates pour le rendu HTML dynamique.
- **Bootstrap 5** : Design responsive et moderne.
- **Font Awesome** : Icônes pour une meilleure UX.

---

## 📁 Structure du Projet


```
src/
├── main/
│   ├── java/
│   │   └── com/example/patientapp/
│   │       ├── controllers/
│   │       │   └── PatientController.java
│   │       ├── entities/
│   │       │   └── Patient.java
│   │       ├── repositories/
│   │       │   └── PatientRepository.java
│   │       └── PatientAppApplication.java
│   └── resources/
│       ├── static/
│       ├── templates/
│       │   └── index.html
│       │   └── createPatient.html
│       │   └── template1.html
│       └── application.properties
```


---

## ⚙️ Prérequis

- Java 21+
- Maven
- MySQL (ou équivalent)
- XAMPP (ou autre outil pour exécuter MySQL en local)

---

## 🚀 Installation

1. **Cloner le dépôt** :
   ```bash
   git clone https://github.com/7soufiane/App-Gestion-Patient.git
   cd App-Gestion-Patient

## 🛠️ Configuration de la base de données

1. Lancer **MySQL** via **XAMPP** ou tout autre outil.
2. Créer une base de données nommée `patientsdb`.
3. Modifier le fichier `src/main/resources/application.properties` :

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/patientsdb?createDatabaseIfNotExist=true
spring.datasource.username=root
spring.datasource.password=
spring.jpa.hibernate.ddl-auto=update
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.database-platform=org.hibernate.dialect.MySQL8Dialect
```
## 🚀 Lancement de l'application

Pour démarrer l'application, exécute la commande suivante :

```bash
mvn spring-boot:run
```
## 📌 Utilisation

- 👁️ **Voir les patients** : Accède à `/index` pour afficher la liste des patients avec options de recherche et pagination.
- ➕ **Ajouter un patient** : Accède à `/createPatient`, remplis le formulaire et soumets-le.
- 🗑️ **Supprimer un patient** : Clique sur le bouton de suppression associé à un patient. Une confirmation est demandée.

## 🤝 Contribuer

Les contributions sont les bienvenues ! Voici comment participer :

1. **Forker** le dépôt.
2. Créer une nouvelle branche :
   ```bash
   git checkout -b feature/nom-de-votre-feature
3. Ajouter vos modifications :
   ```bash
   git commit -m "Ajout de [votre fonctionnalité]"

4. Pousser la branche :
   ```bash
   git push origin feature/nom-de-votre-feature

5. Ouvrir une Pull Request.

## 📄 Licence

Ce projet est sous licence **MIT** – voir le fichier [LICENSE](LICENSE) pour plus d’informations.

---

## 📬 Contact

Pour toute question ou suggestion :

- GitHub : [7soufiane](https://github.com/7soufiane)
