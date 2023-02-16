# Workshop3&4-Algorand
Bienvenue pour ce cinquième workshop :)

🧵 Aujourd'hui nous allons nous concentrer sur un sujet en particulier : les smarts contracts et le déploiement de notre marketplace. Le smart contract, sera enfaite le code qui nous permettra de déployer notre marketplace 

Nous verrons comment : 

✔️ Déployer des smart contracts sur Algorand 

✔️ Déployer notre marketplace sur Algorand 


<details>
  <summary>
  <h1>  Création de la dApp  </h1>
  </summary>
  
1. Création d'un nouveau dossier sur votre ordinateur : 
indication -> ls/mkdir/cd depuis votre terminal 

2. Vous pouvez clôner l'intégralité du répertoire dans votre nouveau document 
  ~~~
  git clone https://github.com/herdaoFrance/Workshop3-4-Algorand.git
  ~~~

3. Dans ce même workspace VSCode, ouvrez le dossier sandbox précedement utilisé (dans les workshop précédent) . 

4. Copiez le chemin du fichier "marketplace_approval" ainsi que le fichier "marketplace_clear"
Dans votre terminal (sandbox), écrivez ces lignes de code : 
  ~~~
  .\sandbox copyTo "chemin_vers_marketplace_approval" 
  .\sandbox copyTo "chemin_vers_marketplace_clear" 
  ~~~
  
5. Création d'un compte Algorand et d'un wallet sur Algorand : 
  Sur votre terminal, voici les commandes que vous pouvez saissir. Pensez à bien sauvegarder votre mot de passe. 
  ~~~
  ./sandbox goal enter 
  goal wallet new NOM DE VOTRE WALLET
  ~~~
  Votre wallet sera bien créer. Ensuite, vous pouvez créer un compte algorand via cette commande (ou réutiliser le compte précédément généré) 
  ~~~
  goal account new 
  ~~~
  
  Une fois cela créer, pensez à alimenter votre compte algorand de faucet, afin d'effectuer les transactions 
 6. La création de la marketplace :
  ~~~
./sandbox goal enter 
  ~~~
  
  ~~~
goal app create --creator 'ICI L'ADRESS DE TON COMPTE" --approval-prog marketplace_approval.teal --clear-prog marketplace_clear.teal --note tutorial-marketplace:uv1 --global-byteslices 3 --global-ints 2 --local-byteslices 0 --local-ints 0 --app-arg str:TestName --app-arg str:TestImage --app-arg str:TestDescription --app-arg int:1000000
  ~~~
  

</details>


<details>
  <summary>
   <h1> Ressources supplémentaire Algorand </h1>
  </summary>
Nous avons finis de parcourir l'ecosysteme Algorand. Félicitation à toi si tu est arrivé jusqu'à là ! 🎆 
Je te laisse avec des ressources sur lequelles tu peux dig d'avantage sur l'écosystème Algorand 
  Github réunissant tous les projets sur Algorand (en englais) : https://github.com/aorumbayev/awesome-algorand#name-services

  
</details>
