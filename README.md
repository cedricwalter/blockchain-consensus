# README

![Logo](https://www.tokens-economy.com/wp-content/uploads/2018/06/logo.png)

## Blockchain Consensus Encyclopedia

More than 66 Blockchain Consensus described.

Donations

* Ethereum [0xC23473B911e86dc614412b3341d1C206aBac6996](https://etherscan.io/address/0xC23473B911e86dc614412b3341d1C206aBac6996#)
* Bitcoin [3ERPPUFLLjmRAookiCTN7rqKkQjDwS8YPe](https://www.blocktrail.com/BTC/address/3ERPPUFLLjmRAookiCTN7rqKkQjDwS8YPe)


## Limited Confidence Proof-of-Activity \(LCPoA\)

Limited Confidence Proof-of-Activity \(LCPoA\) - a method for blockchain protection, based on the modification of the Proof-of-Work algorithm, in the direction of reducing the consumption of computational resources for the block generating. When using this method, the algorithm for block generating does not depend on the computing power. As a proof of work \(or activity\) the algorithm checks the time spent on the solution.

### Used in

* izzz.io [https://izzz.io/](https://izzz.io/)
* BitCoen [https://bitcoen.io](https://bitcoen.io)

### Read more

* Wiki [https://en.bitcoinwiki.org/wiki/Limited\_Confidence\_Proof-of-Activity](https://en.bitcoinwiki.org/wiki/Limited_Confidence_Proof-of-Activity)
* Medium [https://medium.com/@izzzio/lcpoa-universal-as-pow-economical-as-pos-c26f6ba90017](https://medium.com/@izzzio/lcpoa-universal-as-pow-economical-as-pos-c26f6ba90017)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

### Proof of Believability

IOST introduced Servi as both a measurement of users’ contribution to the community and a way to encourage members to contribute to the continued development of the IOSChain.

### Used in

* IOST

  **Read more**

* [whitepaper](https://github.com/iost-official/Documents/blob/master/Technical_White_Paper/EN/Tech_white_paper_EN.md#consensus-mechanism)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## HoneyBadgerBFT

The surprising success of cryptocurrencies has led to a surge of interest in deploying large scale, highly robust, Byzantine fault tolerant \(BFT\) protocols for mission-critical applications, such as financial transactions. Although the conventional wisdom is to build atop a \(weakly\) synchronous protocol such as PBFT \(or a variation thereof\), such protocols rely critically on network timing assumptions, and only guarantee liveness when the network behaves as expected. We argue these protocols are ill-suited for this deployment scenario. We present an alternative, HoneyBadgerBFT, the first practical asynchronous BFT protocol, which guarantees liveness without making any timing assumptions. We base our solution on a novel atomic broadcast protocol that achieves optimal asymptotic efficiency. We present an implementation and experimental results to show our system can achieve throughput of tens of thousands of transactions per second, and scales to over a hundred nodes on a wide area network. We even conduct BFT experiments over Tor, without needing to tune any parameters. Unlike the alternatives, HoneyBadgerBFT simply does not care about the underlying network.

### Read more

* [link1](https://dl.acm.org/citation.cfm?id=2978399)
* [link2](https://infoscience.epfl.ch/record/222858/files/199.pdf)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Proof of Care \(PoC\)

Rather than distributing presale tokens based on, say, how much users are contributing, companies can distribute token based on the quality of your proof-of-care for the project. On top of that, it's not even about social proof \(i.e., how many Twitter followers you have\), it's about the genuineness of your proof-of-care.

It's a great way to essentially crowd-market your blockchain project by encouraging others to get the word out about it. it's about producing interesting, fun, informative content.

### Used in

* Quantstamp
* TomoCoin

### Pros

* Implementing individual caps is very good step and can restrict whales from entering the public sale
* Attract long term investors
* Help spread the word by individuals

  **Cons**

* Content creators have an advantage as they will have more influence and better chances to make it through.
* Other people will just copy content from other's post just to complete their Proof of Care = lot of spam.

  **Read more**

  Whitepaper [https://github.com/iost-official/Documents/blob/master/Technical\_White\_Paper/EN/Tech\_white\_paper\_EN.md\#consensus-mechanism](https://github.com/iost-official/Documents/blob/master/Technical_White_Paper/EN/Tech_white_paper_EN.md#consensus-mechanism)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Proof of Value \(PoV\)

Earn token when user publish work to audience.

### Used in

* [whitepaper](https://docs.google.com/document/d/1VogMc11WOeWB_OrcsIGD_J7F02KZ0I5zlDYTma7FJkA/edit)

### Read more

* LTBcoin

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Proof of Quality \(PoQ\)

E.g after PoV a month later when the performance of any work is compared against all the other work published during that week, user get an additional reward

### Used in

* [whitepaper](https://docs.google.com/document/d/1HBbuN8rmrH22kXSYiDZaRv9aR7MVrI4FB8fSrSQ37tc/edit)

  **Read more**

* LTBcoin

## Variable Delayed Proof Of Stake \(vDPOS\)

Ongoing, but you can help me with links, contact me

### Used in

* CryptoCircuits

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Proof-of-work time \(PoWT\)

Proof-of-Work-Time \(PoWT\) is a novel approach to forming a consensus by introducing a variable blocktime that scales with mining power, where the blockchain speeds up with power increases. This better scales the blockchain, increases transaction speed with power and allows for auto-adjusting more profitable mining. Difficulty dependent blocktime \(Max ~6.2 minutes, minimum 15 seconds\).

Blocktime dependent rewards \(~Reward halving every minute decrease in blocktime till 10x VRC supply parity, then variable ~3% disinflation\). Algo: scrypt² \(N of 1024² or 128MB per thread\) Block 1: 564,705 VRM minted for ICO participants who purchased VRM using VRC. Minimum Transaction Fee: 0.2 VRM \(high commodity transaction fee paid to miners\). RPC Port: 33987, P2Port: 36988 Confirmations: 30, Maturity: 100.

### Used in

* Vericoin
* Verium

### Read more

* [whitepaper](https://wiki.vericoin.info)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Serialization of Proof-of-work Events: Confirming Transactions via Recursive Elections

Utilizes a combination of PoW and DAGs to reach scalable consensus. In SPECTRE, the blocks are mined pointing to multiple parents, not just one, so the network could potentially handle multiple blocks per second. Mining a block pointing to some parent blocks supports those blocks validity. Compared to PoW’s “longest chain wins”, SPECTRE uses something like “blocks with the most childen win.” SPECTRE hasn’t been battle-tested in the wild yet, and new attack vectors are likely to emerge, but it feels like a very clever potential way to fix Bitcoin.

### Used in

* Proposal for Bitcoin [https://bitcoin.org/en](https://bitcoin.org/en)

## Proof-of-work \(PoW\) / High Interest Proof of Stake \(HiPoS\)

Coin combining PoW and HiPoS

### Used in

* EdgeCoin \(EDGE\)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Proof of Work \(PoW\) / Nexus Proof of State \(nPoS\) or Nexus Proof of Holding \(nPOH\)

Nexus uses 3 consensus channels to maximize decentralization and provide fast, secure transactions. Each channel has an independent difficulty algorithm, amongst other checks and balances, to prevent a single channel from monopolizing block production and compromising the security of the network. Nexus channels include a Prime channel \(CPU Mining\), a Hashing channel \(GPU Mining\), and Nexus Proof of Holding \(nPOH\). Nexus takes the proof-of-stake system developed by Peercoin, and combines it with a Trust-based weighting system to create the Proof-of-Holding consensus mechanism. Nodes receive a Trust rating that is established by their contributions to the network, which increases over time. Nodes with greater Trust are granted an increased minting rate, which increases from 0.5% to 3% within one year, the longer you build Trust on the network. 3 consensus channels: Prime \(CPU\), Hashing \(GPU\), and Nexus Proof of Holding \(nPOH\)

### Used in

* [Nexus](https://nexusearth.com)

### Pros

* Key signature scheme to keep an account’s public keys obscured even when making transactions \(This is made possible by moving away from addresses based on public key hashes, and implementing a new system called Signature Chains\).
* quantum resistance \(Nexus uses a combination of SHA3 hashing algorithms combined with 571 bit private keys and 512/1024 bit proof of work\)
* multiple consensus channels greatly reduces the risk of a 51% attack \(attacker would need to control all 3 channels\)
* OnChain scalability Transaction processing is distributed across multiple channels working synergistically to increase transaction throughput as resources increase. Individual channels verify transactions, consolidate verified transactions into Merkle trees, and add finished blocks onto the blockchain. The Unified Time protocol enables transaction processing, trust locks, and block locks to be consistent throughout time. The potential of Nexus 3DC is limited only by node count and represents the most energy-efficient consensus system to date.

### Read more

* [whitepaper](https://nexusearth.com/nexus-white-paper)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Delayed Proof of Work \(dPoW\)

Delayed Proof of Work \(dPoW\) is a hybrid consensus method that allows one blockchain to take advantage of the security provided through the hashing power of a secondary blockchain. This is achieved through a group of notary nodes that add data from the first blockchain onto the second, which would then require both blockchains to be compromised to undermine the security of the first.

Delayed Proof of Work \(dPoW\) is a hybrid consensus method that allows one blockchain to take advantage of the security provided through the hashing power of a secondary blockchain. This is achieved through a group of notary nodes that add data from the first blockchain onto the second, which would then require both blockchains to be compromised to undermine the security of the first. The first to make use of this consensus method is Komodo, which is attached to the Bitcoin blockchain.

### Used in

* [Komodo](https://komodoplatform.com) end-to-end blockchain solutions. DPoW consensus mechanism does not recognize The Longest Chain Rule to resolve a conflict in the network, instead the dPoW looks to backups it inserted previously into the chosen PoW blockchain. The process of inserting backups of Komodo transactions into a secure PoW is “notarization.” Notarisation is performed by the elected notary nodes. Roughly every ten minutes, the notary nodes perform a special block hash mined on the Komodo blockchain and take note of the overall Komodo blockchain “height”. The notary nodes process this specifc block so that their signatures are cryptographically included within the content of the notarized data. There are sixty-four “notary nodes” elected by a stake-weighted vote, where ownership of KMD represents stake in the election. They are a special type of blockchain miner, having certain features in their underlying code that enable them to maintain an effective and cost-efcient blockchain and they periodically receives the privilege to mine a block on “easy difculty.” [Whitepaper](https://komodoplatform.com/en/whitepaper/2018-02-14-Komodo-White-Paper-Full.pdf)

### pros

* Energy efficient
* Increased security

  **Cons**

* Limited to blockchain using PoW or PoS

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Delayed Proof of Work \(dPoW\)

Coin combining PoW and dPoW. Delayed Proof of Work \(dPoW\) is a hybrid consensus method that allows one blockchain to take advantage of the security provided through the hashing power of a secondary blockchain. This is achieved through a group of notary nodes that add data from the first blockchain onto the second, which would then require both blockchains to be compromised to undermine the security of the first. The first to make use of this consensus method is Komodo, which is attached to the Bitcoin blockchain.

### Used in

* [Komodo](https://wiki.komodoplatform.com/wiki/Komodo)

### Pros

* Energy efficient
* Increased security

### Cons

* Limited to blockchain using PoW or PoS

### Read more

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Proof of Work \(PoW\) / PoM / PoSII

Coin combining PoW and PoM and PoSII

### Used in

* NOBL
* Magi Coin

### Read more

* [Github](https://github.com/magi-project/m-Noblecoin)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Proof of Work \(PoW\) / Proof of Stake \(PoS\) / Proof Of Care \(PoC\)

Coin combining PoW and PoS and PoC

### Used in

* TamaGucci

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Proof of Stake \(PoS\) / Proof of Disintegration \(PoD\)

B3 is the first coin to develop and implement Fundamental Nodes \(FN\). A Fundamental Node is similar to a regular masternode in terms of the service it provides to the network but the coins used to purchase a Fundamental Node are destroyed. This reduces the overall supply of the coin over time as more Fundamental Nodes are added to the network. Fundamental Nodes receive 60% of the block reward while those staking receive 40%.

### Used in

* [b3coin](https://b3coin.io)

  **Read more**

* [whitepaper](https://b3coin.io)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Proof-of-Stake \(POS\) / Proof-of-Presence \(PoP\)

1. Reward for generating blocks \(Proof-of-Stake, POS\). This involves running a full node, unlocked and with the user's stake applied to generate blocks. Users who run a block generating node generally need to have at least a moderate amount of token on their account
2. Reward for storing the blockchain \(Proof-of-Presence, POP\). Only the most recent blocks file is distributed amongst all p2p nodes, previous blocks files are not needed for normal p2p operations. Token incentives users to store and make available previously archived block files.

### Used in

HEAT

### Read more

* [whitepaper](https://heatledger.com/HEATWhitepaper.pdf)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Leasing Proof of Stake \(PoS/LPoS\)

LPoS is an enhanced version of Proof-of-Stake. In a regular Proof-of-Stake system, each node that holds a certain amount of cryptocurrency is eligible to add the next block to the blockchain but in the LPoS system, on the Waves Platform, users can lease their balance to full nodes. WithLPoS, the user will have the ability to Lease WAVES form the wallet to different contractors which can pay a percentage as a reward. The larger the amount that is leased to a full node, the higher the chances of that full node being selected to produce the next block. If that full node is selected to produce the next block, the leaser will then receive a percentage of the transaction fee that is collected by the full node. In a LeasedProof-of-Stake environment, users can choose between running a full node or leasing their stake to a full node with receiving rewards. This system allows anyone to participate in the Waves network maintenance. User can leas his waves through leasing on any computer or mobile device that has an internet browser since Waves provides a lite client solution that does not require Miners, that are leasing their balance to store the whole Blockchain or to have the wallet running

### Used in

* Nxt
* Waves

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Direct Acyclic Graph

## Tangle \(DAG\)

Tangle is the DAG consensus algorithm used by Iota. In order to send an Iota transaction, you need to validate two previous transactions you’re received. The two-for-one, pay-it-forward consensus strengthens the validity of transactions the more transactions are added to the Tangle. Because the consensus is established by the transactions, theoretically, if someone can generate 1/3 of the transactions they could convince the rest of the network their invalid transactions are valid. Until there’s enough transaction volume that creating 1/3rd of the volume becomes unfeasible, Iota is sort-of “double-checking” all of the network’s transactions on a centralized node called “The Coordinator”. Iota says The Coordinator works like training wheels for the system, and will be removed once the Tangle is big enough.

![What is Tangle](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/tangle1.png)

This is directed, asynchronous graph \(DAG\) representing each individual transaction. You’ll notice that each transaction references exactly two other transactions to the left.

### Used in

* IOTA

  **Pros**

* Low transaction fees \(PoW on 2 other Tx\)
* Extremely small transactions
* Scalability
* Lightweight
* Quantum-secure \(Use trinary, or balanced ternary computations instead of the standard binary computations performed by classical computers\)

### Cons

* No Smart Contracts yet
* Vulnerable \(only 34% of the total hashing power required\)

### Read more

* [iota1\_4\_3.pdf](https://assets.ctfassets.net/r1dr6vzfxhev/2t4uxvsIqk0EUau6g2sw0g/45eae33637ca92f85dd9f4a3a218e1ec/iota1_4_3.pdf)
* [The Coordinator](https://domschiener.gitbooks.io/iota-guide/content/chapter1/current-role-of-the-coordinator.html)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Block-lattice - Directed Acyclic Graphs \(DAGs\)

The Block-lattice is a structure where every user \(address\) gets their own chain that only they can write to, and everyone holds a copy of all of the chains. Block-lattice transform a shared global ledger\(like in Bitcoin\) into a set of non-shared asynchronous ledgers, which speed up transactions time.

![block-lattice1.png](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/block-lattice1.png) Blockchain consists of ordered units called blocks . Blocks contain headers and transactions. Each block header, amongst other metadata, contains a reference to its predecessor in the form of the predecessor's hash. The initial state is hard-coded in the first block called the genesis block. Unlike other blocks, the genesis block has no predecessor.

![block-lattice2.png](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/block-lattice2.png) In contrast to blocks, a DAG structure stores transactions in nodes, where each node holds a single transaction. In Nano, every account is linked to its own account-chain in a structure called the block-lattice equivalent to the account's transaction/balance history. The structure of the block-lattice is displayed in Figure 2. Each account is granted an account chain. An account chain can be considered as a dedicated blockchain, just for a single account. Nodes are appended to an account-chain, each node representing a single transaction on the account chain. Similar to the genesis block in blockchain, a DAG holds a genesis transaction. The genesis transaction defines the initial state. In Nano, instead of having a single transaction that transfers value, two transactions are needed to fully execute a transfer of value. A sender generates a send transaction, while a receiver generates a matching receive transaction, as depicted in Figure 3. When a send transaction is issued, funds are deducted from the balance of the sender's account, and are pending in the network awaiting for the recipient to generate the corresponding receive transaction. While in this state, transactions are deemed unsettled. When the receive transac- tion is generated, the transaction is settled. The downside of this approach is that a node has to be online in order to receive a transaction.

![block-lattice3.png](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/block-lattice3.png) Transaction handling in the block lattice. S represents a send transaction, R represents a receive transaction.

Every transaction is broken down into both a **send block** on the sender’s chain and a **receive block** on the receiving party’s chain. A send transaction will deduct funds from a sender’s balance, whilst a receive transaction will add funds to a receiving account’s balance. If the account owner misbehaves, then the rest of the network will vote against the invalid block and it will be rejected.

Each account chain can only be updated by the accounts owner. This is because each block in the chain must be signed by the accounts private key. The rest of the node network will still check and verify that every block is valid and make sure there are no double spends and that people don't increase their balance more than they are supposed to.

Nano **secures its ledger** through the use of **delegated proof of stake \(dPoS\)**: With dPoS, users have the ability to choose a representative node to vote on their behalf, acting as a voting proxy. A representative node fulfills tasks such as verifying signatures for blocks that are processed, and in the event of conflicting transactions, voting for the valid transaction. The voting process is balance-weighted, meaning that the weight of a representative’s vote is directly proportional to the amount of Nano that have been linked to it. The greater the number of Nano linked to a representative, the more its vote will be worth. This is possibly more secure than POW coins which rely on 51% of the hashing power: anyone who launches a 51% attack on a DPOS coin would have to own 51% of all coins.

Nano use Proof of Work \(PoW\) to avoid spammers as there is no transaction fees on the network. Each block has a small amount of work associated with it, approximately about 5 seconds to generate, and 1 microsecond to validate. This forces a malicious actor to dedicate a significant amount of computing power to carry out an attack, whilst requiring only a small amount of computing power by everyone else. Furthermore, it is also even possible for these spam transactions to be pruned away, limiting the amount of storage that can be consumed from this type of attack.

### Attacks

* Penny-spend attack: attackers inflate the number of chains node must keep track of by sending negligible amounts to a wide array of empty wallets.
* Double spend by a malicious user. Both versions of the double spend need to be signed by the users private key. It is easy to identify the accounts that are responsible for spam attacks and then blacklist them for a certain period. 
* read more in [Nano wiki](https://github.com/clemahieu/raiblocks/wiki/Attacks)

![Visualization of block lattice](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/block-lattice.png)

### Used in

* Nano \(first to introduced\) [https://www.mycryptopedia.com/raiblocks-explained/](https://www.mycryptopedia.com/raiblocks-explained/) \(previously Raiblocks [https://raiblocks.net/](https://raiblocks.net/)\)

### Pros

* Less intensive storage requirements by means of database pruning since each user’s blockchain tracks their account balance, rather than their transaction amounts.
* User’s blockchain can be updated asynchronously to the rest of the block lattice.
* faster transaction times: the entire network no longer has to process every single transaction that is made. 
* No transaction fees on the network

### Cons

* No smart contracts
* No monetary incentives for running a full node
* Nano is a deflationary currency \(a currency that constantly increases in value\)

### Read more

[Nano Whitepaper](https://raiblocks.net/media/RaiBlocks_Whitepaper__English.pdf)

## LFT

LFT is a continuation of Tendermint to improve BFT consensus algorithms, it is currently what ICON uses as its consensus algorithm. LFT reduces communication overhead by consolidating messages from the network

### Used in

* [ICON](http://icon.support/a-primer-to-lft-loop-fault-tolerance-consensus-algorithm)

### Read more

* [ICON](http://icon.support/a-primer-to-lft-loop-fault-tolerance-consensus-algorithm)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Modified Federated Byzantine Agreement \(mFBA\)

FBA organises nodes into groups call quorums whereby overall consensus is met by: Quorum consensus among a certain amount of nodes \(within a specific quorum\); then Consensus among a certain number of quorums to finally determine the final consensus.

![mFBA](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/mFBA.png)

### pros

* Decentralized control
* Low latency
* Flexible trust
* Asymptotic security

  **Read more**

* [Medium](https://medium.com/@boscoin/dpos-mfba-c84bae2e21ae)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Federated Byzantine Agreement

The general idea is that every Byzantine general, responsible for their own chain, sorts messages as they come in to establish truth. In Ripple the generals \(validators\) are pre-selected by the Ripple foundation. In Stellar, anyone can be a validator so you choose which validators to trust.

### Used in

* Stellar - similar to Ripple but with key difference - quorum slice. [link1](https://www.stellar.org/papers/stellar-consensus-protocol.pdf) - [link2](https://www.stellar.org/stories/adventures-in-galactic-consensus-chapter-1/) - [link3](https://medium.com/a-stellar-journey/on-worldwide-consensus-359e9eb3e949)
* Ripple
  * Each node receives transaction from external applications 
  * Each Node forms public list of all valid \(not included into last ledger \(=block\)\) transactions aka \(Candidate Set\) 
  * Nodes merge its candidate set with UNLs\(Unique Node List\) candidate sets and vote on the veracity of all transactions \(1st round of consensus\) 
  * all transactions that received at least 50% votes are passed on the next round \(many rounds may take place\) 
  * final round of consensus requires that min 80% of Nodes UNL agreeing on transactions. It means that at least 80% of Validating nodes should have same Candidate SET of transactions 
  * after that each Validating node computes a new ledger \(=block\) with all transactions \(with 80% UNL agreement\) and calculate ledger hash, signs and broadcasts 
  * All Validating nodes compare their ledgers hash 
  * Nodes of the network recognize a ledger instance as validated when a 80% of the peers have signed and broadcast the same validation hash. 
  * Process repeats. Ledger creation process lasts 5 sec\(?\). 

    Each transaction includes transaction fee \(min 0,00001 XRP\) which is destroyed. No block rewards.  

    [whitepaper](https://ripple.com/files/ripple_consensus_whitepaper.pdf)

### pros

* High throughput, 
* low transaction cost, 
* network scalability

  **Read more**

  Stellar Whitepaper [https://www.stellar.org/papers/stellar-consensus-protocol.pdf](https://www.stellar.org/papers/stellar-consensus-protocol.pdf)

## Practical Byzantine Fault Tolerance

PBFT works in asynchronous environments like the Internet and incorporates several important optimizations that improve the response time of previous algorithms by more than an order of magnitude.

### Used in

Hyperledger Fabric

### pros

* High transaction throughput

  **Cons**

  Centralized/permissioned

  **Read more**

* [whitepaper](http://pmg.csail.mit.edu/papers/osdi99.pdf)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Delegated Byzantine Fault Tolerance

The dBFT is called the Delegated Byzantine Fault Tolerant, a Byzantine fault-tolerant consensus mechanism that enables large-scale participation in consensus through proxy voting. The holder of the NEO token can, by voting, pick the bookkeeper it supports. The selected group of bookkeepers, through BFT algorithm, reach a consensus and generate new blocks. Voting in the NEO network continues in real time, rather than in accordance with a fixed term.

### sed in

* Neo
* ByteBall  only verified nodes are allowed to be Validation nodes \([list of requirements](https://github.com/byteball/byteball-witness)\). Users choose in transaction set of 12 Validating nodes. Validating nodes\(Witnesses\) receive transaction fees. [Whitepaper](https://byteball.org/Byteball.pdf)

### Read more

* [Neo implementation](https://github.com/neo-project/docs/blob/master/en-us/index.md#neo-technology-implementation)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Byzantine Fault Tolerance \(BFT\)

The classical problem in distributed computing that is usually explained with Byzantine generals.

### Used in

* [Hyperledger](https://www.hyperledger.org)
* [Dispatch](https://t.me/dispatchlabs)
* [Ripple](https://ripple.com)

  **Pros**

* High throughput; low cost; scalable

  **COns**

* Semi-trusted

  **Read more**

* [whitepaper](https://web.archive.org/web/20170205142845)
* [whitepaper](http://lamport.azurewebsites.net/pubs/byz.pdf)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Proof of Devotion

Similar to POI, the PoD selects the accounts with high influence. All accounts are ranked according to their liquidity and propagation \(Nebulas Rank\).

### Algorithm

* Top-ranked accounts are selected 
* Chosen accounts pay deposit and are qualified as the blocks Validators \(Validators Set is dynamic, changes in Set may occur after Epoch change.\)
* Algorithm pseudo-randomly chooses block Proposer 
* After a new block is proposed, Validators Set \(each Validator is charged a deposit\) participate in a round of BFT-Style voting to verify block \(1. Prepare stage -&gt; 2. Commit Stage. Validators should have &gt; 2/3 of total deposits to validate Block\) 
* Block is added. Block rewards : each Validator rewarded with 1 NAS.

### Used in

* Nebula
  * [whitepaper](https://nebulas.io/docs/NebulasTechnicalWhitepaper.pdf)
  * [Github](https://github.com/nebulasio/wiki/wiki)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Magi's proof-of-work \(mPoW\)

The magi's proof-of-work \(PoW\) protocol, in addition to required computational works to be done to deter denial of service attacks, is also a network-dependent rewarding model system. The mPoW rewards participants who solve complicated cryptographical questions not only to validate transactions but also to create new blocks and generate coins. The amout of coins generated are constantly monitored by the mPoW protocol and tuned on the basis of an attraction-repulsion model: 1\) incremental rewarding to stimulate network activities during passive mining phase, and 2\) decremental rewarding to mitigate redundant mining sources during agressive mining phase. mPoW can effectively govern the magi's network and limit it under a certain scale, enabling the general devices to be capable of mining magi.

### Used in

* [MAGI](https://www.m-core.org)

  **Read more**

* [whitepaper](https://arxiv.org/abs/1409.7948)

[&gt;&gt; Go to Index &lt;&lt;](./#index)

## Magi's proof-of-stake \(mPoS\)

Aims to achieve distributed consensus through operations in addition to mPoW. mPoS is designed such that it rejects potential attacks through accumulating a large amount of coins or offline staking time, either of which leads to security concerns. Similar to mPoW's operation, mPoS is constructed in accordance with the concept of the attraction-repulsion model. Magi hybridizes mPoW with mPoS, and integrate both consensus approaches in order to acquire benefits from the two mechanisms and create a more robust payment system.

### Used in

* [MAGI](https://www.m-core.org)

  **Read more**

* [Bitcointalk](https://bitcointalk.org/index.php?topic=735170.msg9991269#msg9991269)

## Common Attacks

### 51% attack

In PoS, you would need a majority of all minted coins to conduct such an attack, In PoW, you would need a majority of amining power to conduct such an attack,

### transaction censoring.

With PoW, a block miner can “choose” not to mine a block containing certain addresses, thereby censoring that address from the network.

