

# SETUP

npm install
nano .env.jnft

This Repo is based on <a href="https://github.com/casper-ecosystem/casper-nft-cep47/blob/master/Contract-Interaction-Tutorial.md">Contract-Interaction-Tutorial</a>
and intended for use within the Casper ecosystem / CasperLab.
I created this repo to have a standalone integration of the NFT-client and will modify it to suit my personal needs.
Before Interacting with a Contract on the Casper Chain, follow this tutorial <a href="https://github.com/casper-ecosystem/casper-nft-cep47/blob/master/Basic-Tutorial.md#sending-the-contract-to-the-network">Install an NFT contract</a>

default path for secret_key.pem and public_key.pem is ../keys/***.pem

----- CONTENT .env.jnft -----
```python

CHAIN_NAME=casper-test
NODE_ADDRESS=http://136.243.187.84:7777/rpc
EVENT_STREAM_ADDRESS=http://136.243.187.84:9999/events/main
MASTER_KEY_PAIR_PATH=../keys
USER_KEY_PAIR_PATH=../keys

TOKEN_NAME=JonasToken
CONTRACT_NAME=my_contract
TOKEN_SYMBOL=JO
TOKEN_META=ID1 NumberOne,ID2 NumberTwo
INSTALL_PAYMENT_AMOUNT=250000000000

MINT_ONE_PAYMENT_AMOUNT=2000000000
MINT_COPIES_PAYMENT_AMOUNT=100000000000
BURN_ONE_PAYMENT_AMOUNT=12000000000
MINT_ONE_META_SIZE=1
MINT_COPIES_META_SIZE=10
MINT_COPIES_COUNT=20
MINT_MANY_META_SIZE=5
MINT_MANY_META_COUNT=5
TRANSFER_ONE_PAYMENT_AMOUNT=2000000000
```
----- END -----

# Content

## Latest

```
	test function calls Balance of Master account,
	test function mints a unique NFT ( hardcoded ),
	test function calls Balance of Master account again

```

## Future Goals

```

	- Create an Interface for a node.js server
 	to easily access all the NFT endpoints.

	- Store JPGs Metadata on the Blockchain,
	Browser NFTs associated with account and 
	retreive their Metadata from the Blockchain.
	

```
