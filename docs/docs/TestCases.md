# Cas de test – Handball Management

| ID    | Titre                              | Étapes                                                                 | Résultat attendu                                                  | Statut |
|------:|------------------------------------|------------------------------------------------------------------------|------------------------------------------------                   |:------:|
| TC-01 | Connexion valide                   | 1. Ouvrir /connexion/ → 2. Saisir email valide + mot de passe valide → 3. Cliquer « Connexion » | Redirection vers tableau de bord         | ☐      |
| TC-02 | Connexion mot de passe incorrect   | 1. Ouvrir /connexion/ → 2. Email valide + mot de passe invalide → 3. Cliquer « Connexion » | Message « Identifiants invalides »            | ☐      |
| TC-03 | Inscription joueur (succès)        | 1. Ouvrir /connexion/inscri_joueurs.php → 2. Champs valides → 3. Soumettre | Compte créé, redirection vers login                           | ☐      |
| TC-04 | Inscription joueur (email utilisé) | 1. Ouvrir /connexion/inscri_joueurs.php → 2. Email déjà utilisé → 3. Soumettre | Message « email déjà utilisé »                            | ☐      |
| TC-05 | Inscription entraîneur (succès)    | 1. Ouvrir /connexion/inscri_entraineur.php → 2. Champs valides → 3. Soumettre | Compte créé, redirection vers login                          | ☐      |
| TC-06 | Confirmation mdp différente        | 1. Ouvrir /connexion/inscri_entraineur.php → 2. MDP A → 3. Confirmation ≠ A → 4. Soumettre | Message « Mots de passe ne correspondent pas »   | ☐      |
