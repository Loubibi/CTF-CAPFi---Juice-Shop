## Zero Stars 
### Donnez un avis de zéro étoile au magasin.

Cliquez sur `Customer Feedback` et remplissez le formulaire de feedback. Activez un intercepteur de requête HTTP comme Burpsuite, modifiez le paramètre `rating` de la requête POST en `0`. Transmettez la requête modifiée pour compléter le défi

exemple :

```
POST /api/Feedbacks/ HTTP/1.1
Hôte : @IP:3000
...
{"captchaId":0,"captcha":"-2","comment":"Nul!","rating":0}
```
