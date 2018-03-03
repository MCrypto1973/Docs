# Basic installation of Linux Mint
Creating a Linux Development Environment

## Download and install Linux Mint
* Download linux from https://linuxmint.com
* Create a new VMWare with Linux Mint

## Install VMWare Tools
* Download VMWare-Tools
* cd /media/<user>/VMWare Tools
* cp *.tar.gz ~/Downloads/
* tar -zxvf VMWareTools-<version>-tar.gz
* cd vmware-tools-distrib/
* sudo ./vmware-install.pl
* Reboot virtual machine

## Update and Upgrade Packages
* sudo apt-get update (Updates the package lists for upgrades)
* sudo apt-get -y dist-upgrade (Upgrade the obsolete packages and dependencies)


## Install Git
* sudo apt-get install -y git 
