# Workshop3&4-Algorand
Bienvenue pour ce cinquième workshop :)

🧵 Aujourd'hui nous allons nous concentrer sur un sujet en particulier : les smarts contracts et le déploiement de notre marketplace. Le smart contract, sera enfaite le code qui nous permettra de déployer notre marketplace 

Nous verrons comment : 

✔️ Déployer des smart contracts sur Algorand 

✔️ Déployer notre marketplace sur Algorand 



</details>

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

4. Copiez le chemin du fichier "marketplace_approval" 
Dans votre terminal (sandbox), écrivez ces lignes de code : 
  ~~~
  .\sandbox copyTo "chemin_vers_marketplace_approval" 
  ~~~
  
5. De même pour le fichier "marketplace_clear" 
  ~~~
  .\sandbox copyTo "chemin_vers_marketplace_clear" 
  ~~~
  
 6. La création de la marketplace :
  ~~~
  ./sandbox goal app create --creator ${CHEMIN_VERS_MARKETPLACE_APPROBATION} --approval-prog marketplace_approbation.teal --clear-prog marketplace_efface.teal --note tutprial-marketplace:uv1 --global-byteslices 3 --global-ints 2 --local-byteslices 0 --locall-ints 0 --app-arg str:TestName --app-arg str:TestImage --app-arg str:TestDescription --app-arg int:1000000
  ~~~
  

</details>

<details>
  <summary>
  <h1> Ressources supplémentaire Algorand </h1>
    <summary/>
    Github réunissant tous les projets sur Algorand (en englais) : https://github.com/aorumbayev/awesome-algorand#name-services
  
  </details>
