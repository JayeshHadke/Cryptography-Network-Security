# Cryptography-Network-Security

## INDEX
**1. Introduction to Cryptography**

**2. Abstract Algebra and Number Theory**

**3. Block Cipher**

**4. Public Key Cryptography**

**5. Cryptographic Hash Function and Digital Signature**

**6. Security Practices adn System Security**

**7. Email, IP and web security**



## 1. Introduction to Crpytograhy

**Why do we need Network Security??**

In our daily life, we are using internet in uncountable times and for that, data has to receive and send from our devices and once it has entered into the Internet we don't know how it will act. And there are many peoples who can steal your data from internet and can send data to us thorugh internet. To protect your data, devices, organization, Infrastructure from this type of attacks, We need some security function which will help to protect our data.
At this time, Network Security plays a vital role to secure us and Cryptography is used to hide our information in human unreadable formate so that ,if in case data has stolen then they cannot understand it and use it by some encryption techniques. 

**Defination**

The protection afforeded to an automated information system in ordered to attain the application objectives of preserving the INTEGRITY, AVAILABILITY and CONFIDENTIALITY of information system.

**CIA Tried**
![CIA Tried](https://github.com/JayeshHadke/Cryptography-Network-Security/blob/master/images/Screenshot%202022-04-19%20194857.png)

CIA is nothing but, 
  - Confidentiality
      - shared data should be understanable by sender and receiver only
      - deals with unauthorized access
      - avoid data discloser 
     
  - Integrity
      - SEND = RECEIVER
      - no modification of data should done between a data transfer or data share
      - if in case data is accessed by unauthorized person then the data should be in such a way that data is ununderstanable to that person
      
  - Availability 
      - timingly and realiable connection
      - deals with DOS (denial of services)

**What is Threat and Attack?**
  
  *Threat*, A potential for voliation of security which exists when there is a circumstances, capability ,action or event that could breach security and cause harm. That is, a threat is a possible danger that might exploit a valnerability.
  
  *Attack*, An assault on system that derives from an intelligent threat, that is an intelligent act that is a deliberate attempt to evade security services and violate the security policy of a system.
  
  
### OSI MODEL (OPEN SYSTEM INTERCONNECTION MODEL) ARCHITECTURE

OSI Architecture has main three sectors,
- Security Attack
    - Action that compromises the security
- Security Mechanism
    - Detect, Prevent, or Recover from a security attack
- Security Service
    - Enhance the security encounter security attack and provide the services

**Security Attack**

Types are :

- Passive Attack
    - only data observation
    - no data Modification
- Active Attack
    - modification of data 
    - false data stream can be shared
 
 *Passive Attack*
 - Release of message contents
    - attacker can see a data transfer between sender and receiver without knowing them
 - Traffic Analysis (when data is send in encrypted formate)
    - observe a pattern of data flow and other details
 
 *Active Attack*
 - Masquerade
    - acting as a original entity but actually it is hacker, who is pretenting to be a authorize user
 - Replay
    - sending same messages so that end user may misdirect and do what hacker wants
 - Modification of Messages
    - hacker act as a intermediate between sender and receiver so that they can modify, replay or delay data
 - Denial of Service (DoS)
    - hacker force a server in such a way that, server doesnot respond to user or make a system in which user doesnot allowed to enter

***Security Mechanism***

Security Mechanism is a set of framework / protocol to follow to ensure a trusted network connectivity and to implement secuirty policies.

Types :

- Specific Security Mechanism
    - security rules design for OSI model
- Prevasive Security Mechanism
    - security rules design for all types of models (a standard rules of every Security Mechanism must have)


*Specific Security Mechanism*
- Encipherment
    - hiding a plaintext into unreadable formate so that only sender and receiver can read that
- Digital Signature
    - a peace of code is send into a packets to authenticate a trusted sender / receiver and helps in data integrity
- Access Control
    - rights to resources are derived for specific users
- Data Integrity
    - no data modification during data transmission in internet
- Authentication Exchange
    - continous authentication of pear routers to ensure other than pear router no one should transmite data from a router 
- Traffic Padding
    - making a dummy data stream line to confuse a enternal entities and the stream doesnot affects to original data stream in communication
- Routing Control
    - manually change a transmission route in internet so that data should not flow from any unknown nodes
- Notarization
    - deloy any trusted third party to secure connection in internet
 
*Pervasive Security Mechanism*
- Trusted Functionality
    - authorize action in resources using some criteria / rules
- Security Lables
    - identifing an action result is valid or invalid
- Event Detection
    - each action are captured and each action is identified as either Normal event or Suspesious event
- Security Audit Trail
    - identifing actor of each action by looking at system log files
- Security Recovery
    - if in case, any attack has been take place, then a machanism to recover it to it's original / previous state

**Security Services**

The processing or communication service that is provided by a system to give a specific kind of protection to system resources; security services implements security policies and are implemented by security mechanism

Types : 

- Authentication
    - proves Identity of user
        - Peer Entity Authentication (authentication of each peer router so that no external or dummy router can send data from it)
        - Data Entity Authentication (authentication of each data onces it received at receiver side)
- Access Control
    - rights for resources are derived for specific custormers
- Data Confidentiality
    - only sender and receiver should understand a transmitted data
- Data Integrity
    - no modification should done in between data transmission
- Non-Repudation
    - protecting against denial of any enetity in communication after data transmitted and received


### Network Security Model

![Network Security Model](https://github.com/JayeshHadke/Cryptography-Network-Security/blob/master/images/Screenshot%202022-04-21%20003555.png)

In this model we are going to study, How a secured network works to prevent any type of vulnerable attack.

At both the ends of Transmission, data needs to be transform in a such a way that it should not be understanble to any one rather than receiver. And original data / transformed data tranformation is takes place with the help of Security Info to form Secured Data / Original Data. 

We used a word called Transform, because we have many types of algorithm to form cipher data / secured data .

We can see Opponent is mentioned and can access your data when data trasmission takes place thought transmission medium. Opponents are the those who wanted to steal your information and they can only get this during a data transmission.

Onces a transformed data is ready which is called as Secured Data, data transmission takes place to send a data. As you can see there is a Trusted Third Party is mentioned in the diagram, It is use to make a Trusted / Secured Connection between two ends (Specially Use for Banking Perpose) and gives SSL(Secure Sockets Layer) certificate to the end users, about this we will discuss in last module.


**Four Major Task Of Security Model**

- Design an Algorithm
- Generate the Secret Key
- Develop a methods for Distribution of Security Info (Specially in Symmetric Encryption / Cryptography) and Sharing of Information
- Specify a protocol


### Cryptography

The art or science encomprassing the principles and methods of transforming an intelligible message into one that is uninelligible and then retransformation and then retransformating the message back to its original form.

![Cryptography](https://github.com/JayeshHadke/Cryptography-Network-Security/blob/master/images/Screenshot%202022-04-21%20011710.png)

Types : 

- Symmetric Cryptography 
    - ![Symmetric Cryptography](https://github.com/JayeshHadke/Cryptography-Network-Security/blob/master/images/Screenshot%202022-04-21%20012251.png)
    - same key is used for encryption and decryption 
    - also called as private key cryptography
- Asymmetric Cryptography
    - ![Asymmetric Cryptography](https://github.com/JayeshHadke/Cryptography-Network-Security/blob/master/images/Screenshot%202022-04-21%20012503.png)
    - different kay is used for encryption and decryption 
    - also called as public key cryptography

Main Purpose of Cryptography
- Unconditionally Secured
    - alogrithm used for encryption is in such a way that, it should not be decrypted without a key 
    - key must be strong key so that no one can even crack it
- Compitationally Secured
    - time requried to break a cipher data / key must be more than the duration of transmitted data is valid in real world.
    - a cost requied to break a cipher text should be more than cost required to encrypt the data
 
 *Asymmetric Cryptography*
 
 - To transmitte a data, receiver should have two keys a Public key, and a Private key and sender should make cipher text from plain text using receivers public key. 
 - Sharing of public key takes place with the help of any Trusted Thired Party Services.
 - A cipher text is encrypted using Receivers Public key and can decrypte using receivers private key.
 
 > Public key which is create by receiver for transformation in sender side has assocication with receivers Private key. 
 
### Classical Encryption Techniques

A simple and basic encryption techniques used to transform a data in Cipher Text. Now a days, we are not using this type of encryption techniques Because these are the basic and oldest encryption techniques which is easy to decrypt using Cryptoanalysis or Brute Force Techniques.


Types : 

- Substitution Techniques
    - in this technique, each letter is replaced by any another sysmbol or number
    - same data should not reapeat
- Transformation Techniques
    - sort of permutation is used to make a different cipher text with same text but with arrangements


**Substitution Techniques**

Types : 

- Caesor Cipher
- Monoalphabetic Cipher
- PlayFair Cipher
- Hill Cipher
- Polyalphabetic Cipher
- One Time Pad

**Transposition Technique**

Types :

- Rail Fence 
- Row Column Transposition



*Caesor Cipher*

- Each letters are replaced with Numbers.
- ![Each Letter Maps to a Number](https://github.com/JayeshHadke/Cryptography-Network-Security/blob/master/images/Screenshot%202022-04-21%20192735.png)


C = cipher text letter

p = plain text letter

k = 3 (for ceasor cipher)

E(a,b) = a + b

D(a,b) = a - b


Algorithm for Encryption ,

**C = E ( p , k ) mod 26**

**C = ( p + k ) mod 26**

> Ceasor Cipher is also called as *Shift Cipher* with k as 3, if k value is other than 3 then algorithm called as Shift Cipher.

Algorithm for Decryption ,

***p = D(C,k) mod 26***             for C >= 3

***p = 26 - ( D(C,k) mod 26 )***      for C < 3 && C >= 0

[MORE EXAMPLES](https://www.javatpoint.com/caesar-cipher-technique)


*Monoalphabetic Cipher*

- mapping a plaintext letters with Language letters to form a Cipher Text using permutation.
- onces any plain text letter maps to language letter, then mapped letter should not use for any another plaintext 

[MORE EXAMPLE](https://www.101computing.net/mono-alphabetic-substitution-cipher/)


*Play Fair Cipher*

- manuall encryption and decryption technique
- firstly invested diagrammatic cipher technique

Algorithm
- 5 X 5 matrix is used for both encryption and decryption and ciphering is done with the help of key
- while creating a matrix, we to make it in such away that, Intially we must put the key for encryption / decryption in matrix with no repeating letters and after filling all the letters of key, start filling all alphabets from A to Z but no letter should repeat in matrix. If any letters is already there in matrix, then no need to place it again in matrix. And I and J place in same block always, Because in English we have 26 alpahbets and for matrix we have just 25 blocks in it, so we usally place I and J together in a same same block. Ex. Key is JAYESH then matrix is ![Matrix](https://github.com/JayeshHadke/Cryptography-Network-Security/blob/master/images/Screenshot%202022-04-22%20071327.png)
- we have to make pair of two letters pairs of plaintext 
    - if in a pair, both the letters are same then we should add filler element in between (filler element - X). Ex, if PlainText is HELLO then pairs must be HE LX LO
    - if a plaintext consists of odd numbers of letters then, at the end of the plaintext we must add filler element to make pairs of two letters. Ex, if Plaintext is WATCH then pairs must be WA TC HX 
- Encryption 
    - Rules
        - if both the letters are in same row, then cipher text letters for respectives letters are the next right letters in same row of matrix. Ex, If A and C is in a pair and in matrix both are in same row then respective Cipher text B and D  
          ![Rule-1](https://github.com/JayeshHadke/Cryptography-Network-Security/blob/master/images/Screenshot%202022-04-22%20065512.png)
        - if both the letters are in same column, then cipher text letters for respective letters are the below next letters in same column of matrix. Ex, If A and C is in a pair and in matrix both are in same column then respective Cipher text A and L  
          ![Rule-2](https://github.com/JayeshHadke/Cryptography-Network-Security/blob/master/images/Screenshot%202022-04-22%20070112.png)
        - if both the letters forms a rectangle, then cipher text for respective letters are the opposite letters in ractangle of matrix. Ex, If O and W is in a pair and forms a rectangle in matrix then respective Cipher text is opposite letter in matrix which is M and Y  
          ![Rule-3](https://github.com/JayeshHadke/Cryptography-Network-Security/blob/master/images/Screenshot%202022-04-22%20070556.png)

*Hill Cipher*

- encryption technique uses Matrix Multiplication to form ciphertext


Encryption Algorithm
- firstly, we make a pair of three letters of plaintext in a row. Ex, [ p1, p2, p3 ]
- make a square matrix of key text 
- then multipy both of the matrix and do mod 26 
- Equation for encryption
  ![Equation](https://github.com/JayeshHadke/Cryptography-Network-Security/blob/master/images/Screenshot%202022-04-22%20100644.png)
- Simplified Form
  ![Simplified Encryption](https://github.com/JayeshHadke/Cryptography-Network-Security/blob/master/images/Screenshot%202022-04-22%20100642.png)
  
  Decryption Algorithm
  - Equation ![Equation](https://github.com/JayeshHadke/Cryptography-Network-Security/blob/master/images/Screenshot%202022-04-22%20100645.png)
  - K^-1 [Refer More](https://byjus.com/maths/inverse-matrix/) 
