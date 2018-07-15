  ## Common Environment
* ### Download and install Linux Mint
  * Download linux from https://linuxmint.com
  * Create a new VMWare with Linux Mint
* ### Install VMWare Tools
* Download VMWare-Tools
    * cd /media/<user_login>/VMWare Tools
    * tar -zxvf VMWareTools-<version>-tar.gz -C ~/Downloads
    * cd ~/Downloads
    * sudo ./vmware-tools-distrib/vmware-install.pl
    * rm -rf vmware-tootls-distrib/
  * Reboot virtual machine
* ### Update the package list
  * sudo apt-get update 
* ### Upgrade obsolete packages and dependencies
  * sudo apt-get -y dist-upgrade

# Java Environment
* ## Install Java from Oracle
  * sudo add-apt-repository ppa:linuxuprising/java
  * sudo apt-get update
  * sudo apt-get install oracle-java10-installer
  * sudo apt-get install oracle-java10-set-default
