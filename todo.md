# STEP 1 - Get NFT from wallets

* Get NFT loaders built for differnet chains/wallets.
* Retern type doesn't matter, assuming we have some JSON that has NFT information in it for the wallet we're interested in, we can mold that to our standard in step 2

getEthArt(walletAddress);
https://docs.opensea.io/reference

getWaxArt(walletAddress);
Source Code: https://github.com/pinknetworkx/eosio-contract-api
AtomicMarket
WAX Mainnet: https://wax.api.atomicassets.io/atomicmarket/docs/
EOS Mainnet: https://eos.api.atomicassets.io/atomicmarket/docs/
WAX Testnet: https://test.wax.api.atomicassets.io/atomicmarket/docs/
AtomicAssets
WAX Mainnet: https://wax.api.atomicassets.io/atomicassets/docs/
EOS Mainnet: https://eos.api.atomicassets.io/atomicassets/docs/
WAX Testnet: https://test.wax.api.atomicassets.io/atomicassets/docs/

getCounterpartyArt(walletAddress);
https://xchain.io/api
https://github.com/droplister/digirare.com/blob/master/routes/api.php

getNearArt(walletAddress);
https://docs.near.org/docs/develop/front-end/near-api-js

#
# STEP 2 - Standardize NFT attributes
#

JSON metadata:

MVP:
* thumbnail (as long as we have thumbnails there is something to display for step #3)

Bonus:
* raw metadata
* creator address
* creation time

#
# STEP 3 - Display wallet contents
#

* web UI that allows multiple wallets to be entered 
* display thumbnails when STEP 1 APIs return them via STEP 2 standard

