# Fedora
## Configuration de Fedora sur mon PC Lenovo Ideadpad 330-15ARR

### 1. À faire dès la distribution installée
#### a) Installer un dépot communautaire : RPM Fusion
Lien : https://rpmfusion.org/Configuration
* sudo dnf install https://mirrors.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://mirrors.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm

#### b) Installer les pilotes NVIDIA (RTX 2070)
Lien : https://rpmfusion.org/Howto
Lien : https://rpmfusion.org/Howto/NVIDIA?highlight=%28%5CbCategoryHowto%5Cb%29
* sudo dnf update -y # and reboot if you are not on the latest kernel
* sudo dnf install akmod-nvidia # rhel/centos users can use kmod-nvidia instead
* sudo dnf install xorg-x11-drv-nvidia-cuda #optional for cuda/nvdec/nvenc support
* modinfo -F version nvidia
* lsmod | grep nouveau
* Rebooter le PC

#### c) Installer logiciel pour configurer la souris
* sudo dnf install piper

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
* Dash To Dock
* Compiz alike magic lamp effect
