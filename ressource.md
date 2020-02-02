# Outils pour blind XSS :

- https://xsshunter.com/
- https://beeceptor.com/
- https://github.com/ssl/ezXSS
- https://github.com/mazen160/xless

# Wordlists :

- https://github.com/danielmiessler/SecLists
- https://github.com/tarraschk/richelieu (française)

# Reverse shell cheat-sheet :

- http://pentestmonkey.net/cheat-sheet/shells/reverse-shell-cheat-sheet
- https://www.asafety.fr/reverse-shell-one-liner-cheat-sheet/

 

# PrivEsc :

- https://gtfobins.github.io/
- https://lolbas-project.github.io/
- https://blog.g0tmi1k.com/2011/08/basic-linux-privilege-escalation/



# Blogs/Ressources :

- https://www.securityidiots.com/
- https://brutelogic.com.br/blog/
- https://github.com/s0md3v/AwesomeXSS
- https://addons.mozilla.org/fr/firefox/addon/new-hackbar/


# Phishing :

- SeToolkit : Outil spécialisé dans le Social Engineering.
- Gophish : Framework de phishing spécialisé dans les campagnes de phishing
- HaveIBeenPwned

# Payload
-  Phantom Evasion
-  Metasploit


# Base de données d'informations :

- LeakProbe.net : Site qui se veut “Easy to use” et qui permet de chercher dans une base de donnée de plus de 2 milliards de référence ses identifiant, mot de passe, pseudo, etc.

- databases.today : Site de diffusion de base donnée. Il se veut libre et permet de profiter de plusieurs base de données leaké gratuitement.

- leak-lookup.com : Comme LeakProbe.net mais avec une plus grande base de donnée (13 milliards) mais payante

# Hardware "hack"

- Wifi pineapple : The world's best rogue access point and **WiFi** pentest platform. The **WiFi Pineapple** lets pentesters perform targeted man-in-the-middle attacks, advanced reconnaissance, credential harvesting, open source intelligence gathering and more – all from a clean, intuitive web interface.
- Rubber Ducky USB: install a backdoor, exfiltrate documents, steal passwords or any number of pentest tasks.
- usb killer: Kill PC


# Responder/MultiRelay
LLMNR/NBT-NS/mDNS Poisoner and NTLMv1/2 Relay. [Github](https://github.com/lgandx/Responder)

# Mimikatz - Benjamin DELPY


Celui-ci est largement utilisé par les pentesters actuellement. L’objectif principal de l’outil était la manipulation des clefs privées et certificats dans l’objectif de pouvoir les rejouer (exemple : Pass-The-Hash).

L’outil permet dans sa version actuelle un grand nombres d’opérations comme la manipulation des identifiants stockées en mémoire, les tickets kerberos, etc....

# Blood Hound 

BloodHound est un outil graphique permettant de mettre en avant les connexions qui peuvent exister au sein d’un domaine Active Directory.

L’outil est constitué de 2 parties :

- La partie Ingestors, qui va récolter les données
- La partie GUI qui va permettre l’upload et l’exploitation des données


<?xml version="1.0" encoding="UTF-8"?>

Rfkill

Gestionnaire d’équipement sans fil

Permet de lister, activer/désactiver les équipements

Gère les filtres de cartes (logiciel et hardware)

Mode monitor nécessite les deux débloqués



Aircrack-ng

Airmon-ng: permet de switch entre deux des 8 modes principaux

Airodump-ng: permet de visualiser et capturer les trames

Aireplay-ng: permet d’injecter des paquets dans un réseau par exemple pour générer du flux ou dés authentifier un client


# WIFI


Rfkill : Gestionnaire d’équipement sans fil

- Permet de lister, activer/désactiver les équipements
- Gère les filtres de cartes (logiciel et hardware)
- Mode monitor nécessite les deux débloqués
- 
Aircrack-ng
 - Airmon-ng: permet de switch entre deux des 8 modes principaux
 - Airodump-ng: permet de visualiser et capturer les trames
-Aireplay-ng: permet d’injecter des paquets dans un réseau par exemple pour générer du flux ou dés authentifier un client

----
  
- iwconfig => pour voir la présence d'une carte wifi
- aircrack-ng => passer la carte en mode monitor
- aircrack-ng check kill => vérifier les process qui peuvent interférer avec le mode monitor
- armon-ng start wlan0 => pour lancer l'analyse du réseau
- airmong-ng -a [nom carte wifi] => scan le réseau et montre les AP
- aireplay-ng --deauth 0 => désauthentifie à l'infini
- aireplay-ng —deauth -d [liste d'adresse mac]

 **Airgeddon**
Permet d’automatiser les attaques

 **Wifite**
Permet d’automatiser les attaques