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
  
* ## Certification Problem
  * Download Oracle Java JDK 10
  * tar -zxvf jdk-<java_version>-linux-x64_bin.tar.gz
  * sudo cp ~/Downloads/jdk-10.0.1/lib/security/cacerts /etc/ssl/certs/java

* ## Install Spring Tool Suite
  * Download and install from https://spring.io/tools
    * cd ~/Download
    * tar -zxvf spring-tool-suite-<spring_version>-linux-gtk-x86_64.tar.gz
    * rm -rf spring-tool-suite-<spring_version>-linux-gtk-x86_64.tar.gz
    * mkdir ~/Development
    * mv ./* ~/Development
