<h1 align="center">
  <a href="https://github.com/git-bd/cissp">
    <img src="./../images/cissp.png" alt="Logo" width="125" height="135">
  </a>
</h1>

<div align="center">
  <p style="color:black;font-size:24px;">CISSP <strong>ISC2</strong></p>
  <p style="color:black;font-size:20px;"><strong>Chapter 3 : Security Architecture and Engineering</strong></p>
  <a href="https://github.com/git-bd/cissp/issues/new?assignees=&labels=bug&template=01_BUG_REPORT.md&title=bug%3A+">Report a Bug</a>
  ·
  <a href="https://github.com/git-bd/cissp/issues/new?assignees=&labels=enhancement&template=02_FEATURE_REQUEST.md&title=feat%3A+">Request a Feature</a>
  .
  <a href="https://github.com/git-bd/cissp/discussions">Ask a Question</a>
</div>

<br />
<div align="center">

✅**A savoir**  ℹ️**Information**  ‼️**Alerte** 🔗**Liens** ✏️**Illustration**  🔎**A approfondir** <br /><br />

</div>

## Sommaire
<br />


<details close="close">

</details>

<br />

# Research, Implement and Manage Engineering Processes Using Score
‼️ Avoid, Transfer, Mitigate, Accept

## ✅Design Principle 
USAF

## ✅ISO/IEC 19249
**Architectural principle**: Domaine Separation, Layering, N-Tiers, Encapsulation, Redundancy, Virtualization,
**Design Principle** : Least PRivilege, Attack Surface Minimization, Centralized Parameter Validation, Centralized Security Service, Preparing for Error and Exception Handling

## ✅Treat Modeling
Slide 63-65
L'identification des menaces constitue la première étape 
* **STRIDE**
* **DREAD**
* **PASTA**

## ✅Secure Defaults
## ✅Fail Securely
## ✅Separation of Duties
## ✅Keep it Simple
## ✅Trust but Verify
## ✅Zero Trust
NIST 800-207
* **Always Verify**
* **Use Least Privilege Access**
* **Assume Breach**

## ✅Privacy by Design
* **Proactive not Reactive, Preventive not Remedial**
* **Privacy as the Default**
* **Privacy Embedded into Design**
* **Full Functionality - Positive-Sum**
* **End-to-End Security**
* **Visibility and Transparency**
* **Respect for User Privacy**

## ✅Shared Responsability
* **CSP** : Cloud Service Provider

## ✅Defense in Depth
* **serie** : Multiple contrôle en série non en parallèle
* **Serie** : resseré (narrow) mais profond (deep)
* **Parallel** : large mai peu profond

* **Abstraction** : Elements similaire regoupé, utilisé pour des les types de données qui permet de simplifier la sécurité en permettant d'attribuer des contrôles.

# Understand the Fundamental Concept of security models
## ✅Primer on Common Modem Components
* **Finite State Machine** : 
* **A Lattice** : 

## ✅Information Flow Model

## ✅Noninterference Model

## ✅Bell-Lapdula Model
‼️Confidentialilté, labels

Il se base sur les classifications des informations: secret, top secret, etc

* **Simple Property** : un sujet ne peut avoir accès supérieur au sien mais inférieur oui.
* **Star Property** : ou `*-property`, il ne peut écrire dans un niveau inférieur au sien, évite que les informations sensibles se retrouvent sur des plateformes moins protégées.
* **Strong Star Property** : Un sujet doit avoir accès uniquement à son environnement 
* **Discretionary-Security Property** :

✏️ dessin de comparatif en fonction des classifications

## ✅Biba Integrity Model
‼️Intégrité

Il se focalise sur l'intgrité des données afin de propager des données fiable et garantie, système financier, santé et journalisme
* **Simple Integrity Axion** : un sujet ne peut lire des données que à son niveau d'intégrité ou supérieur, l'objectif est de ne pas contaminées des informations non fiables (journaliste vs torchon)
* **Star Integrity Axion** : Un sujet ne peut écrire de données qu'à un niveau inférieur car peu fiable, toujours pour ne pas modifier les données sur, vérifiée et intègre.

✏️ dessin de comparatif en fonction des classifications

## ✅Clark-Wilson Model
‼️Intégrité, segregation of Dutie

Il se base principalement sur les transactions, la segregation of Duty doit être fait par des personnes différentes. 

* **CDI** : `Constrained Data Item` donnée dont l'intégrité doit être préservées
* **UDI** : `UnConstrained Data Item` donnée dont l'intégrité n'est pas validée
* **TP** : `tranform Program` programme qui transforme une UDI en CDI
* **IVP** : `Integrity Verification Procedure` valide l'intégrité d'un CDI à un état donné

## ✅Brewer-Nash Model
‼️Confidentialité, conflit d'intérêt

Il permet le contrôle d'accès pour les conflits d'intérêts dans les organisations où les sujets peuvent travailler sur des informations sensibles et concurrentes.

## ✅Take-Grant Model
‼️
* **Take** : 
* **Grant** : 
* **Create** : 
* **Remove** : 

## ✅LIPNER Model
Combinaison de Bell-Lapadula et de BIBA

‼️Confidentialité & intégrité

Il repose sur les concepts d'accès obligatoire MAC et discretionnaire DAC 

# Select Controls Based Upon Systems security traitements
FISMA, GDPR, HIPAAn, SOC, PCI-DSS, NIST 800-37, ISO 27001, COBIT5, ISA624443, ISACAA

✏️ PDCA: Plan Do Check Act

# Understand Security capabilities of Information Systems
## ✅Memory Protection
Potential Weakness
  CPU
  ASLR
  Spectre and Meltdown

