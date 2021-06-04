# Block-lattice - Directed Acyclic Graphs \(DAGs\)

The Block-lattice is a structure where every user \(address\) gets their own chain that only they can write to, and everyone holds a copy of all of the chains. Block-lattice transform a shared global ledger\(like in Bitcoin\) into a set of non-shared asynchronous ledgers, which speed up transactions time.

![block-lattice1.png](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/block-lattice1.png) 

Blockchain consists of ordered units called blocks . Blocks contain headers and transactions. Each block header, amongst other metadata, contains a reference to its predecessor in the form of the predecessor's hash. The initial state is hard-coded in the first block called the genesis block. Unlike other blocks, the genesis block has no predecessor.

![block-lattice2.png](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/block-lattice2.png) 

In contrast to blocks, a DAG structure stores transactions in nodes, where each node holds a single transaction. In Nano, every account is linked to its own account-chain in a structure called the block-lattice equivalent to the account's transaction/balance history. The structure of the block-lattice is displayed in Figure 2. Each account is granted an account chain. An account chain can be considered as a dedicated blockchain, just for a single account. Nodes are appended to an account-chain, each node representing a single transaction on the account chain. Similar to the genesis block in blockchain, a DAG holds a genesis transaction. The genesis transaction defines the initial state. In Nano, instead of having a single transaction that transfers value, two transactions are needed to fully execute a transfer of value. A sender generates a send transaction, while a receiver generates a matching receive transaction, as depicted in Figure 3. When a send transaction is issued, funds are deducted from the balance of the sender's account, and are pending in the network awaiting for the recipient to generate the corresponding receive transaction. While in this state, transactions are deemed unsettled. When the receive transaction is generated, the transaction is settled. The downside of this approach is that a node has to be online in order to receive a transaction.

![block-lattice3.png](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/block-lattice3.png) 

Transaction handling in the block lattice. S represents a send transaction, R represents a receive transaction.

Every transaction is broken down into both a **send block** on the sender’s chain and a **receive block** on the receiving party’s chain. A send transaction will deduct funds from a sender’s balance, whilst a receive transaction will add funds to a receiving account’s balance. If the account owner misbehaves, then the rest of the network will vote against the invalid block and it will be rejected.

Each account chain can only be updated by the accounts owner. This is because each block in the chain must be signed by the accounts private key. The rest of the node network will still check and verify that every block is valid and make sure there are no double spends and that people don't increase their balance more than they are supposed to.

Nano **secures its ledger** through the use of **Open Representative Voting \(ORV\)**: With ORV, users have the ability to choose a representative node to vote on their behalf, acting as a voting proxy. A representative node fulfills tasks such as verifying signatures for blocks that are processed, and in the event of conflicting transactions, voting for the valid transaction. The voting process is balance-weighted, meaning that the weight of a representative’s vote is directly proportional to the amount of Nano that have been linked to it. The greater the number of Nano linked to a representative, the more its vote will be worth. This is possibly more secure than POW coins which rely on 51% of the hashing power: anyone who launches a 51% attack on a ORV coin would have to own 51% of all coins.

Nano use Proof of Work \(PoW\) to avoid spammers as there is no transaction fees on the network. Each block has a small amount of work associated with it, approximately about 5 seconds to generate, and 1 microsecond to validate. This forces a malicious actor to dedicate a significant amount of computing power to carry out an attack, whilst requiring only a small amount of computing power by everyone else. Furthermore, it is also even possible for these spam transactions to be pruned away, limiting the amount of storage that can be consumed from this type of attack.

#### Attacks
* Block gap synchronization: Each block has a link to its previous block. If a new block arrives where we can't find the previous block, this leaves the node deciding whether it's out of sync or if someone is sending junk data. If a node is out of sync, synchronizing involves a TCP connection to a node that offers bootstrapping which is much more traffic than sending a single UDP packet containing a block; this is a network amplification attack. Defense: For blocks with no previous link, nodes will wait until a certain threshold of votes have been observed before initiating a connection to a bootstrap node to synchronize. If a block doesn't receive enough votes it can be assumed to be junk data.


* Transaction flooding: Transaction flooding is simply sending as many valid transactions as possible in order to saturate the network. Usually an attacker will send transactions to other accounts they control so it can be continued indefinitely. Defense: Each block has a small amount of work associated with it, around 5 seconds to generate and 1 microsecond to validate. This work difference causes an attacker to dedicate a large amount to sustain an attack while wasting a small amount of resources by everyone else. Nodes that are not full historical nodes are able to prune old transactions from their chain, this clamps the storage usage from this type of attack for almost all users.


* Sybil attack to change ledger entries: A Sybil attack is a person creating a lot of nodes on the network, possibly thousands on a single machine, in order to get a disproportionate vote on networks where each node gets an equal vote. Defense: The Nano voting system (ORV) is weighted based on account balance. Adding extra nodes in to the network will not gain an attacker extra votes.


* Penny-spend attack: A penny-spend attack is where an attacker spends infinitesimal quantities to a large number of accounts in order to waste the storage resources of nodes. Defense: Blocks publishing is rate-limited by work so this limits accounts to a certain extent. Nodes that are not full historical nodes can prune accounts below a statistical metric where the account is probably not a valid account. Finally, Nano is tuned to use minimal permanent storage space so space required to store one additional account is proportional to the size of one block + indexing ~ 96b + 32b ~ 128b. This equates to 1GB being able to store 8 million penny-spend account. If nodes want to be aggressive, they can calculate a distribution based on access frequency and delegate infrequently used accounts to slower storage.


* read more in [Nano docs](https://docs.nano.org/protocol-design/attack-vectors/)

![Visualization of the block-lattice](https://s6.gifyu.com/images/Nano_blocklattice.gif)

## Used in

* Nano \(first to introduce\) [https://nano.org/](https://nano.org/) \(previously Raiblocks [https://raiblocks.net/](https://raiblocks.net/)\)
* Banano \(A fork of Nano\) [https://banano.cc/](https://banano.cc/)

## Pros

* Less intensive storage requirements by means of database pruning since each user’s blockchain tracks their account balance, rather than their transaction amounts.
* User’s blockchain can be updated asynchronously to the rest of the block lattice.
* faster transaction times: the entire network no longer has to process every single transaction that is made. 
* No transaction fees on the network
* Nano is a deflationary currency \(a currency that constantly increases in value\)

## Cons

* No smart contracts
* No monetary incentives for running a full node

## In Summary
  * The Block-lattice is a structure where every user \(address\) gets their own chain that only they can write to, and everyone holds a copy of all of the chains. 
  * Every transaction is broken down into both a send block on the sender’s chain and a receive block on the receiving party’s chain. 


#### Read more

[Nano Whitepaper](https://docs.nano.org/whitepaper/english/)

