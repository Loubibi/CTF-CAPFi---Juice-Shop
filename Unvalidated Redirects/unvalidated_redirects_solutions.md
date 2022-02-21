## Outdate Whitelist

### Défi : Se rediriger vers l'une des adresses de crypto-monnaies qui ne font plus l'objet de promotion.
1. Log in to the application with any user.
2. Visit the _Your Basket_ page and expand the _Payment_ and
   _Merchandise_ sections with the "credit card"-button.
3. Perceive that all donation links are passed through the `to`
   parameter of the route `/redirect`
4. Open `main.js` in your browser's DevTools
5. Searching for `/redirect?to=` and stepping through all matches you
   will notice three functions that are called only from hidden buttons
   on the _Your Basket_ page:

   ![Hidden crypto currency link functions](img/cryptoLinks.png)
6. Open one of the three, e.g.
   <http://localhost:3000/redirect?to=https://blockchain.info/address/1AbKfgvw9psQ41NbLi8kufDQTezwG8DRZm>
   to solve the challenge.




![image](https://user-images.githubusercontent.com/37535317/155037088-bc6aee37-3cd0-409f-b6c6-a610193070cc.png)
