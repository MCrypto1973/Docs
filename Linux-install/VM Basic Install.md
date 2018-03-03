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

*** 

## Java Environment
### Install Java from Oracle
* sudo add-apt-repository ppa:webupd8team/java
* sudo apt-get update
* sudo apt-get install oracle-java9-installer
* sudo apt-get install oracle-java9-set-default
## Install Spring Tool Suite
* Download and install from https://spring.io/tools
  * cd ~/Download
  * tar -zxvf spring-tool-suite-<version>-linux-gtk-x86_64.tar.gz
  * rm -rf spring-tool-suite-<version>-linux-gtk-x86_64.tar.gz
  * mkdir ~/Development
  * mv ./* ~/Development

***

## Angular Environment
# Install Visual Studio Code
* Download and install from https://code.visualstudio.com/download
## Install NodeJS
* curl -sL https://deb.nodesource.com/setup_9.x | sudo -E bash -
* sudo apt-get install -y nodejs
* sudo apt-get install -y build-essential
## Upgrade NPM
* sudo npm install npm@latest -g

***

## Solidity Environment
## Install Truffle
* sudo npm install -g truffle 
## Install Ganache
* sudo npm install -g ganache-cli
## Install Geth
* download Geth install from https://ethereum.github.io/go-ethereum/downloads/ (Download vesion 1.7.3, version 1.
8.x can't connect with Mist)
* Go to download folder to extract
  * mkdir ~/Development/geth-1.7.3
  * tar -zxvf ~/Downloads/geth-linux-amd64-<version>.tar.gz  
  * cp ./geth-linux-amd64-<version>/* ~/Development/geth-1.7.3
  * rm -rf geth*
* Create genesis.json file on ~/Development/geth-1.7.3
```json
{
  "difficulty" : "0x20000",
  "extraData"  : "",
  "gasLimit"   : "0x8000000",
  "alloc": {},
  "config": {
        "chainId": 15,
        "homesteadBlock": 0,
        "eip155Block": 0,
        "eip158Block": 0
    }
}
```
## Install Mist
* download Mist from https://github.com/ethereum/mist/releases
* Install Mist
