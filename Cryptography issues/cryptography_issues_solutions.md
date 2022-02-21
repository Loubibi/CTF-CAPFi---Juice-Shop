## Weird Crypto

### Défi : Informez le magasin sur un algorithme ou une bibliothèque qu'il ne devrait absolument pas utiliser comme il le fait.

1. On sait que le site se sert d'un serveur FTP pour son transfert de fichier.
2. En sachant cela, il faut se connecter au serveur à travers le protocole FTP sur son navigateur de la façon suivante `http://@IP:3000/ftp`. Puis, il faut récupérer le fichier `package.json.bak`qui est un fichier de "Backup".
3. Dans ce fichier on trouve des informations intéressantes dont celle-ci :

![image](https://user-images.githubusercontent.com/37535317/155037772-047ffd60-fc54-40b9-987a-a19385759a88.png)

4. On aperçoit la librairie "z85".
5. Il suffit de ce rendre dans la section "Feedback Customers" et de rentrer en commentaire "z85" pour valider le challenge.
