# Plan de test – Handball Management

## 1. Objectif
Vérifier la qualité fonctionnelle des principales fonctionnalités du site Handball Management :
- Connexion utilisateur
- Inscription joueur / entraîneur
- Navigation dans les menus
- Formulaire de contact

## 2. Périmètre
Inclus :
- Pages de connexion et d’inscription
- Navigation Joueurs / Entraîneurs / Managers / Préparateurs
- Formulaire de contact
- Sécurité basique (HTTPS)

Exclus :
- Backend et base de données interne (non accessibles)
- Performance et charge

## 3. Environnement
- OS : Windows 11
- Navigateur : Chrome (version la plus récente)
- URL : https://www.handball-management.com/

## 4. Stratégie
- Tests manuels documentés dans `TestCases.md`
- Suivi des anomalies dans Jira et `BugReports/`
- Automatisation prévue pour les scénarios critiques (login, inscription)
