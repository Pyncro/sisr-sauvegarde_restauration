# sisr-sauvegarde_restauration



## Contexte:

Vous travaillez pour un prestataire de services informatiques. Egnom, cette PME assure diverses missions liées à l’infrastructure matérielle et logicielle pour le compte d’autres entreprises dépourvues de personnel dédié à ces taches.

Vous êtes chargé de répondre à la demande d’une petite entreprise spécialisée dans le développement back-end de sites d’e-commerce.
Cette structure emploie six personnes, chacune dotée d’une station de travail reliée par un support cuivre à la box d’un FAI.
Le réseau local comprend également un serveur de stockage et une imprimante, eux aussi reliés à la box.


## Expression de la demande: 

Le gérant de l’entreprise souhaite pourvoir réaliser des sauvegardes complètes des stations de travail afin de pouvoir réaliser rapidement une restauration en cas de problème.

Il souhaite pouvoir stocker ces sauvegardes sur le serveur local, et réaliser la restauration depuis ce dernier (donc à travers le réseau).

Une sauvegarde complète sollicitant de façon durable le réseau, il est nécessaire de prévoir un outil de planification de réalisation des sauvegardes afin de ne pas consommer de la bande passante en pleine journée.

La rédaction d’une documentation complète détaillant les procédures de sauvegarde et de restauration est attendue. Elle sera à destination du gérant, qui dispose de bonnes connaissances en informatique mais pas de grandes compétences en réseau.


### Étape 1 - Installer fog project

```
sudo -i

wget https://github.com/FOGProject/fogproject/archive/1.5.10.tar.gz

tar xvzf 1.5.10.tar.gz

cd fogproject-1.5.10

cd bin

./installfog.shb  

```

### Étape 2

Activez le DHCP pour le serveur de fog et il vous fournira une adresse IP et un login.

<img src="https://github.com/Pyncro/sisr-sauvegarde_restauration/blob/main/fog%20tp/fog-credentials.PNG" />


### Étape 3

L'utilisation d'une machine secondaire avec un système d'exploitation quelconque activera le réglage de fog si vous appuyez sur F12 pendant le menu de démarrage.

<img src="https://github.com/Pyncro/sisr-sauvegarde_restauration/blob/main/fog%20tp/fogf12.PNG" />

### Étape 4

Le sauvegarde s'affiche
https://github.com/Pyncro/sisr-sauvegarde_restauration/blob/main/fog%20tp/imagesavailable.PNG

Associer une image avec la machine pour faire un backup
https://github.com/Pyncro/sisr-sauvegarde_restauration/blob/main/fog%20tp/registerimage.PNG

Les machines sauvegardé.
https://github.com/Pyncro/sisr-sauvegarde_restauration/blob/main/fog%20tp/servers-registered.PNG

#### Source

https://www.infothema.fr/documents/juillet-2022/fogproject.pdf
