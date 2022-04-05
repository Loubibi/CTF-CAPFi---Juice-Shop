## Missing Encoding
### Récupérer la photo du chat de Bjoern en mode "combat en mêlée".

Connectez-vous en tant qu'utilisateur (créez en un si ce n'est pas déjà le cas). Depuis le menu latéral, naviguez jusqu'à `Photo Wall`. Il y aura 3 photos. Avec la première photo il y aura un lien brisé `😼 #zatschi #whoneedsfourlegs`.

Pour voir le lien complet de l'image avec le lien brisé, cliquez avec le bouton droit de la souris sur le lien brisé en utilisant le navigateur Chrome > `Inspect` > `Elements` et voyez que c'est 

```
assets/public/images/uploads/😼-#zatschi-#whoneedsfourlegs-1572600969477.jpg
```

Si vous encodez les caractères 
```
😼-#zatschi-#whoneedsfourlegs-1572600969477.jpg
```

vous obtiendrez 
```
%F0%9F%98%BC-%23zatschi-%23whoneedsfourlegs-1572600969477.jpg
```

Nous connaissons maintenant le chemin absolu de l'image, naviguez vers `http://192.168.247.136:3000/assets/public/images/uploads/%F0%9F%98%BC-%23zatschi-%23whoneedsfourlegs-1572600969477.jpg` pour compléter ce défi

Note : Nous pouvons observer les requêtes du client au serveur en utilisant les outils de développement de Chrome `Network`. Si nous filtrons les requêtes enregistrées en cliquant sur `img`, nous pouvons voir que l'une des url d'image demandée était `http://@IP:3000/assets/public/images/uploads/%F0%9F%98%BC-`, qui est en fait l'url "semi codée" de l'image du chat. Il s'avère que le caractère `#` n'a pas été encodé et que l'image n'a pas été trouvée.
