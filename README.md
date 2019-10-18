# web-raspberry
serveur web avec raspberry


Près-requis:
 -raspbian à jour
 -connexion ssh en tant que root(super-utilisateur)
 FileZilla sur le pc maître (windows ou mac)
 blocnote(windows) ou Visual Studio Code(mac)
 
 Installation:
 
 -Avoir tout les droits (root) => sudo nano /etc/ssh/sshd_config
 allez à la ligne  "PermitRootLogin" et mettez "PermitRootLogin yes"
 Puis control+x
 Ensuite sudo passwd root , choisir votre mot de passe et confirmer.
 Enfin "sudo reboot"
 
 En root:
 -sudo apt-get update
 -sudo apt-get upgrade  
 -sudo apt-get install apache2
 -sudo apt-get install php
 
Droit d'ecriture, lecture et execution sur nos fichiers html,php,py: sudo visudo
aller à la fin du fichier et taper:
www-data  ALL=(ALL:ALL) NOPASSWD: ALL

et enregistrer par control+x
 
et enfin : sudo reboot

Ouvrer votre navigateur (google ou modzila)..... et taper : http://ipdevotreraspberry
Vous tomberez sur la page de présentation d'Apache..

Pour pouvoir modifier tous ça , on va mettre nos fichiers .html ou .php dans "/var/www/html/"
