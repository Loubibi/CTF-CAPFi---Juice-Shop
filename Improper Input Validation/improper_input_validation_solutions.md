## Admin Registration
### Enregistrez-vous en tant qu'utilisateur avec des privilèges d'administrateur.

Si vous utilisez burp pour intercepter le trafic lors de la création d'un nouvel utilisateur, vous remarquerez qu'il y a un appel rest api fait à `/api/Users` et que les entrées d'enregistrement sont ajoutées comme paramètres json.

Des tests plus poussés avec l'api de repos révéleront qu'il y a un paramètre qui définit le `rôle`. Par exemple, si vous envoyez une requête POST vide `/api/Users` sans paramètres, vous obtiendrez la réponse suivante :

![image](https://user-images.githubusercontent.com/37535317/155035607-b5c134dc-d8b4-482c-974e-88771d473eb1.png)

Envoyez une autre requête `POST /api/Users/` avec les paramètres suivants 
`{"nom d'utilisateur" : "adminhacker", "email" : "admin@hack.com", "password" : "admin", "role" : "admin"}``

![Uploading image2.png…]()
