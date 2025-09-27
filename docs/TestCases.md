# Cas de test – Handball Management

| ID    | Titre                              | Étapes                                                                 | Résultat attendu                               | Statut |
|------:|------------------------------------|------------------------------------------------------------------------|------------------------------------------------|:------:|
| TC-01 | Connexion valide                   | 1. Ouvrir /connexion/ → 2. Email valide + mot de passe valide → 3. Cliquer « Connexion » | Redirection vers tableau de bord               | ❌ Fail (voir BUG-002) |
| TC-02 | Connexion mot de passe incorrect   | 1. Ouvrir /connexion/ → 2. Email valide + mot de passe invalide → 3. Cliquer « Connexion » | Message « Identifiants invalides »             | ✅ Pass |
| TC-03 | Inscription joueur (succès)        | 1. Ouvrir /connexion/inscri_joueurs.php → 2. Champs valides → 3. Soumettre | Compte créé, redirection login                 | ✅ Pass |
| TC-04 | Inscription joueur (email utilisé) | 1. Ouvrir /connexion/inscri_joueurs.php → 2. Email déjà utilisé → 3. Soumettre | Message « email déjà utilisé »                 | ☐ Non exécuté |
| TC-05 | Inscription entraîneur (succès)    | 1. Ouvrir /connexion/inscri_entraineur.php → 2. Champs valides → 3. Soumettre | Compte créé, redirection vers login            | ☐ Non exécuté |
| TC-06 | Confirmation mdp différente        | 1. Ouvrir /connexion/inscri_entraineur.php → 2. MDP A → 3. Confirmation ≠ A → 4. Soumettre | Message « Mots de passe ne correspondent pas » | ☐ Non exécuté |
| TC-07 | Affichage de la liste des joueurs      | 1. Ouvrir la page “Joueurs”<br>2. Observer la liste                                   | La liste s’affiche avec cartes (nom, âge, poste, pays) | ✅ Pass |
| TC-08 | Filtrage par nom/prénom                | 1. Dans le champ “Nom ou Prénom”, saisir `Firas`<br>2. Valider                        | La liste affiche uniquement les joueurs correspondant | ✅ Pass |
| TC-09 | Filtrage par poste                     | 1. Sélectionner un poste (ex: pivot)<br>2. Valider                                    | La liste affiche uniquement les joueurs avec ce poste | ✅ Pass |
| TC-10 | Filtrage par pays                      | 1. Sélectionner “Tunisie” dans “Pays”<br>2. Valider                                   | La liste affiche uniquement les joueurs tunisiens | ✅ Pass |
| TC-11 | Filtrage combiné (pays + poste)        | 1. Sélectionner “Tunisie” + “pivot”<br>2. Valider                                     | Seuls les pivots tunisiens apparaissent         | ✅ Pass |
| TC-12 | Aucun résultat trouvé                  | 1. Rechercher un joueur avec un nom inexistant<br>2. Valider                           | Message “Aucun joueur trouvé” ou liste vide     | ❌ Fail (BUG-003) |
| TC-13 | Navigation vers profil joueur          | 1. Cliquer sur la carte d’un joueur (ex: Firas Farhat)                                | Page détail/profil joueur s’ouvre               | ☐ Non exécuté |

