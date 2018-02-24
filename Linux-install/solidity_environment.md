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
