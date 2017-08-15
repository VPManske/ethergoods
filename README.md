TODO:

1. Write tests
2. Deploy to Ropsten using testnet coins
3. Write JS and use metamask to register a new Good, all on ropsten
4.


Fancy storage patterns
https://ethereum.stackexchange.com/questions/13167/are-there-well-solved-and-simple-storage-patterns-for-solidity


## HOW TO TEST

npm install -g ethereumjs-testrpc  (https://github.com/ethereumjs/testrpc)
testrpc

truffle test


##publish to RPOSTEN
1. Make an account with geth --testnet account new  and load it up with eth


2. run geth with
    geth --testnet --fast --rpc --rpcapi eth,net,web3,personal

    geth attach http://127.0.0.1:8545


    personal.unlockAccount(eth.accounts[0])

3. truffle migrate --network ropsten


### Published contracts on ROPSTEN
rev1.  0xdd6fa24be361432c0359ab7f2bde155a4fc31ce5


### HOW TO IMPROVE

-dont allow for bidding or offering on individual supplies of the goods.  Just allow for a bid or offer of ANY supply  and then fulfillment as such ! That way the bids and offers arent mapped inside the struct.
