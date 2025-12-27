<!-- ---
layout: project
lang: fr
title: "Créateur de Challenges CTF"
image: "/img/portfolio/TNS_challmaker.png" # Hero image
category: "Création de challenges pour un événement Capture the Flag organisé par l'université"
sections:
  - title: "Aperçu"
    text: | 
      Les étudiants en cybersécurité de dernière année du département Réseaux & Télécoms de l'université Marie & Louis Pasteur organisent chaque année un événement Capture the Flag appelé SecuRT.  

      Pour l'édition 2026, qui se tiendra en février, j'ai participé à la création de nombreux challenges pour l'événement. Les challenges sont conçus pour les étudiants de première année, avec pour objectif de leur faire découvrir les concepts de base de la cybersécurité tout en s'amusant à résoudre des défis.
    image: "/img/portfolio/securt_resize.png"
    
  - title: "Cryptanalyse"
    text: |
     Mon premier challenge est basé sur la célèbre scène du Seigneur des Anneaux : La Communauté de l'Anneau, lorsque la Communauté se trouve dans les Mines de la Moria face au Balrog. J'ai caché le flag dans le script et chiffré tout le texte en utilisant le chiffrement de Beaufort.

     Voici la partie intéressante : le chiffrement de Beaufort est connu comme un "cousin" de l'emblématique chiffrement de Vigenère. Bien que l'un utilise la soustraction de la clé et l'autre l'addition, la similitude entre les deux algorithmes rend difficile pour l'IA (à ce jour 🙃) de distinguer quelle méthode de chiffrement a été utilisée.

     De plus, le site populaire de chiffrement dCode peut piéger les joueurs du CTF, car il peut identifier incorrectement le chiffrement comme étant Vigenère.

    image1: "/img/portfolio/crypta.png"
    

  - title: "Cracking"
    text: |
      Mon deuxième challenge est un challenge de cracking où les participants doivent trouver le mot de passe correct pour récupérer le flag. Le mot de passe est stocké dans un programme C#, mais le programme doit d'abord être décompilé (les joueurs peuvent utiliser dnSpy ou ILSpy). Après décompilation, le joueur verra le mot de passe à entrer dans le programme pour obtenir le flag. Après avoir entré le mot de passe correct, le flag sera affiché.

      Le flag est XORé avec le simple caractère "*" pour qu'il ne puisse pas être lu directement après décompilation (gardant le challenge facile puisqu'il est destiné aux étudiants de 1ère année).

      L’opération XOR est fréquemment utilisée en cryptographie et en obfuscation. Elle consiste à retourner une valeur vraie uniquement lorsque les bits de l’opérande et de la clé sont différents, ce qui en fait une méthode simple et efficace pour l’obfuscation, notamment lorsqu’elle est combinée à une constante connue, comme un caractère unique.

      Comme le montre l'image à gauche, le mot de passe du programme est "4v_34ag_0xzwb3kbq0v". Entrer ce mot de passe révélera le flag final : "4n_34sy_0prot3cti0n" (qui peut également être obtenu en appliquant un chiffrement ROT18 au mot de passe du programme).
      
    

    image2: "/img/portfolio/program_ctf.png"
    image1: "/img/portfolio/decompil_cs.png"
    
  - title: "Programme National Réseaux & Télécoms"
    text: |
      Ce projet fait partie de notre SAÉ 6.Cyber.01 : Réagir face à une cyber-attaque
      
      Développer des challenges et héberger un serveur pour un événement CTF est un élément clé des compétences d'apprentissage suivantes.

      - AC.34.02Cyber \| Mettre en œuvre des outils avancés de sécurisation d'une infrastructure du réseau

      - AC.34.03Cyber \| Sécuriser les systèmes d'exploitation

      - AC.35.01Cyber \| Surveiller l'activité du système d'information

      - AC.35.03Cyber \| Réagir face à un incident de sécurité

      - AC.35.04Cyber \| Administrer les outils de surveillance du système d'information

      Grâce à ces compétences, j'ai acquis une expérience pratique dans :

      - Le déploiement d'un serveur pour héberger l'événement

      - La création de challenges de niveau débutant - intermédiaires mais intrigants pour les participants

      - La gestion et la maintenance d'un événement Capture The Flag

      - Assurer la sécurité et l'intégrité de l'infrastructure de l'événement
    image: "/img/portfolio/pn_ctf.png"
    large_image: "image"
---
 -->