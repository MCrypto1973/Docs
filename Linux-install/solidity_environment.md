# Install Solidity Environment

## Install NodeJS and update NPM

* curl -sL https://deb.nodesource.com/setup_9.x | sudo -E bash -
* sudo apt-get install -y nodejs
* sudo apt-get install -y build-essential
* sudo npm install npm@latest -g


## Install Truffle
* sudo npm install -g truffle 


## Install Ganache
* sudo npm install -g ganache-cli


## Install Geth
* download Geth install from https://ethereum.github.io/go-ethereum/downloads/
* Go to folder to extract
* tar -zxvf ~/Downloads/geth-linux-amd64-<version>.tar.gz
* Create genesis.json file
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
* PATH=~/Development/geth-linux-amd64-1.8.1-1e67410e/:$PATH
* geth --datadir=./chaindata/ init ./genesis.json


## Install Mist
* download Mist from https://github.com/ethereum/mist/releases


* ./geth --datadir=./chaindata/ --rpc
* mist --node-datadir="~/Development/geth-linux-<version>/chaindata/" --rpc ~/Development/geth-linux-<version>/chaindata/geth.ipc
* geth attach ~/Development/geth-linux-amd64-1.8.1-1e67410e/chaindata/geth.ipc 



./geth attach ipc:/home/marcio1973/Development/geth-linux-amd64-1.8.1-1e67410e/chaindata/geth.ipc 
