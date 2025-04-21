>peer to peer architecture that leverages cryptography for ensuring security of data on the decentralized ledger and creating an addressing system

distributed database system - once data has been recorded inside the ledger it becomes difficult to change it

why are blockchains distributed
- instead of using a single entity to manage the chain, it uses a peer to peer network which anyone can join.
- when someone joins the network, they get a full copy of the blockchain to verify everything is still in order 
- when a new block is created, it is send to everyone on the network, where each peer will verify the block to ensure it's integrity, and then adds it to their blockchain, creating consensus (agreement on the blocks)
- even if blocks are tampered with, they'll be rejected by the other nodes in the network 
	- would need to tamper with every block in the network, redo proof of work for each block, and tamper with at least 50% of the peers on the network 

instead of storing exact transaction amounts in table e.g. for relational databases
transactions are saved within blocks where the amounts can be calculated based on previous transactions

![[Pasted image 20250416143858.png|600]]


what are blocks
- containers of information (e.g. containing a transaction) that can be linked together
- distributed infrastructure 

what information does each block contain 
- data - depends on the type of blockchain e.g. bitcoin blockchain stores transaction data
- own hash - uniquely identifies the data where changing the data changes the hash
- hash of previous block - to create the chain
- contains information on the previous block's hash, timestep, root, nonce
  ![[Pasted image 20250416145420.png|500]]![[Pasted image 20250416145532.png|500]]

the first block is called the genesis block since it does not have any previous blocks


what is a Merkle tree 
- a binary tree of hash values where each leaf node represents a single piece of data / a hash piece of data - use to verify the integrity of large amounts of data efficiently
- hashes are combined and rehashed to create new hashed (going up the tree) until they form into a root hash (Merkle Root)
- if any node changes, all the hashes above the node will also change
  
  ![[Pasted image 20250416144401.png]]

- to verify a node, download it's hash and parents and siblings and try to calculate the Merkle Root, if the Merkle root is not the same as it should be then something has changed
	- means we don't have to download every file in the tree


how does blockchain use Merkle Trees
- each leaf in the Merkle Tree is a block containing a transaction
  ![[Pasted image 20250416151758.png]]


in the exam need to understand which **consensus mechanisms** can be done when employing a blockchain architecture - for securing the blockchain and ensuring agreement between parties.

hashing is not enough to validate the blockchain since computers are good enough to manipulate the block and recalculate the entire hashes again to make it seem correct, so need to have consensus mechanisms 

what is a **consensus mechanisms**
- a method used to validate a transaction and ensure it is authentic 

what are the different consensus mechanisms 
- proof of work
- proof of stake
- proof of burn
- proof of capacity
- proof of authority
- proof of weight 


what is Proof of Work - Mining 
- cryptographic proof to verity cryptocurrency transactions and add them to the blockchain 
- required significant computational effort and time
- specifically a bitcoin equivalent, which if applied to a new system is too much processing power 


how does mining work
1. New block content hash is calculated. 
2. A nonce (random string) is appended to the hash. 
3. This new string is hashed again. 
4. The final hash is then compared to a difficulty level:
	1. – If NOT LESS, then the nonce is changed and the process repeats again. 
	2. – If LESS, then the block is added to the chain and the public ledger is updated and replicated. 
5. The miners responsible for this are rewarded with bitcoins


what is Proof of Stake 
- alternate way of verifying and validating the transaction or block
- validator is picked (equivalent of “miner” in the PoW) by the amount of stake (e.g. coins) a validator has and the respective age of the stake.
	- new traders and traders with little coins are not considered highly


smart contracts are an evolution on blockchain architecture 

what are smart contracts e.g. solidity
- a digital agreement stored and executed on a blockchain network that are programmed to perform specific actions once predefined conditions trigger them 
- e.g. automatically exchange coins

how do smart contracts work
- written using a program like ***Solidity*** to encode the contract's terms and instructions 
- contract is deployed onto the blockchain where it becomes immutable (unchangeable)
- when the conditions are met, smart contract automatically executes eg. release funds automatically to a wallet when a tenant transfers cryptocurrency 
- the contract execution is validated to ensure it ran as intended 
  
  ![[Pasted image 20250416151047.png]]
	e.g. instead of using kickstarter, people give money to the smart contract, if the money reaches the goal it goes to the owners, else it goes to the supporters 


what are the benefits of smart contracts 
- tamper proof and less susceptible to fraud like traditional contracts 
- instant execution 
- more secure due to immutability
- distributed - output of the contract is validated by everyone on the network, so a single person can't force the contract to release the funds

what are the cons of smart contracts 
- coding errors can result in weaknesses that hackers can exploit
- immutable also means mistakes are difficult to reverse

what are the uses cases of blockchain 
- cryptocurrency trading 
- storing medical records 
- e-notary - verifying the authenticity of documents 
- collecting taxes 
- managing the movement of goods through a supply chain 

what are the use cases of smart contracts 
- banks to automate loan issue or automatic payments
- insurance companies to process claims 
- postal companies to automatically do payment on delivery
- Ethereum is an open source blockchain network that has smart contract functionality 