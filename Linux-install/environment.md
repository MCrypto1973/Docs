  ## Common Environment
* ### Download and install Linux Mint
  * Download linux from https://linuxmint.com
  * Create a new VMWare with Linux Mint
* ### Install VMWare Tools
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
  * sudo apt-get update 
* ### Upgrade obsolete packages and dependencies
  * sudo apt-get -y dist-upgrade
