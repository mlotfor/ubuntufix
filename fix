#!/bin/bash
sudo mkdir -p /etc/apt/sources.list.d/kali-backup
sudo mv /etc/apt/sources.list.d/*kali* /etc/apt/sources.list.d/kali-backup/ 2>/dev/null
echo -e "deb http://archive.ubuntu.com/ubuntu plucky main restricted universe multiverse
deb http://archive.ubuntu.com/ubuntu plucky-updates main restricted universe multiverse
deb http://archive.ubuntu.com/ubuntu plucky-security main restricted universe multiverse
deb http://archive.ubuntu.com/ubuntu plucky-backports main restricted universe multiverse" | sudo tee /etc/apt/sources.list
sudo apt update
sudo apt install --allow-downgrades -y gnome-session-bin=47.0.1-2ubuntu3 gnome-session-common=47.0.1-2ubuntu3
sudo apt --fix-broken install -y
sudo apt install --reinstall -y ubuntu-desktop ubuntu-session
sudo apt autoremove -y
sudo reboot
