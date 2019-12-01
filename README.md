﻿# offchain-ethereum-storage
 
 ## Storage on IPFS
 
 Using a Merkle B-tree implemented on a decentralized public (and free) storage (like this implementation ) we satisfy the requirement of have a free and fast storage for the dataset. Now the problem remains who can update the root of this Merkle tree, that is the administrator.
 
 ## Smart Contract Admin
 
 Now the database will be administered by an Ethereum smart contract. Then we can have, for example, and open database where anyone can add elements but only the owner of the smart contract can remove data. Or we can have a group of administrators that can add or delete elements from the database. In the standard Ethereum-type blockchain, everything is public, so anyone can read the database if is in plain-text. If you use an encrypted database you can have that too.
 
 In the smart contract, at least you need to store the root of the Merkle B-tree, and anyone update the database/table will have to update the root of the tree on the smart contract.
 
 ## Checking immutability
 
 maintaining immutability of the database accros transactions is a property that we want to move from Ethereum into our off-chain storage. For this, we 
