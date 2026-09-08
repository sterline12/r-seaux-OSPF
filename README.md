# Projet Cisco Packet Tracer


## 📌 Description
Ce projet a été réalisé avec Cisco Packet Tracer dans le cadre de monapprentissage des réseaux informatiques.

Réalisation d'un réseau de communication via le protocole d’OSPF avec d’autres réseaux. 

Un protocole qui nous permet de régir le trafic au sein d’un système autonome (AS) de grande envergure (celui d’une entreprise par 
exemple). Qui peut être lui-même être constitué de plusieurs zones (areas) distinctes interconnectées par des routeurs.

Réaliser le routage de sorte que le réseau forme un espace totalement connexe, c-à-d tout terminal rattaché à tout routeur peut être joint par tout autre terminal du même réseau. De plus, ce réseau, qui est vu comme un AS, possède un Intranet et il est connecté au reste d’INTERNET, ainsi qu’à un site particulier via une liaison dédié. 
##khlkhdlkfldkfd;kf
## 🎯 Objectifs

* Concevoir une topologie réseau
* Configurer les équipements réseau
* Assurer la communication entre les différents appareils
* Tester la connectivité du réseau

## 🖥️ Outils utilisés

* Cisco Packet Tracer

## 📁 Contenu du projet

Le fichier `.pkt` contient la topologie et les configurations du réseau.

Configuration 
• Il y aura 3 sites dont seul le 3ième peut posséder un seul routeur 
• Le 1er site aura  n1=3+(DSG(0) modulo 2)  routeurs (c’est-à-dire 3 ou 4) 
• Le 2nd site aura n2=7-n1 routeurs
• Le préfixe (A.B.0.0) du site 1 sera : A=128+(DSG(1) module 64), B= DSG(2) 
• Le préfixe (A.B.0.0) du site 2 sera : A=128+(DSG(3) module 64), B= DSG(4) 
• Le préfixe (A.B.0.0) du site 3 sera : A=128+(DSG(5) module 64), B= DSG(6) 
• Le 1er site sera « area 1>, le 2nd site sera « area 2 » 
o Si le 3ieme site possède plusieurs routeurs, il sera « area 3 » 
• Rappel : Il y aura au moins un routeur dans chaque site qui sera sur le « area 0 » 

Remarque :   L(SG)=31     DSG (0) = DSG (31) =78     et      DSG (2) = DSG (33) =80 

Adressage 
D’après les consignes du projet selon les besoins : 
 
A. Résultats du nombre de routeurs pour chaque area : 
 Pour l’area 1  
n1=3 + (DSG (0) modulo 2) routeurs         
DSG (0) = 72          DSG (0) % 2 =0       Alors n1=3+0 = 3 routeurs 

 Pour l’area 2  
n2=7- n1 = 7-3 = 4 routeurs 

 L’area 3 
On a décidé de choisir trois routeurs donc n3 = 3 routeurs 

B. Adressage pour chaque site 
 Pour l’area 1     Adresse réseaux : 142.80.0.0  
 Pour l’area 2      Adresse réseaux : 129.68.0.0  
 Pour l’area3      Adresse réseau : 143.66.0.0 
 Remarque Il s’agit d’adresses de classe B car leurs 1 ers octets sont compris [128-191]

Résultats à présenter 

Présenter le réseau et illustrer son bon fonctionnement à travers, au moins, les éléments suivants  
    • La topologie du réseau 
    • La connexité entre deux terminaux sur deux sites différents dans deux Areas différents par au moins un exemple.  
    • Montrer la connexité entre l'AS et le site 192.33.182.0/24., ainsi que un site Internet (hors l’AS) hors  192.33.182.0/24.  
     • La robustesse de cette connexion  versus des pannes de liaison doit être montrée.
      
La configuration formant un réseau maillé, un moyen de montrer cette robustesse consiste à montrer le basculement vers un 2nd chemin, 
suite à la désactivation  d’une interface (utilement choisie) situant sur le 1er chemin. 
    • Montrer, pour au moins  deux routeurs, autres que Rd, Rs et Ri, les informations détenues par le routeur que vous jugez pertinentes.
      Une attention particulière sera accordée.
    • Le bon fonctionnement de votre NAT par au moins deux exemples de communication.

## 🚀 Utilisation

1. Télécharger le fichier `.pkt`
2. Ouvrir Cisco Packet Tracer
3. Ouvrir le fichier du projet
4. Tester la communication entre les différents équipements

## 👤 Auteur

Sterline Point du jour




    
         
