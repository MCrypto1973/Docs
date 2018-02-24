# Linux-Install
Creating a Linux Development Environment


## Install VMWare Tools
  
* Download VMWare-Tools
* cd /media/marcio1973/VMWare Tools
* cp *.tar.gz ~/Downloads/
* tar -zxvf VMWareTools-<version>-tar.gz
* cd vmware-tools-distrib/
* sudo ./vmware-install.pl
* Reboot virtual machine


## Update and Upgrade Packages

* sudo apt-get update (Updates the package lists for upgrades)
* sudo apt-get dist-upgrade (Upgrade the obsolete packages and dependencies)


## Install Git

* sudo apt-get install git 


## Install GEdit
* sudo apt-get install gedit
