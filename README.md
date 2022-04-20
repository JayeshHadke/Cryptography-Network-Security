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
    - security rules design for specific layers
- Prevasive Security Mechanism
    - security rules design for all types of layers (a standard rules of every Security Mechanism must have)


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
