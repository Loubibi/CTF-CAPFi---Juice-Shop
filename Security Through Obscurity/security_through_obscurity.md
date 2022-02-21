## Privacy Policy Inspection

### Défi : Prouvez que vous avez réellement lu notre politique de confidentialité.

1. Ouvrez <http://@IP:3000/#/privacy-security/privacy-policy>.
2. En déplaçant le curseur de votre souris sur chaque paragraphe, vous ferez apparaître un effet de feu sur certains mots ou parties de phrases.
   apparaître sur certains mots ou parties de phrases.

   ![image](https://user-images.githubusercontent.com/37535317/155036801-59194063-bf48-4a30-b5c2-1a5d7472e158.png)

3. Inspectez le HTML dans votre navigateur et notez tout le texte à l'intérieur des balises `<span
   class="hot">`, qui sont `http://localhost`, `Nous pouvons également`,
   `s'instruire`, `refuser tout`, `raisonnablement nécessaire` et
   `responsabilité`.
4. Combinez-les dans l'URL
   <http://localhost:3000/we/may/also/instruct/you/to/refuse/all/reasonably/necessary/responsibility>
   (en ajoutant le port du serveur si nécessaire) et résolvez le défi en le
   le visitant.

Il semble que l'équipe de Juice Shop n'ait pas suffisamment apprécié votre effort de lecture pour vous fournir une gratification, même minime.
efforts de lecture pour vous donner ne serait-ce qu'une petite satisfaction, car vous ne recevrez
seulement une `404 Error : ENOENT : no such file or directory, stat
'/app/frontend/dist/frontend/assets/private/thank-you.jpg'`.
