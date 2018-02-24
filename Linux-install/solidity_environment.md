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
* download Geth install from https://ethereum.github.io/go-ethereum/downloads/ (Download vesion 1.7.3, version 1.
8.x can't connect with Mist)
* Go to folder to extract
* tar -zxvf ~/Downloads/geth-linux-amd64-<version>.tar.gz
* copy all inside /geth-linux-amd64-<version> to /Geth-1.7.3
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
* PATH=~/Development/Geth-1.7.3/:$PATH


## Start genesis file
* geth --datadir=./chaindata/ init ./genesis.json


## Start Geth
* geth --datadir=./chaindata/ --rpc


## Install Mist
* download Mist from https://github.com/ethereum/mist/releases
* Install Mist


## Start Mist Wallet
* mist --node-datadir="~/Development/Geth-1.7.3/chaindata/" --rpc ~/Development/Geth-1.7.3/chaindata/geth.ipc
* Start wallet
* Create the ETHERBASE ACCOUNT


## Attach Geth Console to Geth Server
* geth attach ipc:/home/marcio1973/Development/Geth-1.7.3/chaindata/geth.ipc 


## Strat Miner
* miner.start()

## Change truffle.js
```javascript
module.exports = {
  // See <http://truffleframework.com/docs/advanced/configuration>
  // for more about customizing your Truffle configuration!
  networks: {
    development: {
      host: "127.0.0.1",
      port: 7545,
      network_id: "*"
    },
    ourTestNet: {
      host: "127.0.0.1",
      port: 8545,
      network_id: "*" 
    }
  }
};
```

