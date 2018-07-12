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


# Hybrid Proof of Work (HPoW)
 HPoW still uses PoW but modifies it so it isn’t profitable and, as a result, creates an entire cryptocurrency network that can run on energy efficient, easy to set-up, low-cost computers or cloud services. HPoW removes the profit incentive for miners because the mining reward is so low. In fact, mining farms would actually lose money if they tried to mine Lynx, meaning they will leave Lynx to the individuals who want to solve the sustainability problem. This takes control away from mining farms and pools and puts it squarely into the hands of individuals (solo miners) who want to build upon and use Lynx. HPoW supports network maintenance by incentivizing and empowering those who want to use Lynx. With every new solo miner that connects, the network becomes more secure by reducing the risks associated with a centralized and hierarchical cryptocurrency network. This security is achieved through redundancy: the more individual nodes on the network, the stronger the network becomes. If an individual node or miner fails, or if an entire region of nodes fail due to widespread power outages or war, the network is still secure because mining rigs are plentiful.

Taken together, the three business rules result in “Hybrid Proof of Work” (HPoW)
1. A single miner can’t win a block more than once every 30 minutes.
2. The miner’s reward address balance must be greater than or equal to a required
fluctuating minimum amount of Lynx to win a block.
3. By using random selection, the fastest miners are not always guaranteed to win the block reward.

## Used in
Lynx https://getlynx.io/

## Pros
mining unprofitable

## Cons

## Read more
https://consensus.tokens-economy.com/glossary.html#index

# Delegated proof-of-stake (DPoS)
 DPoS is a twist on Proof of Stake consensus that relies upon a group of delegates to validate blocks on behalf of all nodes in the network. Works using witnesses, who generate blocks. Witnesses are elected by stakeholders at a rate of one vote per share per witness. However, with PoA, the appointment of an authority is automatic, meaning that there can be no bias or uneven process caused by unequal stakes. Coin age is irrelevant. All coins that are mature will add the same staking weight (usually 1 in the wallet hover display). Results in stable, consistent interest only for active wallets and only with small inputs. Downtime and large inputs will significantly impact your interest with DPOS. On the plus side, no age means that moving coins is less costly because lost coin age is not detrimental.

With DPoS blockchain consensus protocols, coin holders use their coin balances to elect delegates, called witnesses. These witnesses have the opportunity to stake blocks of new transactions and add them to the blockchain. Voting power is determined by cyberwealth. Those who have more coins or tokens will have a greater impact on the network that those with fewer.

## Used in
Steemit https://steemit.com/@zanewithspoon
EOS https://eos.io/
BitShares https://bitshares.org/

## Pros
* Cheap transactions
* scalable
* energy efficient
* Coin age is irrelevant: no age means that moving coins is less costly because lost coin age is not detrimental.
* All coins that are mature will add the same staking weight (usually 1 in the wallet hover display).
* Results in stable, consistent interest only for active wallets and only with small inputs.
* Downtime and large inputs will significantly impact your interest with DPOS.
## Cons
* Partially centralized

## Read more
* Wikipedia https://en.wikipedia.org/wiki/Delegated_proof-of-stake

# Leased Proof-of-Stake (LPoS)
Your chances to find a new block only depend on how many Token you have ( i.e. your stake).

## Used in
* NXT
* Waves

## Pros
you don’t need a lot of computing power to forge a new block

## Read more
Medium1 https://medium.com/@wavesgo/explaining-waves-lpos-3a9f838cf167
Medium2 https://blog.wavesplatform.com/waves-launches-balance-leasing-in-lite-client-14db9eac0377

# Proof-of-Stake-Time (PoST)
A time-accepted periodic proof factor in a nonlinear distributed consensus. Stake-Time as “The coin-age of a transaction or set of transactions in which the Stake-Time is the product of the total coins (C) and the fraction (f) of acceptable age(a)

introducing a nonlinear proof function that defines a fraction of time active and idle, at a given block. Idle-time is defined as the fraction of age that no longer supports the distribution of consensus and instead begins to degrade it. This quantified idle-time is unique to each stake, as It decreases the probability to meet the proof and impacts the fraction of earnable matured interest via consensus. Where the fraction of accepted age (f) is equal to the squared cosine of the product of π and that transactions consensus power (p), defined as the fraction coin-age (g) of the average network wide stake-time weight (n) over 60 blocks (1 hour) [figure 1]. If the consensus-power (p) is greater than 0.45 all age is lost and the Time-active fraction is equal to the minimum stake time (m) of 8 hours

## Used in
* PostCoin
* Vericoin

## Pros
* maintains the efficiencies of Proof-of-Stake

## Read more
https://vericoin.info/
Whitepaper
