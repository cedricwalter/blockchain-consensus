# Proof-of-Activity

Combine Proof of Work component with a Proof of Stake. mining first begins in the traditional manner, with miners vying to be the first to solve a puzzle and claim their reward. The difference is that the blocks being mined do not contain transactions. They are simply templates with header information and the mining reward address. Once this nearly blank block is mined, the system switches to a proof of stake protocol. The header information is used to select a random group of validators to sign the block. These are coin holders \(stakeholders\) and the larger the stake a validator holds, the greater the chance they will be selected to sign the new block. Once all the chosen validators sign the block it becomes an actual part of the blockchain. If the block remains unsigned by some of the chosen validators after a given time, it is discarded as incomplete and the next winning block is used. Validators are once again chosen and this continues until a winning block is signed by all the chosen validators. The network fees are split between the winning miner and the validators who signed the block.

## Used in

* [Decred](https://www.decred.org)
  * Blocks are created about every 5 minutes. 
  * Nodes in the network looking for a solution with a known difficulty to create a block \(PoW\). 
  * Once the solution is found it is broadcast to the network. 
  * The network then verifies the solution. 
  * Stakeholders who have locked some DCR in return for a ticket \(1 ticket = ability to cast 1 vote. Stakeholders must wait an average of 28 days \(8,192 blocks\) to vote their tickets\) now have the chance to vote on the block \(PoS\). 
  * 5 tickets are chosen pseudo-randomly from the ticket pool and if at least 3 of 5 vote ‘yes’ the block is permanently added to the blockchain. 
  * Both miners and voters are compensated with DCR : PoS - 30% and PoW - 60% of about 30 new Decred issued with a block.  
* Espers
* [Coinbureau](https://www.coinbureau.com/blockchain/proof-of-activity-explained-hybrid-consensus-algorithm)

## Read more

* [Research Paper](https://eprint.iacr.org/2014/452.pdf)

