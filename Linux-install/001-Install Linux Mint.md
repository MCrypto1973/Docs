# Basic installation of Linux Mint
Creating a Linux Development Environment

## Common Environment
* ### Download and install Linux Mint
  * Download linux from https://linuxmint.com
  * Create a new VMWare with Linux Mint
* ### Setting root password
  * sudo passwd root
  * enter sudo password
  * enter root password
* ### Testing root
  * su
  * enter root password
* ### Install VMWare Tools
  * log with root
    * su
  * Download VMWare-Tools
    * cd /media/<user_login>/VMWare Tools
    * cp *.tar.gz ~/Downloads/
    * tar -zxvf VMWareTools-<version>-tar.gz
    * cd vmware-tools-distrib/
    * ./vmware-install.pl
    * cd..
    * rm -rf vmware-tootls-distrib/
    * rm -rf VMwareTools-<version>-tar-gz
  * Reboot virtual machine
* ### Update the package list
  * log with root
    * su
  * sudo apt-get update 
* ### Upgrade obsolete packages and dependencies
  * log with root
    * su
  * sudo apt-get -y dist-upgrade
