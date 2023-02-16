# Workshop3&4-Algorand
Bienvenue pour ce cinquième workshop :)

🧵 Aujourd'hui nous allons nous concentrer sur un sujet en particulier : le front end et le déploiement d'une dApp sur le web

Nous verrons comment : 

✔️ Transformer un design en front-end 

✔️ Déployer sa dApp sur le front 




<details>
  <summary>
  <h1>🤝 Générer un design front - end  </h1>
  </summary>
Lors d'un hackathon, vous serez peut-être ammené à créer un front-end, qui sera l'interface de votre produit. Un outil permet de rapidement créer un front-end à partir d'un design : plasmic. 
 
Vous pourrez trouvez le code dans le réportoire, que vous pouvez copier/coller dans vos fichier algorand. 


</details>

<details>
  <summary>
  <h1> Interaction avec la blockchain : le wallet  </h1>
  </summary>
Précédemment, nous avons créer sur la blockchain Algorand, un compte et nous avons effectué notre première transaction. Pour créer une vrai dApp ou décentralized  Application, nous souhaitons implémenter une 


  ${CHEMIN_VERS_MARKETPLACE_APPROVAL}: Chemin vers la marketplace_approval.teal
  
  ${CHEMIN_VERS_MARKETPLACE_CLEAR} : Chemin vers marketplace_clear.teal 

1. Création d'un nouveau dossier sur votre ordinateur : 
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
  
 6. La création de la marketplace :
  ~~~
  ./sandbox goal app create --creator ${CHEMIN_VERS_MARKETPLACE_APPROBATION} --approval-prog marketplace_approbation.teal --clear-prog marketplace_efface.teal --note tutprial-marketplace:uv1 --global-byteslices 3 --global-ints 2 --local-byteslices 0 --locall-ints 0 --app-arg str:TestName --app-arg str:TestImage --app-arg str:TestDescription --app-arg int:1000000
  ~~~
  

</details>

<details>
  <summary>
  <h1> Ressources supplémentaire Algorand </h1>
    <summary/>
    
    - Github réunissant tous les projets sur Algorand (en englais) : https://github.com/aorumbayev/awesome-algorand#name-services
    - 
  
  </details>
