---
title: "Installation unter Linux"
date: 2020-12-31T09:29:07+02:00
draft: false
chapter: true
weight: 60
---
# Installation von Element Desktop unter Linux
Wir empfehlen das Installieren des Clients über die Paketverwaltung der jeweiligen Distribution. Die folgenden Befehle installieren den Element Desktop Client über die Kommandozeile.

### Debian/Ubuntu
```sh
sudo apt install -y wget apt-transport-https

sudo wget -O /usr/share/keyrings/riot-im-archive-keyring.gpg https://packages.riot.im/debian/riot-im-archive-keyring.gpg

echo "deb [signed-by=/usr/share/keyrings/riot-im-archive-keyring.gpg] https://packages.riot.im/debian/ default main" | sudo tee /etc/apt/sources.list.d/riot-im.list

sudo apt update

sudo apt install element-desktop
```
### Fedora
```sh
sudo dnf install -y dnf-plugins-core distribution-gpg-keys
sudo dnf copr enable taw/element
sudo dnf install -y element --refresh
```
### Arch Linux
```sh
sudo pacman -Sy element-desktop
```
### NixOS
```sh
nix-env -iA nixos.element-desktop
```
