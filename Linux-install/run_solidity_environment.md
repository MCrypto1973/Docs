
* ## Running Geth
  * geth --datadir=~/Development/geth-1.7.3/chaindata/ --rpc --rpccorsdomain "http://localhost:8000"
  
* ## Running Mist and create ETHERBASE Account
  * mist --node-datadir="~/Development/geth-1.7.3/chaindata/" --rpc ~/Development/geth-1.7.3/chaindata/geth.ipc
  * Start wallet
  * Create the ETHERBASE ACCOUNT
  
* ## Attach Geth Console to Geth Server
  * geth attach ipc:/home/marcio/Development/geth-1.7.3/chaindata/geth.ipc
  
* ## Start miner
  * miner.start()
* ## Stop miner
  * miner.stop()
