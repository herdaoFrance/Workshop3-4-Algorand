# Workshop3-Algorand
Bienvenue pour ce troisième workshop :)

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
  <h1> Commande pour déployer notre marketplace </h1>
  </summary>
Les variables ci-dessous, seront simplement les chemins à copier/coller depuis le fichier désirer. Si le fichier marketplace_approbation.teal, placez vous sur ce fichier, puis avec un clic droit, il sera possible de récupérer le chemin du contrat. 

  ${CHEMIN_VERS_MARKETPLACE_APPROBATION}: Chemin vers la marketplace_approbation.teal
  
  ${CHEMIN_VERS_MARKETPLACE_EFFACE} : Chemin vers marketplace_efface.teal 

  ~~~
  ./sandbox goal app create --creator ${CHEMIN_VERS_MARKETPLACE_APPROBATION} --approval-prog marketplace_approbation.teal --clear-prog marketplace_efface.teal --note tutprial-marketplace:uv1 --global-byteslices 3 --global-ints 2 --local-byteslices 0 --locall-ints 0 --app-arg str:TestName --app-arg str:TestImage --app-arg str:TestDescription --app-arg int:1000000
  ~~~
  

</details>
