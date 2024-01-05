# Virtualisation et conteneur 
Ce projet a été réalisé par Anaïs DERAMCHIA et Romain FOURNET

## INTRODUCTION
Le projet HumansBestFriend - ApplicaFon Distribuée avec Docker et Kubernetes a pour objecFf la créaFon d’une applicaFon distribuée simple, appelée HumansBestFriend, qui permet aux uFlisateurs de voter pour leur animal de compagnie préféré, qu'il s'agisse de chats ou de chiens. L'applicaFon sera déployée à l'aide de Docker et Kubernetes pour illustrer la gesFon de conteneurs et d'orchestraFon dans un environnement distribué. Le projet sera réalisé à l'intérieur d'une machine virtuelle exécutant Docker et Docker Compose.

## DÉROULEMENT
Dans le cadre de notre projet, notre première étape a été de meYre en place notre environnement ESXi et de lancer notre machine virtuelle. Une fois ceYe configuraFon réalisée, nous avons établi une connexion SSH entre le terminal de notre PC et notre machine virtuelle en uFlisant la commande suivante :
SSH romain@172.16.223.129
Afin de pouvoir exploiter les fichiers disponibles sur GitHub, nous avons procédé à l'installaFon de Docker en suivant les instrucFons détaillées sur le lien suivant : hYps://docs.docker.com/engine/install/ubuntu/
CeYe première étape cruciale nous a permis de préparer notre environnement pour la suite du projet.
Suite à l'installaFon de Docker, nous avons également installé le plugin Compose en suivant les direcFves spécifiées dans la documentaFon : hYps://docs.docker.com/compose/install/linux/#install-using-the-repository
CeYe étape a été essenFelle pour la gesFon des services et la configuraFon de l'ensemble de notre applicaFon.
De même, nous avons créé un répertoire et ensuite, nous avons procédé au clonage du projet à parFr du référenFel GitHub du professeur. Le clonage a été réalisé en uFlisant la commande git clone suivie de l'URL du référenFel.
Le cœur de notre travail a véritablement commencé avec la créaFon de deux fichiers clés : "docker-compose.images.yml" et "docker-compose.yml".
Le premier fichier, "docker-compose.images.yml", était responsable de la construcFon des images de l'applicaFon à parFr du contenu du fichier Docker fourni.
Le second fichier, "docker-compose.yml", était dédié au déploiement de l'applicaFon et à la gesFon de tous les conteneurs nécessaires.
Lors de la créaFon de ces fichiers, nous avons minuFeusement suivi la procédure, en spécifiant notamment que le service de vote serait accessible sur le port localhost 5002 et les résultats du vote sur le port localhost 5001.
   
Une fois le code rédigé, nous avons exécuté la commande suivante pour lancer l'ensemble du système :
sudo docker compose up : CeYe commande est uFlisée pour lancer et démarrer les services définis dans un fichier de configuraFon Docker Compose
Enfin, pour visualiser les résultats de notre travail, nous nous sommes connectés à Internet en ouvrant différents onglets de navigateur et en accédant aux adresses suivantes : 172.16.223.129:5002 (service de vote)
172.16.223.129:5001 (résultats du vote)
Cela nous a permis de vérifier le bon foncFonnement de notre applicaFon distribuée et de constater concrètement les résultats de notre travail sur ce projet.
## CONCLUSION 
En conclusion, le projet HumansBestFriend a consFtué une expérience enrichissante dans la concepFon et le déploiement d'une applicaFon distribuée. En suivant rigoureusement les étapes, depuis la configuraFon iniFale de l'environnement ESXi jusqu'à la mise en œuvre des fichiers Docker Compose, notre équipe a acquis une compréhension approfondie de la gesFon de conteneurs à l'aide de Docker et de l'orchestraFon avec Kubernetes.
En ce qui concerne les difficultés rencontrées, elles furent minimes (type problème de droit ou d’installaFon) mais dans l’ensemble tout était très bien indiqué et détaillé dans les consignes.

