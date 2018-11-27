# Proof of Work \(PoW\)



PoW was originally invented as a means to combat spam \(see [hashcash](https://en.wikipedia.org/wiki/Hashcash)\)if you make it computationally expensive to send email then spamming would be cost prohibitive while still being almost free for a normal user to send email.

Bitcoin, which made the blockchain technology popular, developed the so-called Proof of Work \(PoW\) algorithm. In principle, each participant on the Bitcoin network can participate in the block generation. In order to confirm the transaction and enter a block into the blockchain, a miner has to provide an answer, or a proof, to a specific challenge. Miners use PoW to validate transactions and mining new coins, but its main goal is to block potential cyber-attacks or suspicious activities within the network.

#### Miners

In cryptocurrency networks, “miners” are special nodes that perform the PoW calculation on a set of transactions plus the hash of the previous block to generate the next block in the blockchain. Since the block contains the hash of the previous block, changing a historical block would require regenerating all of the subsequent blocks. Regenerating all the hashes would be computationally intensive and would require a lot of energy – and energy isn’t free. It would also be time consuming. The process of proving work and generating blocks is called ”mining”. Miners are rewarded for this work with newly minted coins adding to the total supply.

**Nodes**

Nakamoto consensus to determine the next head block; that is, at its core:

"Nodes always consider the longest chain to be the correct one and will keep working on extending it. If two nodes broadcast different versions of the next block simultaneously, some nodes may receive one or the other first. In that case, they work on the first one they received, but save the other branch in case it becomes longer. The tie will be broken when the next proof-of-work is found and one branch becomes longer; the nodes that were working on the other branch will then switch to the longer one."

#### algorithm

1. Transactions are bundled together in form of blocks.
2. Miners verify the transactions within the blocks as legitimate.
3. Miners then solve a mathematical problem known as the proof-of-work problem.
4. A reward is then given to the first person to solve the problem.
5. Verified transactions are stored in the public blockchain.

#### attacks

* With a PoW coin the miners don't need to own an investment in the coin that they are attacking, so there might be an incentive for them to run a 51% attack.

#### Pros

* Oldest and safest
* Transaction fees not mandatory
* Easy to verify solutions
* Hard to find solutions
* Difficulty of finding solutions can be precisely quantified
* Provably inseparable from the block it secures

#### Cons

* Poor performance
* PoW uses an enormous amount of computing power, which, in itself lowers incentive
* It is also vulnerable to attack, as a potential attacker would only need to have 51% of the mining resources \(hashrate\) to control a network, although this is not easy to do.
* Reducing block rewards
* Proof of Work restricts the inputs to the structure of given blockchains mining algorithm. In Bitcoin’s case this would have to be a nonce, and in Ethereum’s case the input must be a random integer, a nonce, and a seed hash of the block.

**Read more**

* [https://en.wikipedia.org/wiki/Proof-of-work\_system](https://en.wikipedia.org/wiki/Proof-of-work_system)
* "Proof-of-work": [Pricing via processing or combatting junk mail](https://web.cs.dal.ca/~abrodsky/7301/readings/DwNa93.pdf). Dwork C, Naor M. '92.
* [Hashcash - A Denial of Service Counter-Measure](http://www.hashcash.org/papers/hashcash.pdf). Back A. '02.
* [Cuckoo Cycle: a memory bound graph-theoretic proof-of-work](http://fc15.ifca.ai/preproceedings/bitcoin/paper_12.pdf). Tromp J. FC '15.
* [PieceWork: Generalized Outsourcing Control for Proofs of Work](http://fc17.ifca.ai/bitcoin/papers/bitcoin17-final24.pdf). Daian P, Eyal I, Juels A, Sirer EG. FC '17.
* [Permacoin: Repurposing bitcoin work for data preservation](http://ieeexplore.ieee.org/iel7/6954656/6956545/06956582.pdf). Miller A, Juels A, Shi E, Parno B, Katz J. Permacoin. S&P '14.

