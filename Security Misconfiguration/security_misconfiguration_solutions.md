## Deprecated Interface
### Défi : Utiliser une interface B2B dépréciée qui n'a pas été correctement fermée.

Ce défi peut se réaliser en utilisant Chrome `Inspect` > `Sources` > `main-es2015.js`. Faites une recherche en utilisant `Ctrl + F` pour le mot clé `upload`. 

Observez que le `allowedMimeType` qui autorise les fichiers de type `xml`. Si vous naviguez dans le formulaire `Complaint` et cliquez sur upload file, vous remarquerez que les seuls fichiers autorisés sont les fichiers avec les extensions `pdf` et `zip`. 

![image](https://user-images.githubusercontent.com/37535317/155036370-a117d5e8-ab19-43f5-8ef2-087edad955cc.png)

Choisissez `Tous les fichiers (*.*)` dans le formulaire de téléchargement et soumettez un fichier `xml` pour compléter le défi. 

L'examen de la console javascript montre qu'il y a un [Code d'erreur 410 (Gone)].(https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/410) 
