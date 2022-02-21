## Outdate Whitelist

### Défi : Se rediriger vers l'une des adresses de crypto-monnaies qui ne font plus l'objet de promotion.

1. Connectez-vous à l'application avec n'importe quel utilisateur.
2. Visitez la page `_Votre panier_` et développez les sections `_Paiement_` et `_Merchandise_` avec le bouton "carte de crédit".
3. Percevez que tous les liens vers les dons sont passés par le paramètre `to` de la route `/redressing`.
   de la route `/redirect`.
4. Ouvrez `main.js` dans les DevTools de votre navigateur.
5. En recherchant `/redirect?to=` et en parcourant toutes les correspondances vous
   vous remarquerez trois fonctions qui ne sont appelées que par des boutons cachés
   sur la page _Votre panier_ :

![image](https://user-images.githubusercontent.com/37535317/155037088-bc6aee37-3cd0-409f-b6c6-a610193070cc.png)

6. Ouvrez l'une de ces trois fonctions, par exemple
   <http://@IP:3000/redirect?to=https://blockchain.info/address/1AbKfgvw9psQ41NbLi8kufDQTezwG8DRZm>
   pour résoudre le défi.
