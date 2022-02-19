## Bjoern's Favorite Pet
### Réinitialiser le mot de passe du compte OWASP de Bjoern via le mécanisme Mot de passe oublié avec la réponse originale à sa question de sécurité.
### Catégorie : Authentification cassée

A partir du défi précédent, après avoir piraté le panneau `/administration` en utilisant l'utilisateur admin. Nous avons une liste des emails de login de Bjoern utilisés pour le magasin de jus. En utilisant la fonction d'oubli du mot de passe, il y a un login email particulier `bjoern@owasp.org` qui pose la question `Nom de votre animal préféré``. 

En cherchant sur Google l'animal préféré de bjoern, la réponse est "Zaya" dans la page des solutions. Même si la solution prévue se trouve dans une conférence donnée par Bjoern où il enregistre un compte dans Juiceshop avec la réponse à cette question de mot de passe oublié. La leçon clé ici est de ne jamais utiliser une question de mot de passe oublié qui pourrait être facilement répondue par n'importe qui en faisant une reconnaissance de base et une recherche ciblée !