## ✅Secure Cryptoprocessor
Cryptoprpocessor, 
Trust Plateform Module TPM
Potential Weakness
Cryptographic Module 
HSM Hardware Security Module

# Assess and mitigate the vulnérabilities of Architectures, Designs and Solution elements
## ✅Client-Based Systems
## ✅Server-Based Systems
Hardening server
## ✅Database Systems
FDE, TDE, CLE
## ✅Cryptographic Systems
Algorithm and protocol weaknesses
  EC DBRG
  WEP
  DES
  POODLE
Implementation Weaknesses
  Heartbleed
Key management Vulnerabilities
  NIST SP 800-133

## ✅Industrial Control Systems
ICS, IAS/IEC62443, NERC, ERN-CIP CNPI 

## ✅Cloud-Based Systems 
NIST SP 800-145
Saas, IaaS, PaaS
REsponsabilities models

## ✅Distributed Systems 
## ✅Internet of Things
IoT
## ✅Microservices
## ✅Containerization
## ✅Serverless
## ✅Embedded Systems
## ✅High-Performance Computing Systems
## ✅Edge Computing Systems
## ✅Virtualized Systems
VM, HOST, OS, 

# Select and Determine Cryptographic solutions
CIA

## ✅Cryptography Basics
Plaintext
Clearttext
Ciphertext
Encryption
Decryption
Cryptographic algorithm
Key

## ✅Cryptographic Lifecycle
ECB, CBC, CFB

## ✅Cryptographic Methods
Symetric Encryption
  OR XOR, AND, NAND 
Stream cipher
Block Cipher
DES
3DES
AES
Rivest Ciphers
Asymetric Encrption
Diffie-Hellman-MerkleKey Exchange
RSA
El gamal
Elliptic Curve Cryptography
Quantum Cryptography
## ✅Public key Infrastructure
X.509 ITU
  version, serial, signature, etc 
PKI
  Identity, intermediate, Root
  ✏️ SChéma
DANE
## ✅Key Management Pratices
Secure Key Generation
Secure Key Storage and Use
  KEK, DEK, 
Separation of Duties, Dual Control and Split Knowledge
Timely Key Rotation and Key Change
Key Destruction
## ✅Digital Signature and Digital Certificates
✏️ Schéma de création et vérification des signatures digitale

## ✅Nonrepudiation
RFC3161
Blockchain and non repudiation
## ✅Integrity
Schema Tampering
HMAC process

# Understand Methods of Cryptanalytic attacks
* **Attaque analytique** : manipulation algébrique afin de réduire la complexité de l'algorythme
* **Attaque d'implémentation** :
* **Attaque Statistique** : souvent lié au matériel ou système d'exploitation 
## ✅Brute Force
* **rainbow table** : valeurs précalculées pour les opérations basées sur le hash
* **spécialisé** : machine permettant de réaliser le brute force
* **Salt** : le `sel cryptographique` est une valeur aléatoire qui est ajouté à la fin avant le hash du mot passe🔎
## ✅Ciphertext

## ✅Know plaintext

## ✅Chosen Plaintext Attack

## ✅Frequency Analysis

## ✅Chosen Ciphertext

## ✅Implementation Attacks

## ✅Side-Channel Attacks
CPU Attack
Memory attack
TEMPEST

## ✅Fault injection

## ✅Timing Attack
* **Anniversary Attack** ou **Collision** ou **hashage inversé**: faille trouver par résultat identique

## ✅Man-in-the-Middle
* **Man-in-the-Middle** :
* **Meet-in-the-Middle** : vaincre les algorithmes de chiffrement qui utilisent 2 tours de chiffrement (2DES)
> ℹ️ Aujourd'hui il est minimum recommandé 3 voir plus

## ✅Pass the Hash

## ✅Kerberos Exploitation

## ✅Ransomware

# Apply Security Principle to Site and Facility Design
CIA
# Design site and facility security controls
## ✅Wiring Closets/Intermediate Distribution Facilities
## ✅Server Room/Data Centers
ASHRAE
ANSI/BICSI
EIA/TIA
EN 50600
ISO 20134
## ✅Media Storage Facilities

## ✅Evidence Storage
## ✅Restricted and Work Area Security
Least privilege
separation of Dutie
Defense in Depth
Compliance Obligation SCIF 
## ✅Utilities and Heating, Ventilation and Air Conditionning
HVAC
UPS: Load, Capacity Filtering and Reliability
## ✅Environnement Issues 
Earthquake, flood, vlocanoes, etc

## ✅Fire Prevention, Detection and Suppression
NFPA 75
Sprinkler
Class of fuel: A, B , C, D, E, F or K
# Summary
## ✅Question / Remarks






# 🚀 Module : Security Architecture and Engineering

**Formatrice / Formateur :** [Votre Nom]** |
Durée estimée :** ⏳ 45 min**
Niveau :** ⭐⭐ Intermédiaire

---

## ✅🎯 Objectifs de la leçon
À la fin de ce module, vous serez capable de :
1.  Comprendre le fonctionnement global de **[Sujet]**.
2.  Savoir implémenter la solution à l'aide d'un script dédié.
3.  Identifier et contourner les erreurs les plus communes.

---

## ✅ 1. Secure Design principles

## ✅ 2. Concept of security models

## ✅ 3. System security traitements

## ✅ 4. Security capabilities

## ✅ 5. Assess and mitigate the vulnérabilités

## ✅ 6. Cryptographic solutions

## ✅ 7. Cryptanalytic attacks

## ✅ 8. Design site and facility security controls

