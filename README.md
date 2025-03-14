# 🔐 Authentification avec Spring Boot, Angular et Keycloak

## 📚 Description du projet

Ce projet met en place un **système d'authentification sécurisé** en utilisant **Keycloak** comme fournisseur d'identité (Identity Provider), **Spring Boot** pour la gestion du backend, et **Angular** pour le frontend.

L'objectif est d'assurer une **gestion centralisée de l'authentification et de l'autorisation** des utilisateurs dans une architecture **full-stack**. L'application utilise **OpenID Connect (OIDC)** et **OAuth 2.0** via Keycloak pour protéger les API backend et sécuriser l'accès aux pages frontend Angular.

---

## ⚙️ Technologies utilisées

- **Keycloak** : Fournisseur d'identité open-source pour la gestion des utilisateurs et des rôles.
- **Spring Boot (Java)** : Backend REST API avec sécurisation OAuth 2.0 / OIDC.
- **Angular** : Frontend SPA (Single Page Application) consommant les API sécurisées.
- **Spring Security** : Intégration de la couche de sécurité dans l'application backend.
- **Keycloak Angular Library** : Gestion de la session et des tokens sur le frontend.

---

## 🚀 Fonctionnalités principales

- ✅ Authentification via Keycloak (Login / Logout)
- ✅ Gestion des utilisateurs et rôles dans Keycloak
- ✅ Protection des endpoints REST avec Spring Security
- ✅ Accès aux routes Angular en fonction des rôles utilisateurs
- ✅ Récupération et gestion des tokens JWT (Access Token / Refresh Token)
- ✅ Déconnexion sécurisée avec redirection vers Keycloak

---

## 🗂️ Architecture générale

```plaintext
Frontend (Angular) ---> Authentification avec Keycloak (OIDC)
                                |
Backend (Spring Boot) <--- Validation JWT / Sécurisation API avec Spring Security

