---
layout: project
lang: fr
title: "Serveur de Jeu Privé"
image: "/img/portfolio/HSQL-Acore.png" # Hero image
category: "Une structure complète de serveur privé pour le jeu World of Warcraft (fonctionnant sur AzerothCore)"youtube: "YOUR_VIDEO_ID_HERE" # Remplacer par l'ID de la vidéo YouTubesections:
  - title: "Aperçu"
    text: |
      > ⚠️ AVERTISSEMENT : <font color="yellow">RTRealm</font> est un projet privé créé uniquement à des fins d'apprentissage. Ce projet n'est pas affilié, approuvé ou connecté à <font color="blue">Blizzard Entertainment</font> de quelque manière que ce soit. World of Warcraft, WoW et tout le contenu connexe sont des marques commerciales et des propriétés de <font color="blue">Blizzard Entertainment Inc</font>. Ce serveur est maintenu uniquement à des fins éducatives et non commerciales dans un environnement académique.

      Mon serveur fonctionne sur <font color="red">AzerothCore</font> qui est un framework MMORPG open-source. Il est écrit en C++ et est basé sur le projet <font color="gray">TrinityCore</font>. <font color="red">AzerothCore</font> permet aux développeurs de créer et gérer des serveurs privés pour World of Warcraft, offrant une plateforme de personnalisation et d'expansion du jeu.

      Pour la base de données, j'ai choisi d'utiliser <font color="green">HeidiSQL</font> qui est une interface puissante et facile à utiliser pour gérer MySQL, MariaDB et d'autres systèmes de bases de données. Il fournit des outils pour la conception de bases de données, l'exécution de requêtes et la gestion des données.

      Les utilisateurs peuvent créer un compte sur le site web suivant : <a href="https://iodimetric-rolf-malapportioned.ngrok-free.dev/index.php"><font color="yellow">RTRealm</font></a>
    image: "/img/portfolio/srvimg.png"
    
  - title: "Sécurité des Comptes"
    text: |
  
       La base de données possède son propre utilisateur, qui est utilisé uniquement pour cette seule finalité, et dispose de permissions limitées pour éviter tout risque de <font color="lightblue">sécurité</font> potentiel.
       
       La base de données du serveur est <font color="lightblue">sécurisée</font> par le hachage des détails utilisateur tels que les <font color="cornflowerblue">mots de passe</font>, les clés de session et le <font color="orange">sel</font> en utilisant l'algorithme SRP6. Cela garantit que même si la base de données est compromise, les <font color="cornflowerblue">mots de passe</font> réels restent protégés. (Plus de détails dans les paragraphes ci-dessous)
       
       <br>
       <br>
       <br>
       <br>
       <br>
       <br>
       <br>

        Sur cette image, vous pouvez voir le formulaire où les utilisateurs pourront créer leur compte. Ils devront choisir un <font color="cornflowerblue">mot de passe</font> suffisamment long et complexe pour assurer un bon niveau de <font color="lightblue">sécurité</font> (8 caractères sont nécessaires).

        Le compte nouvellement créé sera stocké dans la base de données avec les détails suivants : le nom du compte, un <font color="orange">sel</font> (une chaîne aléatoire de caractères utilisée pour améliorer la <font color="lightblue">sécurité</font> du <font color="cornflowerblue">mot de passe</font>), le <font color="red">vérificateur</font> (une valeur dérivée du <font color="cornflowerblue">mot de passe</font> et du <font color="orange">sel</font> en utilisant l'algorithme SRP6), et d'autres informations pertinentes telles que l'email, la date d'inscription, la dernière IP, etc.

       <br>
       <br>
       <br>
       <br>
       <br>
       <br>
       <br>
       <br>
       <br>
       <br>
       <br>

       SRP‑6 est une version du protocole Secure Remote Password conçue pour permettre à un client et un serveur de s'authentifier mutuellement sans jamais envoyer le <font color="cornflowerblue">mot de passe</font> réel sur le réseau. Il fonctionne en faisant générer par les deux parties leurs propres valeurs privées et publiques, échanger uniquement les parties publiques sûres, et calculer indépendamment la même clé de session partagée en utilisant un mélange de mathématiques à grands nombres premiers et le <font color="red">vérificateur</font> de <font color="cornflowerblue">mot de passe</font> stocké.
       
       Parce que le <font color="cornflowerblue">mot de passe</font> lui-même n'est jamais transmis ou exposé, SRP‑6 protège contre l'écoute clandestine, les attaques par rejeu et les fuites de bases de données de serveur où un attaquant n'obtient que le <font color="red">vérificateur</font>. Le protocole se termine par les deux parties prouvant qu'elles ont dérivé la même clé, offrant une authentification mutuelle et une base <font color="lightblue">sécurisée</font> pour le reste de la session.

       <br>
       <br>
       <br>
       <br>
       <br>
       <br>
       <br>
       <br>
       <br>
       <br>
    

       
       
        
        Sur cette image, vous pouvez voir un exemple du <font color="cornflowerblue">mot de passe</font> salé et haché stocké dans la base de données, avec les autres détails du compte.

    image1: "/img/portfolio/admin-pw.png"
    image2: "/img/portfolio/register.png"
    image3: "/img/portfolio/srp6.png"
    image4: "/img/portfolio/accounts.png"

  - title: "Démonstration Vidéo"
    text: |
      Voici une démonstration vidéo du serveur en action, présentant le processus d'inscription et de connexion. Les interactions avec la base de données sont également mises en évidence pour illustrer comment les données utilisateur sont gérées de manière <font color="lightblue">sécurisée</font> lors d'une inscription.
    video: "/mov/contenu.mp4"
    
  - title: "Programme National Réseaux & Télécoms"
    text: |
      Ce projet démontre directement des connaissances dans plusieurs apprentissages critiques tels que :
      
      - AC34.01 Cyber - Mettre en œuvre des outils avancés de sécurisation d'une infrastructure du réseau
        
        Grâce au déploiement de <font color="red">RTRealm</font>, j'ai configuré des mécanismes d'authentification <font color="lightblue">sécurisés</font> et mis en œuvre des protocoles de <font color="lightblue">sécurité</font> en couches pour protéger l'infrastructure du serveur de jeu contre les accès non autorisés.
      
      - AC34.04 Cyber - Proposer une architecture sécurisée de système d'information pour une petite structure
        
        J'ai conçu et mis en œuvre une architecture <font color="lightblue">sécurisée</font> complète pour le serveur <font color="red">RTRealm</font>, incluant une séparation appropriée des préoccupations entre le serveur de jeu, la couche de base de données et le système d'inscription orienté utilisateur, garantissant l'intégrité et la confidentialité des données.
      
      - AC36.01 Cyber - Surveiller l'activité du système d'information
        
        La gestion des comptes et la journalisation des transactions ont été intégrées pour surveiller les inscriptions d'utilisateurs, les tentatives de connexion et les échecs d'authentification, fournissant des pistes d'audit pour la surveillance de la <font color="lightblue">sécurité</font> et la réponse aux incidents.
      
      - AC32.04 - Permettre aux collaborateurs de se connecter de manière sécurisée au système d'information de l'entreprise
        
        Le protocole d'authentification <font color="orange">SRP6</font> garantit que les utilisateurs peuvent se connecter en toute <font color="lightblue">sécurité</font> au serveur sans exposer leurs <font color="cornflowerblue">mots de passe</font> sur le réseau, mettant en œuvre les meilleures pratiques d'authentification à distance <font color="lightblue">sécurisée</font> dans des environnements réseau.
      
      Ces implémentations démontrent l'application pratique de la <font color="lightblue">sécurité</font> réseau, de l'administration système et des principes de <font color="lightblue">sécurité</font> de base de données essentiels au programme N&T.

    image: "/img/portfolio/AC_gameserv.png"
    image2 : "/img/portfolio/gameserv_lastac.png"
---
