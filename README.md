# TP 1 – Spring Boot REST API (CRUD)

## Description

Ce projet est une **API RESTful développée avec Spring Boot** permettant la gestion des produits via les opérations **CRUD**.
L’application utilise une **architecture en couches** et peut être exécutée sous différents **profils Spring** (dev, prod, integration).

## Architecture

* Controller : exposition des endpoints REST
* Service : logique métier
* Model : entités métier
* Configuration : gestion des profils et paramètres

Serveur embarqué : Tomcat

## Endpoints principaux

* `GET /hello` : test de l’API
* `GET /products` : liste des produits
* `GET /products/{id}` : produit par ID
* `POST /products` : ajouter un produit
* `PUT /products/{id}` : modifier un produit
* `DELETE /products/{id}` : supprimer un produit

Formats supportés : JSON et XML

## Exécution

### Lancer l’application

```bash
mvn spring-boot:run
```

### Avec un profil spécifique

```bash
mvn spring-boot:run -Dspring-boot.run.profiles=prod
```

### Générer et exécuter le JAR

```bash
mvn clean package
java -jar target/rest-api-demo.jar
```

## Tests

Les services REST ont été testés avec Postman.

## Objectifs pédagogiques

* Comprendre Spring Boot
* Créer une API REST
* Implémenter le CRUD
* Gérer les profils Spring
* Packager une application Java en JAR

---

**Binôme** : **MOHAMMED EL KHAYATI & MOUAD MOUDID**
**Classe** : **5IIR-11G2**
