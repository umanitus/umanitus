1 joueur **_Serveur_** veut revendre un produit qu'il a au meilleur prix

1. Il crée une carte vente de son produit et donne son coût plancher  
2. Il partage sa carte avec ses connaissances  
3. Chaque connaissance servie a trois coups possibles  
   * Passer son tour  
   * Miser son prix plafond en tant que **_Client_**
   * Faire tourner la carte à ses connaissances en tant que **_Procureur_** 
4. A la condition donnée par le **_Serveur_**, la partie finit en :
   * Nulle s'il n'y a aucun **_Client_** supérieur au coût
   * Compte simple s'il y a un **_Client_** supérieur au coût  
       * Le client paie le coût plancher
       * La valeur créée est 1 point et va au **_Client_**
   * Compte double s'il y a deux **_Client_** supérieurs au coût 
       * Si les 2 **_Client_** sont de deux connaissances différentes :
           * Le meilleur **_Client_** paie le prix du deuxième meilleur
           * La valeur créée en plus est l'écart entre le deuxième meilleur et le coût, qui va au **_Serveur_**
       * Si les 2 clients sont du même **_Procureur_** :   
           * Le meilleur **_Client_** paie aussi le prix du deuxième meilleur
           * La valeur créée en plus va cette fois au **_Procureur_**
   * Compte triple s'il y a trois **_Client_** supérieurs au coût dont les deux meilleurs du même **_Procureur_** :  
       * Le **_Client_**, le **_Serveur_** et le **_Procureur_** créent et récupère de la valeur
