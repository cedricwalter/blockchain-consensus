# Proof-of-Elapsed-Time \(PoET\)

PoET is a consensus mechanism algorithm that is often used on the permissioned blockchain networks to decide the mining rights or the block winners on the network. Permissioned blockchain networks are those which require any prospective participant to identify themselves before they are allowed to join. Based on the principle of a fair lottery system where every single node is equally likely to be a winner, the PoET mechanism is based on spreading the chances of a winning fairly across the largest possible number of network participants.

The timer is different for each node. Every participant in the network is assigned a random amount of time to wait, and the first participant to finish waiting gets to commit the next block to the blockchain. Similar to pulling straws, but this time, the shortest stem in the stack wins the lottery.

## Used in

* **Resource-Efﬁcient Mining** \(REM\) provides an economic analysis to show that a miner’s revenue source originates from useful work, and not farming chips.
* [Hyperledger Sawtooth](https://sawtooth.hyperledger.org) Solve BFT Validating Nodes limitation and required intel’s SGX. PoET uses a random leader election model or a lottery based election model based on SGX, where the protocol randomly selects the next leader to finalize the block. Every validator requests a wait time from an enclave \(a trusted function\). 
  * The validator with the shortest wait time for a particular transaction block is elected the leader. 
  * The BlockPublisher is responsible for creating candidate blocks to extend the current chain. He takes direction from the consensus algorithm for when to create a block and when to publish a block. He creates, Finalizes, Signs Block and broadcast it 
  * Block Validators check block 
  * Block is created on top of blockchain.

## Pros

* Node will rest, so more energy efficient

  **Cons**

* Trust Intel, require dedicated hardware

  **Read more**

## Attacks and Mitigation

Breaking a single piece of trusted hardware enables the attacker to always win the lottery. Both Sawtooth and REM argue that a statistical analysis of newly minted blocks sufﬁces to detect whether a chip can be compromised. Second, the stale chip problem highlights that it is advantageous to collect chips as this increases the probability of minting a new block \(i.e., every new chips is an additional lottery ticket\). 



