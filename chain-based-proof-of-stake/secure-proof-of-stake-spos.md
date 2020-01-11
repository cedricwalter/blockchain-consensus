# Secure Proof of Stake \(SPoS\)

Elrond has proposed a novel approach to consensus called “**Secure Proof of Stake**” which eliminates PoW computational waste, and combines eligibility through **stake** and rating with random validator selection, and an optimal dimension for the consensus group.

Elrond’s approach to consensus is made by combining random validators’ selection, eligibility through stake and rating, with an optimal dimension for the consensus group.

### Algorithm

1. Each node ni is defined as a tuple of public key \(P k\), rating \(default is 0\) and the locked stake. If ni wishes to participate in the consensus, it has to first register through a smart contract, by sending a transaction that contains an amount equal to the minimum required stake and other information \(P ks, a public key derived from P k and nodeid that will be used for the signing process in order not to use a real wallet address\). 
2. The node ni joins the node pool and waits for the shard assignment at the end of the current epoch e. The shard assignment mechanism creates a new set of nodes containing all the nodes that joined in epoch e and all the nodes that need to be reshuffled \(less than 1 3 of every shard\). All nodes in this set will be reassigned to the waiting lists of shards. Wj represents j’s shard waiting list and Nsh represents the number of shards. A node also has a secret key sk that by nature is not to be made public.
3. At the end of the epoch in which it has joined, the node will be moved to the list of eligible nodes \(Ej \) of a shard j, where e is the current epoch.
4. Each node from the list Ej can be selected as part of an optimally dimensioned consensus group \(in terms of security and communication\), by a deterministic function, based on the randomness source added to the previous block, the round r and a set of variation parameters. The random number, known to all shard nodes through gossip, cannot be predicted before the block is actually signed by the previous consensus group. This property makes it a good source of randomness and prevents highly adaptive malicious attacks. We define a selection function to return the set of chosen nodes \(consensus group\) Nchosen with the first being the block proposer, that takes following parameters: E, r and sigr−1 - the previous block signature
5. The block will be created by the block proposer and the validators will co-sign it based on a modified practical Byzantine Fault Tolerance \(pBFT\).
6. If, for any reason, the block proposer did not create a block during its allocated time slot \(malicious, offline, etc.\), round r will be used together with the randomness source from the last block to select a new consensus group.

### Advantages

* Effectively partitioning the blockchain and account state into multiple shards, handled in parallel by different participating validators
* An improved variation of Proof of Stake \(PoS\)

### Used in 

* [https://elrond.com/technology/](https://elrond.com/technology/)

### Whitepaper

* [https://elrond.com/assets/files/elrond-whitepaper.pdf](https://elrond.com/assets/files/elrond-whitepaper.pdf)

