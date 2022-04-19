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
      - if in case data is accessed by unauthorized person then the data should be in such a way so that data is ununderstanable to that person
      
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
 
