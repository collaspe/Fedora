# Fedora
## Configuration de Fedora sur mon PC Lenovo Ideadpad 330-15ARR

### 1. À faire dès la distribution installée
#### a)
##### 


## Lignes de commande à connaître
### 1. 
#### a) Mises à jour
* dnf check-update
* dnf upgrade
* dnf system-upgrade

#### b) Installer et desinstaller des logiciels
* dnf install
* dnf remove


#### c) Supprimer un logiciel et des dépendances
*

### 2. Flatpak
#### Installer Flatpak
* sudo zypper install flatpak
#### Ajouter le depot Flatpak
* flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
#### a) Lister les paquets
* flatpak list
#### b) Installer un logiciel
* flatpak install 'nom du logiciel'
#### c) Désinstaller un logiciel
* flatpak uninstall 'nom du logiciel'

## GNOME
### 1. Extensions Gnome
