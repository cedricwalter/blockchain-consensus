# blockchain-consensus
This is my attempt to list all possible blockchain consensus out there, i welcome pull request of the blockchain community! lets make it the main reference for blockchain consensus

At the core of the Blockchain disruption are consensus algorithm:

Consensus algorithms enable network participants to agree on the contents of a blockchain in a distributed and trust-less manner.

And the consensus algorithm plays a crucial role in maintaining the safety and efficiency of blockchain. Using the right algorithm may bring a significant increase to the performance of blockchain application.

The trilemma claims that blockchain systems can only at most have two of the following three properties:
Decentralization (defined as the system being able to run in a scenario where each participant only has access to O(c) resources, i.e. a regular laptop or small VPS)
Scalability (defined as being able to process O(n) > O(c) transactions)
Security (defined as being secure against attackers with up to O(n) resources)
Each consensus algorithm has its own application scenario. There is no absolute good or bad. The choice of which consensus to use for implementing the blockchain depends on the type of network and data.

# Proof of Work (PoW)
Bitcoin, which made the blockchain technology popular, developed the so-called Proof of Work (PoW) algorithm. In principle, each participant on the Bitcoin network can participate in the block generation. In order to confirm the transaction and enter a block into the blockchain, a miner has to provide an answer, or a proof, to a specific challenge. Miners use PoW to validate transactions and mining new coins, but its main goal is to block potential cyber-attacks or suspicious activities within the network. Each time a miner confirms a transaction, he is rewarded with Bitcoin(s). The disadvantage of this algorithm is that it consumes large quantities of electricity.

1. Transactions are bundled together in form of blocks.
2. Miners verify the transactions within the blocks as legitimate.
3. Miners then solve a mathematical problem known as the proof-of-work problem.
4. A reward is then given to the first person to solve the problem.
5. Verified transactions are stored in the public blockchain.

## Pros
* Oldest and safest
* Transaction fees not mandatory

## Cons
* Energy intensive
* vulnerable to 51% attack
Reducing block rewards

### Read more
https://en.wikipedia.org/wiki/Proof-of-work_system

# Proof of stake (PoS)
Proof of stake (PoS) is a type of algorithm by which a cryptocurrency blockchain network aims to achieve distributed consensus. Coin age is used in the calculation for both stake weight AND the staking reward. Staking reward is set by the coin's APR. The effect is a stable, consistent interest for all staking wallets, regardless of input size or reasonable downtime.

Coin age is used in the calculation for both stake weight AND the staking reward. Staking reward is set by the coin's APR. The effect is a stable, consistent interest for all staking wallets, regardless of input size or reasonable downtime.

## Used in
* Ada
* EOS.IO
* Gridcoin
* Nxt
* Waves

## Pros
Cost efficient: speed, energy, hardware

## Cons
* Economic inequality, rich get richer.

## Read more
https://en.wikipedia.org/wiki/Proof-of-stake

