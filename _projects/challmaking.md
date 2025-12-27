<!-- ---
layout: project
lang: en
title: "CTF Challmaker"
image: "/img/portfolio/TNS_challmaker.png" # Hero image
category: "Creating challenges for a Capture the Flag event organized by the university"
sections:
  - title: "Overview"
    text: | 
      The senior cybersecurity students from the Networks & Telecoms departement of the university of Marie & Louis Pasteur are organising each year a Capture the Flag event called SecuRT.  

      For the 2026 edition, which will be held in February, I took part in the creation of many challenges for the event. The challenges are designed for first-year students, with the goal of introducing them to basic concepts of cybersecurity whilst  focusing on having fun solving challenges.
    image: "/img/portfolio/securt_resize.png"
    
  - title: "Cryptanalysis"
    text: |
     My first challenge is based on the well-known scene from The Lord of the Rings: The Fellowship of the Ring, when the Fellowship is in the Mines of Moria facing the Balrog. I hid the flag within the script and encrypted the entire text using the Beaufort cipher.

     This is the interesting part: the Beaufort cipher is known as a "sibling" of the iconic Vigenère cipher. While one uses subtraction of the key and the other uses addition, the similarity between the two algorithms makes it difficult for AI (as of today 🙃) to distinguish which encryption method was used.

     Additionally, the popular cipher website dCode can lead CTF players into a trap, as it may incorrectly identify the cipher as Vigenère.

    image1: "/img/portfolio/crypta.png"
    

  - title: "Cracking"
    text: |
      My second challenge is a cracking challenge where participants have to find the correct password to retrieve the flag. The password is stored in a C# program, but the program needs to be decompiled first. (The players can use dnSpy or ILSpy). After decompiling, the player will see the password that needs to be entered in the program to get the flag. After entering the correct password in the program, the flag will be displayed.

      The flag is XORed with the simple character "*" so that it can't be directly read after decompiling (keeping the challenge easy since it is for 1st year students).

      XOR is a common operation used in cryptography and obfuscation, and it operates by returning true only when bits differ between the operand and key, making it ideal for simple obfuscation when combined with a known constant like a single character.

      As shown in the image on the left, the password for the program is "4v_34ag_0xzwb3kbq0v". Inputing this password will reveal the final flag : "4n_34sy_0prot3cti0n" (which can at the same time be obtained by applying a ROT18 cipher to the program password).
      
    

    image2: "/img/portfolio/program_ctf.png"
    image1: "/img/portfolio/decompil_cs.png"
    
  - title: "French Networks & Telecoms National Program"
    text: |
      This project is part of our SAÉ 6.Cyber.01 : Reacting to a cybersecurity incident
      
      Developing challenges and hosting a server for a CTF event is a key component of these following learning outcomes.

      - AC.34.02Cyber \| Implement advanced tools for securing a network infrastructure

      - AC.34.03Cyber \| Secure operating systems

      - AC.35.01Cyber \| Monitor information system activity

      - AC.35.03Cyber \| Respond to a security incident

      - AC.35.04Cyber \| Administer information system monitoring tools

      Through these learning outcomes, I gained practical experience in:

      - Deploying a server to host the event

      - Creating intriguing beginner and intermediate challenges for participants

      - Managing and maintaining a Capture The Flag event

      - Ensuring the security and integrity of the event infrastructure
    image: "/img/portfolio/pn_ctf.png"
    large_image: "image"
---
 -->