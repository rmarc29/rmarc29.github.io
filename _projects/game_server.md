---
layout: project
lang: en
title: "Private Game Server"
image: "/img/portfolio/HSQL-Acore.png" # Hero image
category: "An entire private server structure for the game World of Warcraft (running on AzerothCore)"
sections:
  - title: "Overview"
    text: |
      > ⚠️ DISCLAIMER : <font color="yellow">RTRealm</font> is a private educational project created for learning purposes only. This project is not affiliated with, endorsed by, or connected to <font color="blue">Blizzard Entertainment</font> in any way. World of Warcraft, WoW, and all related content are trademarks and properties of <font color="blue">Blizzard Entertainment Inc</font>. This server is maintained solely for educational and non-commercial use within an academic environment.

      My server is running on <font color="red">AzerothCore</font> which is an open-source MMORPG framework. It is written in C++ and is based on the <font color="gray">TrinityCore</font> project. <font color="red">AzerothCore</font> allows developers to create and manage private servers for World of Warcraft, providing a platform for customization and expansion of the game.

      For the database i chose to use <font color="green">HeidiSQL</font> which is a powerful and easy-to-use interface for managing MySQL, MariaDB, and other database systems. It provides tools for database design, query execution, and data management.

      Users can create an account on the following website : <a href="https://iodimetric-rolf-malapportioned.ngrok-free.dev/index.php"><font color="yellow">RTRealm</font></a>
    image: "/img/portfolio/srvimg.png"
    
  - title: "Account Security"
    text: |
  
       The database has it's own user, that is used only for this sole purpose, and has limited permissions to avoid any potential <font color="lightblue">security</font> risks.
       
       The server's database is secured by hashing user details such as <font color="cornflowerblue">passwords</font>, session key and <font color="orange">salt</font> using the SRP6 algorithm. This ensures that even if the database is compromised, the actual <font color="cornflowerblue">passwords</font> remain protected. (More details in paragraphs below)
       
       <br>
       <br>
       <br>
       <br>
       <br>
       <br>
       <br>

        Here, users will be able to create their account. They will have to chose a <font color="cornflowerblue">password</font> that is long and complex enough to ensure a good level of <font color="lightblue">security</font> (8 characters are needed).

        The newly created account will be stored in the database with the following details : the account name, a <font color="orange">salt</font> (a random string of characters that is used to enhance <font color="cornflowerblue">password</font> <font color="lightblue">security</font>), the <font color="red">verifier</font> (a value derived from the <font color="cornflowerblue">password</font> and <font color="orange">salt</font> using the SRP6 algorithm), and other relevant information such as email, joindate, last_ip, etc.

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

       SRP‑6 is a version of the Secure Remote Password protocol designed to let a client and server authenticate each other without ever sending the actual <font color="cornflowerblue">password</font> across the network. It works by having both sides generate their own private and public values, exchange only the safe public parts, and independently compute the same shared session key using a mix of large‑prime math and the stored <font color="cornflowerblue">password</font> <font color="red">verifier</font>. 
       
       Because the <font color="cornflowerblue">password</font> itself is never transmitted or exposed, SRP‑6 protects against eavesdropping, replay attacks, and server‑database leaks where an attacker only obtains the <font color="red">verifier</font>. The protocol ends with both sides proving they derived the same key, giving you mutual authentication and a <font color="lightblue">secure</font> foundation for the rest of the session.

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
       <br>
       <br>
       <br>
       <br>
       
        
        Here you can see an example of the salted and hashed <font color="cornflowerblue">password</font> stored in the database, along with the other account details.

    image1: "/img/portfolio/admin-pw.png"
    image2: "/img/portfolio/register.png"
    image3: "/img/portfolio/srp6.png"
    image4: "/img/portfolio/accounts.png"

  - title: "Video Demonstration"
    text: |
      Here is a video demonstration of the server in action, showcasing the register and login process. The database interactions are also highlighted to illustrate how user data is <font color="lightblue">securely</font> managed when a registration occurs.
    youtube: "3-5Nw5YSHaI"
    
  - title: "French Networks & Telecoms National Program"
    text: |
      This project directly demonstrates knowledge in several critical learning outcomes such as:
      
      - AC34.01 Cyber - Implementing Advanced Network Infrastructure Security Tools
        
        Through the deployment of <font color="yellow">RTRealm</font>, I configured <font color="lightblue">secure</font> authentication mechanisms and implemented layered <font color="lightblue">security</font> protocols to protect the game server infrastructure from unauthorized access.
      
      - AC34.04 Cyber - Proposing Secure Information System Architecture for Small Structures
        
        I designed and implemented a complete <font color="lightblue">secure</font> architecture for the <font color="yellow">RTRealm</font> server, including proper separation of concerns between the game server, database layer, and user-facing registration system, ensuring data integrity and confidentiality.
      
      - AC36.01 Cyber - Monitoring System Activity
        
        Account management and transaction logging were integrated to monitor user registrations, login attempts, and authentication failures, providing audit trails for <font color="lightblue">security</font> monitoring and incident response.
      
      - AC32.04 - Enabling Secure Employee/User Connection to Enterprise Information Systems
        
        The <font color="orange">SRP6</font> authentication protocol ensures that users can <font color="lightblue">securely</font> connect to the server without exposing their <font color="cornflowerblue">passwords</font> over the network, implementing best practices for <font color="lightblue">secure</font> remote authentication in networked environments.
      
      These implementations showcase practical application of network <font color="lightblue">security</font>, system administration, and database <font color="lightblue">security</font> principles essential to the N&T curriculum.

    image: "/img/portfolio/AC_gameserv.png"
    image2 : "/img/portfolio/gameserv_lastac.png"
---
