# web-raspberry
serveur web avec raspberry


Près-requis:
 -raspbian a jour
 -connecxion ssh en tant que root(super-utilisateur)
 FileZilla sur le pc maître (windows ou mac)
 blocnote(windows) ou Visual Studio Code(mac)
 
 Installation:
 
 -Avoir tout les droit (root) => sudo nano /etc/ssh/sshd_config
 allez a la ligne  "PermitRootLogin" et mettez "PermitRootLogin yes"
 Puis control+x
 Ensuite sudo passwd root et choisisez votre mot de passe et confirmer.
 Enfin "sudo reboot"
 
 En root:
 -sudo apt-get update
 -sudo apt-get upgrade  
 -sudo apt-get install apache2
 -sudo apt-get install php
 
Droit d'ecriture, lecture et execution sur nos fichier html,php,py: sudo visudo
allez a la fin du fichier et taper:
www-data  ALL=(ALL:ALL) NOPASSWD: ALL

et enregistrez par control+x
 
et enfin : sudo reboot

Ouvrez votre navigateur (google ou modzila)..... et taper : http://ipdevotreraspberry
Vous tomberez sur la page de présentation d'Apache..

Pour pouvoir modifier tous ça , on va mettre nos fichier .html ou .php dans "/var/www/html/"
