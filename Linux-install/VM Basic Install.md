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
* rm -rf vmware-tootls-distrib/
* rm -rf VMwareTools-<version>-tar-gz
* Reboot virtual machine

## Update the package list
* sudo apt-get update 

## Upgrade obsolete packages and dependencies
* sudo apt-get -y dist-upgrade 

## Install Java from Oracle
* sudo add-apt-repository ppa:webupd8team/java
* sudo apt-get update
* sudo apt-get install oracle-java9-installer
* sudo apt-get install oracle-java9-set-default

## Download and install Chrome
* Doandload and install from https://www.google.com/chrome/

## Install Git
* sudo apt-get install -y git 

## Install Spring Tool Suite
* Download and install from https://spring.io/tools
* mkdir Development
* cd Development
* mv ~/Download/* ./
* tar -zxvf spring-tool-suite-<version>-linux-gtk-x86_64.tar.gz
* rm -rf spring-tool-suite-<version>-linux-gtk-x86_64.tar.gz
