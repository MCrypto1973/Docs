# Basic installation of Linux Mint
Creating a Linux Development Environment

## Common Environment
### Download and install Linux Mint
* Download linux from https://linuxmint.com
* Create a new VMWare with Linux Mint
### Install VMWare Tools
* Download VMWare-Tools
* cd /media/<user>/VMWare Tools
* cp *.tar.gz ~/Downloads/
* tar -zxvf VMWareTools-<version>-tar.gz
* cd vmware-tools-distrib/
* sudo ./vmware-install.pl
* rm -rf vmware-tootls-distrib/
* rm -rf VMwareTools-<version>-tar-gz
* Reboot virtual machine
### Update the package list
* sudo apt-get update 
### Download and install Chrome
* Doandload and install from https://www.google.com/chrome/
### Install Git
* sudo apt-get install -y git 
### Upgrade obsolete packages and dependencies
* sudo apt-get -y dist-upgrade 

## Java Environment
### Install Java from Oracle
* sudo add-apt-repository ppa:webupd8team/java
* sudo apt-get update
* sudo apt-get install oracle-java9-installer
* sudo apt-get install oracle-java9-set-default
## Install Spring Tool Suite
* Download and install from https://spring.io/tools
* mkdir Development
* cd Development
* mv ~/Download/* ./
* tar -zxvf spring-tool-suite-<version>-linux-gtk-x86_64.tar.gz
* rm -rf spring-tool-suite-<version>-linux-gtk-x86_64.tar.gz

## Angular Environment
# Install Visual Studio Code
* Download and install from https://code.visualstudio.com/download
## Install NodeJS
* curl -sL https://deb.nodesource.com/setup_9.x | sudo -E bash -
* sudo apt-get install -y nodejs
* sudo apt-get install -y build-essential
## Upgrade NPM
* sudo npm install npm@latest -g

## Solidity Environment
## Install Truffle
* sudo npm install -g truffle 
## Install Ganache
* sudo npm install -g ganache-cli
