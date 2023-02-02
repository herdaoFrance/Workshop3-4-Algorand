# Workshop3&4-Algorand
Bienvenue pour ce troisième et quatrième workshop  :)

🧵 Aujourd'hui nous allons nous concentrer sur un sujet en particulier : les smart contracts, particulièrement sur Algorand. 

Nous verrons comment : 

✔️ Coder dans le langage de programmation PyTeal 

✔️ Créer un smart contract sur Algorand 

✔️ Exécuter notre premier smart contract 



<details>
  <summary>
  <h1>🤝 Ecriture du smart contract </h1>
  </summary>
 Notre smart contract sera enfaite un smart contract créant une Dapp qui sera une marketplace 

Vous pourrez trouvez le code dans le réportoire, que vous pouvez copier/coller dans vos fichier algorand. 


</details>

<details>
  <summary>
  <h1>Commande pour déployer notre marketplace </h1>
  </summary>
Les variables ci-dessous, seront simplement les chemins à copier/coller depuis le fichier désirer. Si le fichier marketplace_approbation.teal, placez vous sur ce fichier, puis avec un clic droit, il sera possible de récupérer le chemin du contrat. 


  ${CHEMIN_VERS_MARKETPLACE_APPROVAL}: Chemin vers la marketplace_approval.teal
  
  ${CHEMIN_VERS_MARKETPLACE_CLEAR} : Chemin vers marketplace_clear.teal 

1. Création d'un nouveau dossier sur votre ordinateu : 
indication -> ls/mkdir/cd depuis votre terminal 

2. Vous pouvez clôner l'intégralité du répertoire dans votre nouveau document 
  ~~~
  git clone https://github.com/herdaoFrance/Workshop3-4-Algorand.git
  ~~~

3. Dans ce même workspace sur VSCode, ouvrez le dossier sandbox précedement utilisé. 

4. Copiez le chemin du fichier "marketplace_approval" 
Dans votre terminal (sandbox), écrivez ces lignes de code : 
  ~~~
  .\sandbox copyTo "chemin_vers_marketplace_approval" 
  ~~~
  
5. De même pour le fichier "marketplace_clear" 
  ~~~
  .\sandbox copyTo "chemin_vers_marketplace_clear" 
  ~~~
  
  
  ~~~
  ./sandbox goal app create --creator ${CHEMIN_VERS_MARKETPLACE_APPROBATION} --approval-prog marketplace_approbation.teal --clear-prog marketplace_efface.teal --note tutprial-marketplace:uv1 --global-byteslices 3 --global-ints 2 --local-byteslices 0 --locall-ints 0 --app-arg str:TestName --app-arg str:TestImage --app-arg str:TestDescription --app-arg int:1000000
  ~~~
  

</details>
