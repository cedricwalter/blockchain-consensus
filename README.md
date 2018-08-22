![Logo](https://www.tokens-economy.com/wp-content/uploads/2018/06/logo.png)

# Blockchain Consensus Encyclopedia

More than 56 Blockchain Consensus described.

# Index
  * [Introduction](#introduction)
  * [Blockchain Consensus?](#blockchain-consensus)
- [Avalanche](#avalanche)
- [Proof of Work (PoW)](#proof-of-work-pow)
- [Proof of Meaningful Work (PoMW)](#proof-of-meaningful-work-pomw)
- [Proof of stake (PoS)](#proof-of-stake-pos)
- [Hybrid Proof of Work (HPoW)](#hybrid-proof-of-work-hpow)
- [Delegated proof-of-stake (DPoS)](#delegated-proof-of-stake-dpos)
- [Leased Proof-of-Stake (LPoS)](#leased-proof-of-stake-lpos)
- [Proof-of-Stake-Time (PoST)](#proof-of-stake-time-post)
- [Traditional Proof of stake / Tiered Proof Of Stake (TPOS)](#traditional-proof-of-stake---tiered-proof-of-stake-tpos)
- [High Interest Proof of Stake (HiPoS)](#high-interest-proof-of-stake-hipos)
- [Proof of Identity (PoI)](#proof-of-identity-poi)
- [Proof-of-authority (PoA)](#proof-of-authority-poa)
- [Ethereum Proof of Authority](#ethereum-proof-of-authority)  
- [Proof of Ownership](#proof-of-ownership)
- [Proof-of-space (PoC)](#proof-of-space-poc)
- [Proof-of-Signature (PoSign)](#proof-of-signature--posign)
- [Proof of Time](#proof-of-time)
- [Proof of Existence](#proof-of-existence)
- [Ouroboros](#ouroboros)
- [Proof of Retrievability (POR)](#proof-of-retrievability-por)
- [Limited Confidence Proof-of-Activity](#limited-confidence-proof-of-activity)
- [Proof-of-Proof (PoP)](#proof-of-proof-pop)
- [Proof of Processed Payments (PoPP)](#proof-of-processed-payments-popp)
- [Scrypt-adaptive-N (ASIC resistant)](#scrypt-adaptive-n--asic-resistant)
- [Proof of Reputation (PoR)](#proof-of-reputation-por)
- [Proof of Research (DPoR)](#proof-of-research-dpor)
- [Proof of Burn (PoB)](#proof-of-burn-pob)
- [Proof-of-Weight (PoWeight)](#proof-of-weight-poweight)
- [Proof of Zero (PoZ)](#proof-of-zero-poz)
- [Raft](#raft)
- [PoET](#poet)
- [Proof of History](#proof-of-history)
- [Proof of Stake Velocity](#proof-of-stake-velocity)
- [Proof of Importance](#proof-of-importance)
- [Proof of Participation (PoP)](#proof-of-participation-pop)
- [Proof Of Activity](#proof-of-activity)
- [Proof of Believability](#proof-of-believability)
- [Proof of Care (PoC)](#proof-of-care-poc)
- [Proof of Value (PoV)](#proof-of-value-pov)
- [Proof of Quality (PoQ)](#proof-of-quality-poq)
- [Variable Delayed Proof Of Stake (vDPOS)](#variable-delayed-proof-of-stake-vdpos)
- [Proof-of-work time (PoWT)](#proof-of-work-time-powt)
- [Serialization of Proof-of-work Events: Confirming Transactions via Recursive Elections](#serialization-of-proof-of-work-events--confirming-transactions-via-recursive-elections)
- [Proof-of-work (PoW) / High Interest Proof of Stake (HiPoS)](#proof-of-work--pow----high-interest-proof-of-stake-hipos)
- [Proof of Work (PoW) / Nexus Proof of State (nPoS) or Nexus Proof of Holding (nPOH)](#proof-of-work--pow----nexus-proof-of-state--npos--or-nexus-proof-of-holding-npoh)
- [Delayed Proof of Work (dPoW)](#delayed-proof-of-work-dpow)
- [Proof of Work (PoW) / PoM / PoSII](#proof-of-work-pow-pom-posii)
- [Proof of Work (PoW) / Proof of Stake (PoS) / Proof Of Care (PoC)](#proof-of-work--pow----proof-of-stake--pos----proof-of-care-poc)
- [Proof of Stake (PoS) / Proof of Disintegration (PoD)](#proof-of-stake--pos----proof-of-disintegration--pod-)
- [Proof-of-Stake (POS) / Proof-of-Presence (PoP)](#proof-of-stake--pos----proof-of-presence-pop)
- [Leasing Proof of Stake (PoS/LPoS)](#leasing-proof-of-stake--pos-lpos)
- [Direct Acyclic Graph](#direct-acyclic-graph)
- [Tangle (DAG)](#tangle-dag)
- [Block-lattice - Directed Acyclic Graphs (DAGs)](#block-lattice---directed-acyclic-graphs-dags)
- [LFT](#lft)
- [Modified Federated Byzantine Agreement (mFBA)](#modified-federated-byzantine-agreement-mfba)
- [Federated Byzantine Agreement](#federated-byzantine-agreement)
- [Practical Byzantine Fault Tolerance](#practical-byzantine-fault-tolerance)
- [Delegated Byzantine Fault Tolerance](#delegated-byzantine-fault-tolerance)
- [Byzantine Fault Tolerance (BFT)](#byzantine-fault-tolerance-bft)
- [Magi's proof-of-work (mPoW)](#magi-s-proof-of-work-mpow)
- [Magi's proof-of-stake (mPoS)](#magi-s-proof-of-stake-mpos)

## Introduction
This is my attempt to list all possible blockchain consensus out there, i welcome pull request of the blockchain community! lets make it the main reference for blockchain consensus

## Blockchain Consensus?
At the core of the Blockchain disruption are consensus algorithm:

> Consensus algorithms enable network participants to agree on the contents of a blockchain in a distributed and trust-less manner.

> “Consensus decision-making is a group decision-making process in which group members develop, and agree to support a decision in the best interest of the whole. Consensus may be defined professionally as an acceptable resolution, one that can be supported, even if not the “favourite” of each individual. Consensus is defined by Merriam-Webster as, first, general agreement, and second, group solidarity of belief or sentiment.” Wikipedia


And the consensus algorithm plays a crucial role in maintaining the safety and efficiency of blockchain. Using the right algorithm may bring a significant increase to the performance of blockchain application.

The trilemma claims that blockchain systems can only at most have two of the following three properties:
1. Decentralization (defined as the system being able to run in a scenario where each participant only has access to O(c) resources, i.e. a regular laptop or small VPS)
2. Scalability (defined as being able to process O(n) > O(c) transactions)
3. Security (defined as being secure against attackers with up to O(n) resources)

Each consensus algorithm has its own application scenario. There is no absolute good or bad. The choice of which consensus to use for implementing the blockchain depends on the type of network and data.

For a transaction to be valid on most cryptocurrency networks, the transaction needs to collect a certain number of confirmations (often equals to an inclusion in a block of a blockchain) from the network. E.g 10 confirmations means to see a specific transaction in one block and 9 consecutive blocks.

# Table of contents

# Avalanche
The core idea of Avalanche is metastability.

## Pros
* Quick finality and low latency
* Higher throughput: 1000–10,000 transactions per second.
* Robust: The network does not need to agree on who the participants are to achieve undeniable consensus.
* No miners

## Cons

### Read more
* [Snowflake to Avalanche: A Novel Metastable Consensus Protocol Family for Cryptocurrencies](https://ipfs.io/ipfs/QmUy4jh5mGNZvLkjies1RWM4YuvJh5o2FYopNPVYwrRVGV)
* [demystifying-snowflake-to-avalanche](https://medium.com/zkcapital/demystifying-snowflake-to-avalanche-966f56c33fd7)

# Proof of Work (PoW)
PoW was originally invented as a means to combat spam (see [hashcash](https://en.wikipedia.org/wiki/Hashcash))if you make it computationally expensive to send email then spamming would be cost
prohibitive while still being almost free for a normal user to send email. 

Bitcoin, which made the blockchain technology popular, developed the so-called Proof of Work (PoW) algorithm. In principle, each participant on the Bitcoin network can participate in the block generation. In order to confirm the transaction and enter a block into the blockchain, a miner has to provide an answer, or a proof, to a specific challenge. Miners use PoW to validate transactions and mining new coins, but its main goal is to block potential cyber-attacks or suspicious activities within the network. 

## Miners
In cryptocurrency networks, “miners” are special nodes that perform the PoW calculation on a set of transactions plus the hash of the previous block to generate the next block in the blockchain. Since the block contains the hash of the previous block, changing a historical block would require regenerating all of the subsequent blocks. Regenerating all the hashes would be computationally intensive and would require a lot of energy – and energy isn’t free. It would also be time consuming. The process of proving work and generating blocks is called ”mining”. Miners are rewarded for this work with newly minted coins adding to the total supply.

## algorithm
1. Transactions are bundled together in form of blocks.
2. Miners verify the transactions within the blocks as legitimate.
3. Miners then solve a mathematical problem known as the proof-of-work problem.
4. A reward is then given to the first person to solve the problem.
5. Verified transactions are stored in the public blockchain.

## attacks
* With a PoW coin the miners don't need to own an investment in the coin that they are attacking, so there might be an incentive for them to run a 51% attack.

## Pros
* Oldest and safest
* Transaction fees not mandatory
* Easy to verify solutions
* Hard to find solutions
* Difficulty of finding solutions can be precisely quantified
* Provably inseparable from the block it secures

## Cons
* Poor performance
* PoW uses an enormous amount of computing power, which, in itself lowers incentive
* It is also vulnerable to attack, as a potential attacker would only need to have 51% of the mining resources (hashrate) to control a network, although this is not easy to do.
* Reducing block rewards

### Read more
- https://en.wikipedia.org/wiki/Proof-of-work_system
- "Proof-of-work": [Pricing via processing or combatting junk mail](https://web.cs.dal.ca/~abrodsky/7301/readings/DwNa93.pdf). Dwork C, Naor M. '92.
- [Hashcash - A Denial of Service Counter-Measure](http://www.hashcash.org/papers/hashcash.pdf). Back A. '02.
- [Cuckoo Cycle: a memory bound graph-theoretic proof-of-work](http://fc15.ifca.ai/preproceedings/bitcoin/paper_12.pdf). Tromp J. FC '15.
- [PieceWork: Generalized Outsourcing Control for Proofs of Work](http://fc17.ifca.ai/bitcoin/papers/bitcoin17-final24.pdf). Daian P, Eyal I, Juels A, Sirer EG. FC '17.
- [Permacoin: Repurposing bitcoin work for data preservation](http://ieeexplore.ieee.org/iel7/6954656/6956545/06956582.pdf). Miller A, Juels A, Shi E, Parno B, Katz J. Permacoin. S&P '14.

[Go to Index](#index)

# Proof of Meaningful Work (PoMW)
While the basic idea, to protect the Blockchain by proving that a certain amount of computation was invested to create every single block, is worth being preserved, the current implementation, using purely artificial computational tasks (hashing), with the sole goal of burning “enough” energy, is much too wasteful to be used productively1 and scales
very badly. Proof of Meaningful Work keep the good idea, but implement it using meaningful computation tasks, so that the energy invested in the proof of the miners’ computational strength is used for calculations that support public scientific research projects (e.g. medical research for cures, chemical research, astrophysical simulations).

Here below combined with PoS so the ratio of PoS to PoMW can be adjusted continuously according to the momentary load
situation.

![ProofOfMeaningfulWorkWithPoS.png](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/ProofOfMeaningfulWorkWithPoS.png)

## Pros
* Decrease wasted energy. The needed energy will be used for socially responsible projects in the fields of healthcare, science, ecological protection and more.

## Cons
* attack of more than 50% of the total computing power

## Read more
* [Vrenelium](www.vrenelium.ch)

[Go to Index](#index)

# Proof of stake (PoS)
The proof-of-stake (PoS) mechanism works using an algorithm that selects participants with the highest stakes as validators, assuming that the highest stakeholders are incentivized to ensure a transaction is processed. 
The idea is that those with the most coins in circulation have the most to lose so they are positioned to work in the interest of the network. The amount of coins that a network may require changes just like the difficulty in PoW.

## Coin age
To distinguish between users who have just obtained their coins and users who have been holding their coins for a period of time, proof-of-stake algorithms use the idea of coin age.

Coin age is used in the calculation for both stake weight AND the staking reward. Staking reward is set by the coin's APR. The effect is a stable, consistent interest for all staking wallets, regardless of input size or reasonable downtime.

The longer a user holds the coins, the higher the changes of winning the right to create a block of the network blockchain and get a reward.

## Incentivizing to stay connected
In order to keep most user active, the reward for the creation of a block increase if there is too many users offline, so there is more  benefits to go online.

## Penalizing offline users
Most if not all PoS algorithm penalize Holders which can stay offline for long periods of time. Otherwise they could get control by connecting back to it and having over 50% of voting power because of the size of their holdings.

## Pseudo anonymous users
Validators within the PoS network are anonymous users who are identified only by their wallet address. This pro-vides no additional accountability over PoW for bad actors who can amass significant wealth on the network.

## Security
The security model is an economic one, based on the “game-theory” assumption that the cost of acquiring the tokens necessary to become a block producer is more than an attacker is willing to bear, that couples the network’s security to the value of its token, ie: the higher the value of the token, the more secure the network becomes.

## nothing-at-stake attack
 Without economic penalties for attackers, the chain can suffer nothing-at-stake attacks where stakers are incentivised to validate all proposed forks to maximise their returns.
![pos-nothing-stake](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/pos-nothing-stake.png)
 
## Algorithm
![Cosmos.network.pos](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/pos-cosmos.network.png)

1. The validators will have to lock up some of their coins as stake.
2. After that, they will start validating the blocks. Meaning, when they discover a block which they think can be added to the chain, they will validate it by placing a bet on it.
3. If the block gets appended, then the validators will get a reward proportional to their bets.

## BlackCoin / Qtum specifics
TODO

## Used in
* Ada
* EOS.IO
* Gridcoin
* Nxt
* Waves
* BlackCoin 
* Qtum 
* In Future with Casper in Ethereum

## Pros
* Cost efficient: speed, energy, hardware
* The more people use the network and have coins, the more secure the network.

## Cons
* Economic inequality, rich get richer.
* Attackers can calculate the probability of winning the reward to create a block of the blockchain based on who has how many coins.
* Initial targets for Ethereum’s Casper implementation are only 100 TPS

## Read more
https://en.wikipedia.org/wiki/Proof-of-stake

[Go to Index](#index)

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

[Go to Index](#index)

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

[Go to Index](#index)

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

[Go to Index](#index)

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
Whitepaper https://vericoin.info/

# Traditional Proof of stake / Tiered Proof Of Stake (TPOS)
TPOS or Traditional Proof of stake is a form of the algorithm through which a cryptocurrency Social Network Blockchain aims to realize distributed agreement. In TPOS-derived currencies, the originator of the next block is selected through different combinations of random collection and the stake.

## Used in
XSN
## Pros
* Payments through processing dealings counts mainly on coin holders instead of on miners.

[Go to Index](#index)

# High Interest Proof of Stake (HiPoS)
Coin age is used in the calculation for stake weight, but not staking reward. Staking reward is fixed per a schedule. Results in stable, consistent interest for staking wallets as long as down time is minimal and inputs are small. Large input size is harshly punished by HiPOS.

hiPOS is High Interest Proof of Stake. Essentially; a POS system that is a fixed reward rather than a percentage yield; which is awarded out based on luck/coin age/coin weight. hiPOS can be viewed as an extension of POW. Where hiPOS blocks equal the output in terms of coin count as POW blocks - in a short period of time. So a hiPOS coin would say have a total 10M coins; 5M of which are POW over a timespan of 60 Days; and the other 5M are hiPOS minted as POS over an additional 60 Days.

## Used in
* Positron(2015)
* BitBean (2015)
* EdgeCoin (EDGE)
* GRAVITYBITS

## Pros
* Great for incentivizing people to hold as developers release more info on their projects
* allow people with smaller holdings to benefit greatly by simply finding a few blocks at the right time.

# Proof of Identity (PoI)
Proof of Identity (PoI) is a cryptographic evidence (piece of data) which tells that any user knows a private key that compares to an authorized identity and cryptographically attached to a specific transaction. Every individual from some group can create a PoF (only a block of data) and present it to anyone for instance to the processing node.

## Used in
NEM

## Read more
Reddit https://www.reddit.com/r/CryptoUBI/comments/2v2gi6/proof_of_identityproof_of_person_the_elephant_in/

[Go to Index](#index)

# Proof-of-authority (PoA)
In PoA-based networks, transactions and blocks are validated by approved accounts, known as validators. alidators run software allowing them to put transactions in blocks. The process is automated and does not require validators to be constantly monitoring their computers. It, however, does require maintaining the computer (the authority node) uncompromised.
With PoA individuals earn the right to become validators, so there is an incentive to retain the position that they have gained. By attaching a reputation to identity, validators are incentivized to uphold the transaction process, as they do not wish to have their identities attached to a negative reputation. 

This is considered more robust than PoS, as:
* In PoS, while a stake between two parties may be even, it does not take into account each party’s total holdings. This means that incentives can be unbalanced.
* PoW uses an enormous amount of computing power, which, in itself lowers incentive

## Establishing authority
The three main conditions that must be fulfilled for a validator to be established are:
1. Identity must be formally verified on-chain, with a possibility to cross-check the information in a publicly available domain
2. Eligibility must be difficult to obtain, to make the right to validate the blocks earned and valued. (Example: potential validators are required to obtain public notary license)
3. There must be complete uniformity in the checks and procedures for establishing an authority

## Used in
* POA.Network https://poa.network/
* Ethereum Kovan https://kovan.etherscan.io/
* testnetRinkeby https://gist.github.com/cryptogoth/10a98e8078cfd69f7ca892ddbdcf26bc

## Pros
* High throughput; scalable
* No mining mechanism like in PoW, PoA uses identity as the sole verification of the authority to validate,
* PoA is suited for both private networks and public networks
* PoA only allows non-consecutive block approval from any one validator, meaning that the risk of serious damage is minimized.
## Cons
* By identifying validators it is a centralized system

## Read more
Wikipedia https://en.wikipedia.org/wiki/Proof-of-authority

[Go to Index](#index)

# Ethereum Proof of Authority
Ethereum Proof-of-Authority on Azure allows enterprises to build applications on an Ethereum blockchain that is not secured by a Proof-of-Work (PoW) consensus algorithm and consequently does not require mining. Since all participants on an enterprise blockchain network are known and reputable, governance can be separated from network operation.
Azure features a built-in decentralized application (DApp or dApp) called the “Governance DApp” that provides consortium members with the authority to govern the network or delegate their voting power to others. Network participants can also delegate other nodes to vote on their behalf in the event that their primary nodes go offline, ensuring that all members maintain continual consensus participation. Network administrators, in turn, can use on-chain voting to vote on and alter network authorities in a transparent and auditable manner.

## Used in
* [Ethereum on Azure](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/microsoft-azure-blockchain.azure-blockchain-ethereum?tab=Overview)

# Proof of Ownership
This technique can be used by artists or businesses to certify the integrity, date of publication and ownership of their creations or contracts. A Proof of Ownership is always attached to a piece of data using cryptographic functions. This makes it impossible to alter the data after certification. If the content is modified, even by a single bit, then the whole certificate becomes invalid.

Only the people with the private key associated with the signature can prove they are the owner.

# Proof-of-space (PoC)
(PoSpace), also called proof-of-capacity (PoC) is a means of showing that one has a legitimate interest in a service (such as sending an email) by allocating a non-trivial amount of memory or disk space to solve a challenge presented by the service provider.

## Used in
* Burstcoin https://hackernoon.com/burst-part-3-proof-of-capacity-the-green-alternative-8e2651211671
* Chia
* SpaceMint

## Pros
* Efficient , cheap, distributed

## Cons

## Read more
Wikipedia https://en.wikipedia.org/wiki/Proof-of-space

[Go to Index](#index)

# Proof-of-Signature (PoSign)
 PROOF-OF-SIGNATURE is a new consensus method (developed by Borzalom) that utilizes a network of registered STATIC nodes. STATIC nodes must be registered and active in order to participate in consensus. STATIC node registration status is verified using Proof-of-Signature, as all node are registered and known

PoSIGN consensus is achieved through the interactions between a system of real and virtual node networks in constant communication, ensuring precise, rapid, signature-verified transactions. Additional benefits achieved by the ZOLT algorithm include substantially decreased energy consumption, as the consensus algorithm does not require nodes to solve computationally difficult problems to earn transaction fees or create new tokens. The STATIC (Services Transactions and Trusted in Control) node network is the bedrock upon which the XTRABYTES platform is built. STATIC nodes provide security, ensure consensus, and play a large and developing future role in XTRABYTES governance. The virtual VITALS network of nodes utilizes a proprietary network protocol in order to create an enclosed, private network by which online STATIC nodes can directly communicate. Lastly, to ensure STATIC nodes are indeed verifying the correct block as the VITALS network maintains consensus, the PULSE network functions as the central communication transmission system, providing time stamps in order to make block verification simpler across the entire STATIC network. Transactions are verified by a network of what are called STATIC nodes—importantly, each of these nodes must sign off on a transaction before the associated block can be appended to the chain. Should a malicious node repeatedly attempt to compromise the chain, it will be blacklisted automatically.

## Used in
* XBY

## Read more
* Reddit https://www.reddit.com/r/CryptoCurrency/comments/7ifzer/understanding_xbys_proofofsignature_posign/
* Whitepaper https://xtrabytes.global/build/files/whitepaper.pdf/

[Go to Index](#index)

# Proof of Time
 ChronoLogic considers time as value. Rather than proof-of-work or proof-of-stake mechanisms, ChronoLogicworks on proof-of-time. In its first use-case ChronoLogic pegs time to a store of value token named DAY based on the Ethereum blockchain. This cryptocurrency enables future value to be independent of third party assets that can be harvested such as electricity & processing power in the case of traditional cryptocurrency mining. The only way additional DAY can be produced is via the passage of time.

The DAY smart contract has advanced minting capabilities and a halving mechanism to limit the total supply of DAY in the future. Every contributor in any phase of the token contribution period will receive a minting address called a TimeMint with a specific minting power called ChronoPower. ChronoPower ranges from 1% to 0.5% minting additional DAY in the respective TimeMint based on the TimeMint’s current balance of DAY. ChronoPower decays linearly among contributors based on their contribution order. The first contributor receives TimeMint0001 with the highest ChronoPower of 1% & the last TimeMint receives the lowest ChronoPower of 0.5%.

## Used in
Chronologic https://chronologic.network/

## Read more
Whitepaper https://chronologic.network/uploads/Chronologic_Whitepaper.pdf

[Go to Index](#index)

# Proof of Existence
Proof of Existence is an online service that verifies the existence of computer files as of a specific time via timestamped transactions in the bitcoin blockchain.

## Used in
* Poex.io
* HeroNode
* DragonChain

## Read more
* Wikipedia https://en.wikipedia.org/wiki/Proof_of_Existence

# Ouroboros
A variation of Proof-of-stake(with rigorous security guarantees) used by Cardano.

## Used in
* Cardano

## Read more
- Whitepaper https://eprint.iacr.org/2016/889.pdf
- [Ouroboros: A provably secure proof-of-stake blockchain protocol](https://pdfs.semanticscholar.org/1c14/549f7ba7d6a000d79a7d12255eb11113e6fa.pdf). Kiayias A, Russell A, David B, Oliynykov R. '16.

[Go to Index](#index)

# Proof of Retrievability (POR)
A proof of Retrievability (POR) is a compact proof by a file system (prover) to a client (verifier) that a target file F is intact, in the sense that the client can fully recover it. As PORs incur lower communication complexity than transmission of F itself, they are an attractive building block for high-assurance remote storage systems. It can be really useful as a consensus algorithm for Cloud computing systems.

Permacoin proposed a modification to Bitcoin that repurposes its mining resources to achieve a more broadly useful goal: distributed storage of archival data. Unlike Bitcoin and its proposed alternatives, Permacoin requires clients to invest not just computational resources, but also storage. This scheme involves an alternative scratch-off puzzle for Bitcoin based on Proofs-of-Retrievability (PORs). Successfully minting money with this SOP requires local, random access to a copy of a file. Given the competition among mining clients in Bitcoin, this modified SOP gives rise to highly decentralized file storage, thus reducing the overall waste of Bitcoin.

## Used in
* Microsoft
* [PermaCoin](https://www.cs.umd.edu/~elaine/docs/permacoin.pdf)

## Read more
* Whitepaper https://eprint.iacr.org/2008/175.pdf

[Go to Index](#index)

# Limited Confidence Proof-of-Activity
Combine Proof of Work component with a Proof of Stake. mining first begins in the traditional manner, with miners vying to be the first to solve a puzzle and claim their reward. The difference is that the blocks being mined do not contain transactions. They are simply templates with header information and the mining reward address. Once this nearly blank block is mined, the system switches to a proof of stake protocol. The header information is used to select a random group of validators to sign the block. These are coin holders (stakeholders) and the larger the stake a validator holds, the greater the chance they will be selected to sign the new block. Once all the chosen validators sign the block it becomes an actual part of the blockchain. If the block remains unsigned by some of the chosen validators after a given time, it is discarded as incomplete and the next winning block is used. Validators are once again chosen and this continues until a winning block is signed by all the chosen validators. The network fees are split between the winning miner and the validators who signed the block.

## Used in
* Decred https://www.decred.org/
* Espers
* Coinbureau https://www.coinbureau.com/blockchain/proof-of-activity-explained-hybrid-consensus-algorithm

## Read more
* Research Paper https://eprint.iacr.org/2014/452.pdf

[Go to Index](#index)

# Proof-of-Proof (PoP)
The Proof of Proof™ consensus protocol enables blockchains to inherit proof-of-work security from other blockchains, creating an ecosystem wherein security originates on established blockchains like Bitcoin and extends to other blockchains. 
The PoP protocol introduces a new type of miner who performs periodic publications of one blockchain’s current state to another blockchain. These publications are referenced in the event of a potential blockchain reorganization. PoP requires a blockchain has some means of creating blocks, such as low-hashrate local PoW, PoS, etc. 

## Used in
* [VeriBlock](https://www.veriblock.org)

## Read more
* [WhitePaper](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/whitepaper/PoP-Whitepaper.pdf)

[Go to Index](#index)

# Proof of Processed Payments (PoPP)
Proof-of-Processed-Payments (PoPP) is how Metal aims to distribute MTL to the masses. Think of it as a human-powered Proof-of-Work (POW), as opposed to a computational-powered PoW, such as the one Bitcoin uses. PoPP acts as a provable way of identifying users and distributing new currency into the system. At the same time, it rewards users who convert fiat currency into cryptocurrency. When a payment is settled, a portion of the gross amount of the payment is returned in MTL. The amount received is up to 5% of the volume of the transaction at trading value for MTL in either direction (sender/receiver). Consider as an example that Alice sends Bob $100 using the Metal Pay app and at the time MTL is trading at $1 per MTL. Following confirmation of a successful transaction, both Alice and Bob would receive $5 in MTL, which in this case would be 5 MTL.

## Used in
metalpay

## Read more
MetalPay https://support.metalpay.com/hc/en-us/articles/115000369474-What-is-PoPP-

[Go to Index](#index)

# Dynamic Proof of Location 
Today’s geolocation tools are great for determining the location of a device, but cannot offer reliable and trusted location verification services. They are uni-directional and unencrypted, which makes it problematic to rely on GPS for smart contracts that need to execute when spatial parameters are met.
Dynamic Proof of Location empowers a permissionless and autonomous network of radio beacons that can offer secure location verification services through time synchronization in a decentralized manner.

## Used in
* [FOAM](https://www.foam.space/)

## Pros
* Trustless: Byzantine fault tolerant clock synchronization
* Independent: Does not rely on GPS
* Open: Anyone can utilize the network or offer utility services
* Accountable: Economics structured to ensure honest behavior, verified with fraud proofs
* Incentivized: Service providers remunerated for extending localization and verification zones

## read more
[FOAM blog](https://blog.foam.space/introduction-to-proof-of-location-6b4c77928022)

[Go to Index](#index)

# Scrypt-adaptive-N (ASIC resistant)
 The idea behind the algorithm is that even if the memory requirements of the Scrypt algorithm used by Litecoin were adjusted, there would always come a time when it would not be high enough to render ASIC development impossible. Since this issue must be dealt with from the start, Scrypt-N is a perfect solution. Scrypt-N relies on the “Adaptive N-Factor” in which N is the memory required to complete new hashing functions.

The idea is that N (memory requirement) will always increase over time, rendering ASIC development unfeasible. A coin with an adaptive 'n' factor usually starts at '11' , and stating it is adaptive that means that over time usually specific to a future unix time stamp it will become '12' , '13'... As it increases the amount of memory necessary to 'mine' the coin increases....quickly.

## Used in
* Vertcoin https://vertcoin.org/
* ExeCoin (EXE)
* GPUcoin (GPUC)
* ParallaxCoin (PLX)
* SiliconValleyCoin (XSV)

[Go to Index](#index)

# Proof of Reputation (PoR)
POR is an upgraded, stronger, and more secure form of Proof of Authority (POA). In POA the transactions and blocks are validated by approved accounts known as validators. POA has typically been used in private networks and most recently a few companies that have adopted it to use individuals as the validators whose identities are publicly disclosed and at stake.

Proof of Reputation (PoR) consensus model depends on the reputation of the participants to keep the network secure. A participant (a block signer) must have a reputation important enough that they would face significant financial and brand consequences if they were to attempt to cheat the system. POR uses companies as validators not individuals. 

Once a company proves reputation and passes verification, they may be voted into the network as an authoritative node and at this point, it operates like a Proof of Authority network (PoA), where only authoritative nodes can sign and validate blocks.

A company caught cheating would not only be risking its reputation. It would be risking its entire market cap and the reputation of
the officers and shareholders of the company. It would have significantly more to lose than any one individual. 

## 
**Authorized Signers** Authorized signers are trusted nodes that create blocks, sign them, and distribute them to
other nodes. A list of authorized signers will be maintained on the blockchain. Only authorized nodes can sign blocks and all blocks are verified that this is true by checking the signer is in the authorized list. The signing algorithm is essentially the same signature algorithm as PoW but with a different set of headers. PoW-specific headers will be removed and additional headers added to
enable voting.
Given N authorized signers, a signer may only sign a block every (N/2) + 1. This ensures that someone would need to control > 50% of signers to perform a malicious attack.
Authorized signers will be rewarded in Coins per block signed.

The consensus protocol ensures fairness and liveness by incentivizing the assigned signer of a block to perform the signing but also allowing other blocks to sign if the assigned signer is unavailable. The assigned signer for a block is determined by a round-robin lookup of the authorized signer list. If the assigned signer doesn’t respond then then other signers can sign at a lower block difficulty level. 

## Pros
* For private, permissioned blockchains.
* Fast since no PoW needed

## Cons
* Only for private, permissioned blockchains.
* Subject to 51% attack like PoW, but more unlikely that spo many entities in the network colludes.

## Used by
* [GoChain](https://gochain.io/) that support smart contracts

## Read more
[Medium](https://medium.com/gochain/proof-of-reputation-e37432420712)

[Go to Index](#index)

# Proof of Research (DPoR)
Each participant helps performing research by computations in Gridcoins network. The network average is similar to difficulty in PoW mining. As the network average rises it becomes harder to get the same magnitude so if you want to keep getting the same reward you would have to add more compute power if we have an environment of a rising network average. If the price rose significantly more compute power would come on board, raising the network average, making it harder to get the same reward, just like difficulty in PoW.

## Used in
Gridcoin https://wiki.gridcoin.us/Proof-of-Research

## Read more
Gridcoin https://wiki.gridcoin.us/Proof-of-Research

[Go to Index](#index)

# Proof of Burn (PoB)
With proof of burn, instead of pouring money into expensive computer equipment, you ‘burn’ coins by sending them to an address where they are irretrievable. By committing your coins to never-never land, you earn a lifetime privilege to mine on the system based on a random selection process.
A user who gives up short term wealth proves that they are following the consensus mechanism and is rewarded with a lifetime privilege to mine the next block on the blockchain. Coins are sent to unspendable address

## Used in
Slimcoin
TGCoin (Third Generation Coin)

## Pros
Keeping coins is not rewarded like in PoS
## Cons
* Burning coins doesnt guarantee that you’re selected to mine future blocks, whales are favored
* security get better with huge market capital (attack costs increase)
* As with PoS, the principle is not suitable for distributing the first coins.

## Read more
* HackerNoon https://hackernoon.com/consensuspedia-an-encyclopedia-of-29-consensus-algorithms-e9c4b4b7d08f
* bitcointalk.org https://bitcointalk.org/index.php?topic=704213.0

[Go to Index](#index)

# Proof-of-Weight (PoWeight)
Proof-of-Weight is a broad classification of consensus algorithms based around the Algorand consensus model. The general idea is that where in PoS, your percentage of tokens owned in the network represents your probability of “discovering” the next block, in a PoWeight system, some other relatively weighted value is used. Concrete example: Filecoin’s Proof-of-Spacetime is weighted on how much IPFS data you’re storing. Other systems could include weights for things like Proof-of-Reputation.

## Used in
* Algorand https://people.csail.mit.edu/nickolai/papers/gilad-algorand-eprint.pdf
* Filecoin https://filecoin.io/
* Chia https://chia.network/

## Pros
* Customizable; scalable
## Cons
* Incentivization can be a challenge
## Read more
- [ALGORAND: The Efficient and Democratic Ledger](https://arxiv.org/pdf/1607.01341.pdf). Micali S. '16.

[Go to Index](#index)

# Proof of Zero (PoZ)
PoZ is an evolution of actual PoS, with the main difference that is capable of Zero-Knowledge transactions. PoZ gives every users the chance of earning interest over their owned coins, just as standard Proof of Stake. Last but not least PoZ is far away more cheap than PoW, in term of power & processor consumption. Zcrypt is an anoymouc cryptocurrency that uses zero knowledge proofs. It uses a Proof of Work/Proof of Stake protocol with a new algorithm, LyraZ.

## Used in
* ZCrypt

# Raft
 Raft is a consensus algorithm designed as an alternative to Paxos. It was meant to be more understandable than Paxos by means of separation of logic, but it is also formally proven safe and offers some additional features. Raft offers a generic way to distribute a state machine across a cluster of computing systems, ensuring that each node in the cluster agrees upon the same series of state transitions.

## Used in
* IPFS Private Cluster
* Quorum

# PoET
PoET is a consensus mechanism algorithm that is often used on the permissioned blockchain networks to decide the mining rights or the block winners on the network. Permissioned blockchain networks are those which require any prospective participant to identify themselves before they are allowed to join. Based on the principle of a fair lottery system where every single node is equally likely to be a winner, the PoET mechanism is based on spreading the chances of a winning fairly across the largest possible number of network participants.

The timer is different for each node. Every participant in the network is assigned a random amount of time to wait, and the first participant to finish waiting gets to commit the next block to the blockchain. Similar to pulling straws, but this time, the shortest stem in the stack wins the lottery.

## Used in
* Hyperledger Sawtooth

## Pros
* Node will rest, so more energy efficient
## Cons
* Trust Intel, require dedicated hardware
## Read more
* HackerNoon https://hackernoon.com/consensuspedia-an-encyclopedia-of-29-consensus-algorithms-e9c4b4b7d08f

[Go to Index](#index)

# Proof of History
Instead of trusting the timestamp on the transaction, you could prove that the transaction occurred sometime before and after an event. The Proof of History is a high frequency Verifiable Delay Function. A Verifiable Delay Function requires a specific number of sequential steps to evaluate, yet produces a unique output that can be efficiently and publicly verified.

Proof of History is a sequence of computation that can provide a way to cryptographically verify passage of time between two events. It uses a cryptographically secure function written so that output cannot be predicted from the input, and must be completely executed to generate the output. The function is run in a sequence on a single core, its previous output as the current input, periodically recording the current output, and how many times its been called. The output can then be re-computed and verified by external computers in parallel by checking each sequence segment on a separate core. Data can be timestamped into this sequence by appending the data (or a hash of some data) into the state of the function. The recording of the state, index and data as it was appended into the sequences provides a timestamp that can guarantee that the data was created sometime before the next hash was generated in the sequence. This design also supports horizontal scaling as multiple generators can synchronize amongst each other by mixing their state into each others sequences.

## Description
The system is designed to work as follows. With a cryptographic hash function, whose output cannot be predicted without running the function (e.g. sha256, ripemd, etc.), run the function from some random starting value and take its output and pass it as the input into the same function again. Record the number of times the function has been called and the output at each call. The starting random value chosen could be any string, like the headline of the New York times for the day.

For example:
PoH Sequence 
Index Operation                          Output Hash 
1     sha256(”any random starting value”)    hash1
2     sha256(hash1)                          hash2
3     sha256(hash2)                          hash3

Where hashN represents the actual hash output.
It is only necessary to publish a subset of the hashes and indices at an interval.

Index Operation                           Output Hash 
1     sha256(”any random starting value”) hash1 
200   sha256(hash199)                     hash200
300   sha256(hash299)                     hash300

As long as the hash function chosen is collision resistant, this set of hashes can only be computed in sequence by a single computer thread. This follows from the fact that there is no way to predict what the hash value at index 300 is going to be without actually running the algorithm from the starting value 300 times. Thus we can thus infer from the data structure that real time has passed between index 0 and index 300. 

In the example in Figure 2, hash 62f51643c1 was produced on count 510144806912 and hash c43d862d88 was produced on count 510146904064. Following the previously discussed properties of the PoH algorithm, we can trust that real time passed between count 510144806912 and count 510146904064.

![PoH sequence](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/poh-sequence.png)

Check solana-whitepaper.pdf for more details how PoH is implemented and how it scale https://raw.github.com/cedricwalter/blockchain-consensus/master/whitepaper/PoH-Solana-whitepaper.pdf


## Used in
* Solana
## Read more
Whitepaper https://solana.com/solana-whitepaper.pdf

[Go to Index](#index)

# Proof of Stake Velocity
Proof of Stake Velocity (PoSV) is proposed as an alternative to Proof of Work (PoW) and Proof of Stake (PoS) to secure the peer-to-peer network and confirm transactions of Reddcoin, a cryptocurrency created specifically to facilitate social interactions in the digital age. PoSV is designed to encourage both ownership (Stake) and activity (Velocity) which directly correspond to the two main functions of Reddcoin as a real currency: store of value and medium of exchange. Reddcoin can also function as the unit of account in heterogeneous social context.

## Used in
* Reddcoin

## Read more

[Go to Index](#index)

# Proof of Importance
 NEM’s consensus network depends not only the number of coins but on the possibility that productive system action ought to be remunerated. The chances of staking a block are a component of various factors, including notoriety (controlled by a different purpose-designed framework), balance, and the number of transactions made to and from that position.

Productive network activity, not just the number of coins accumulated, should be rewarded. Participants who frequently send and receive transactions are more likely to find blocks.

## Used in
New Economy Movement (XEM)
## Pros
You can still be a priority (over miner) if you perform frequent transactions and connections that are good for the ecosystem.
## Read more

[Go to Index](#index)

# Proof of Participation (PoP)
If you read or listen to podcasts on the Let's Talk Bitcoin website, you have just participated in PoP

# Read more
Example https://docs.google.com/document/d/1L7HmE8IupFiSrfqk9BgNa4Zg9XogqtScyQjTw0k2xCc/edit

[Go to Index](#index)

# Proof Of Activity
Proof of activity is a hybrid approach that combines both proof of work and proof of stake.
As in PoW, miners race to solve a cryptographic puzzle. Then the system switches to PoS.

## Used in
* Decred https://www.decred.org/

## Pros
* Criticisms are the same as for both proof of work and proof of stake.

## Read more

[Go to Index](#index)

## Proof of Believability
IOST introduced Servi as both a measurement of users’ contribution to the community and a way to encourage members to contribute to the continued development of the IOSChain.

## Used in
* IOST
## Read more
Whitepaper https://github.com/iost-official/Documents/blob/master/Technical_White_Paper/EN/Tech_white_paper_EN.md#consensus-mechanism

[Go to Index](#index)

# Proof of Care (PoC)
Rather than distributing presale tokens based on, say, how much users are contributing, companies can distribute token based on the quality of your proof-of-care for the project. On top of that, it's not even about social proof (i.e., how many Twitter followers you have), it's about the genuineness of your proof-of-care.

It's a great way to essentially crowd-market your blockchain project by encouraging others to get the word out about it. it's about producing interesting, fun, informative content.

## Used in
Quantstamp
TomoCoin

## Pros
* Implementing individual caps is very good step and can restrict whales from entering the public sale
* Attract long term investors
* Help spread the word by individuals
# Cons
* Content creators have an advantage as they will have more influence and better chances to make it through.
* Other people will just copy content from other's post just to complete their Proof of Care = lot of spam.
## Read more
Whitepaper https://github.com/iost-official/Documents/blob/master/Technical_White_Paper/EN/Tech_white_paper_EN.md#consensus-mechanism

[Go to Index](#index)

# Proof of Value (PoV)
Earn token when user publish work to audience.

## Used in
Doc https://docs.google.com/document/d/1VogMc11WOeWB_OrcsIGD_J7F02KZ0I5zlDYTma7FJkA/edit

## Read more
* LTBcoin

[Go to Index](#index)

# Proof of Quality (PoQ)
E.g after PoV a month later when the performance of any work is compared against all the other work published during that week, user get an additional reward

## Used in 
Doc https://docs.google.com/document/d/1HBbuN8rmrH22kXSYiDZaRv9aR7MVrI4FB8fSrSQ37tc/edit
## Read more
* LTBcoin

# Variable Delayed Proof Of Stake (vDPOS)
Ongoing, but you can help me with links, contact me

## Used in
* CryptoCircuits

[Go to Index](#index)

# Proof-of-work time (PoWT)
Proof-of-Work-Time (PoWT) is a novel approach to forming a consensus by introducing a variable blocktime that scales with mining power, where the blockchain speeds up with power increases. This better scales the blockchain, increases transaction speed with power and allows for auto-adjusting more profitable mining. Difficulty dependent blocktime (Max ~6.2 minutes, minimum 15 seconds).

Blocktime dependent rewards (~Reward halving every minute decrease in blocktime till 10x VRC supply parity, then variable ~3% disinflation). Algo: scrypt² (N of 1024² or 128MB per thread) Block 1: 564,705 VRM minted for ICO participants who purchased VRM using VRC. Minimum Transaction Fee: 0.2 VRM (high commodity transaction fee paid to miners). RPC Port: 33987, P2Port: 36988 Confirmations: 30, Maturity: 100.

## Used in
* Vericoin
* Verium

## Read more
Wiki https://wiki.vericoin.info/

[Go to Index](#index)

# Serialization of Proof-of-work Events: Confirming Transactions via Recursive Elections
 Utilizes a combination of PoW and DAGs to reach scalable consensus. In SPECTRE, the blocks are mined pointing to multiple parents, not just one, so the network could potentially handle multiple blocks per second. Mining a block pointing to some parent blocks supports those blocks validity. Compared to PoW’s “longest chain wins”, SPECTRE uses something like “blocks with the most childen win.” SPECTRE hasn’t been battle-tested in the wild yet, and new attack vectors are likely to emerge, but it feels like a very clever potential way to fix Bitcoin.

## Used in
* Proposal for Bitcoin https://bitcoin.org/en

# Proof-of-work (PoW) / High Interest Proof of Stake (HiPoS)
Coin combining PoW and HiPoS

## Used in
* EdgeCoin (EDGE)

[Go to Index](#index)

# Proof of Work (PoW) / Nexus Proof of State (nPoS) or Nexus Proof of Holding (nPOH)
 Nexus uses 3 consensus channels to maximize decentralization and provide fast, secure transactions. Each channel has an independent difficulty algorithm, amongst other checks and balances, to prevent a single channel from monopolizing block production and compromising the security of the network. Nexus channels include a Prime channel (CPU Mining), a Hashing channel (GPU Mining), and Nexus Proof of Holding (nPOH). Nexus takes the proof-of-stake system developed by Peercoin, and combines it with a Trust-based weighting system to create the Proof-of-Holding consensus mechanism. Nodes receive a Trust rating that is established by their contributions to the network, which increases over time. Nodes with greater Trust are granted an increased minting rate, which increases from 0.5% to 3% within one year, the longer you build Trust on the network.
3 consensus channels: Prime (CPU), Hashing (GPU), and Nexus Proof of Holding (nPOH)

## Used in
* Nexus https://nexusearth.com/

## Pros
* Key signature scheme to keep an account’s public keys obscured even when making transactions (This is made possible by moving away from addresses based on public key hashes, and implementing a new system called Signature Chains).
* quantum resistance (Nexus uses a combination of SHA3 hashing algorithms combined with 571 bit private keys and 512/1024 bit proof of work)
* multiple consensus channels greatly reduces the risk of a 51% attack (attacker would need to control all 3 channels)
* OnChain scalability Transaction processing is distributed across multiple channels working synergistically to increase transaction throughput as resources increase. Individual channels verify transactions, consolidate verified transactions into Merkle trees, and add finished blocks onto the blockchain. The Unified Time protocol enables transaction processing, trust locks, and block locks to be consistent throughout time. The potential of Nexus 3DC is limited only by node count and represents the most energy-efficient consensus system to date.

## Read more
Whitepaper https://nexusearth.com/nexus-white-paper

[Go to Index](#index)

# Delayed Proof of Work (dPoW)
Delayed Proof of Work (dPoW) is a hybrid consensus method that allows one blockchain to take advantage of the security provided through the hashing power of a secondary blockchain. This is achieved through a group of notary nodes that add data from the first blockchain onto the second, which would then require both blockchains to be compromised to undermine the security of the first.

Delayed Proof of Work (dPoW) is a hybrid consensus method that allows one blockchain to take advantage of the security provided through the hashing power of a secondary blockchain. This is achieved through a group of notary nodes that add data from the first blockchain onto the second, which would then require both blockchains to be compromised to undermine the security of the first. The first to make use of this consensus method is Komodo, which is attached to the Bitcoin blockchain.

## pros
* Energy efficient
* Increased security
## Cons
* Limited to blockchain using PoW or PoS

[Go to Index](#index)

# Delayed Proof of Work (dPoW)
Coin combining PoW and dPoW.
Delayed Proof of Work (dPoW) is a hybrid consensus method that allows one blockchain to take advantage of the security provided through 
the hashing power of a secondary blockchain. This is achieved through a group of notary nodes that add data from the first blockchain onto the second, which would then require both blockchains to be compromised to undermine the security of the first. The first to make use of this consensus method is Komodo, which is attached to the Bitcoin blockchain.

## Used in
Komodo https://wiki.komodoplatform.com/wiki/Komodo

## Pros
Energy efficient
Increased security
## Cons
Limited to blockchain using PoW or PoS

## Read more

[Go to Index](#index)

# Proof of Work (PoW) / PoM / PoSII
Coin combining PoW and PoM and PoSII

## Used in
* NOBL
* Magi Coin

## Read more
Github https://github.com/magi-project/m-Noblecoin

[Go to Index](#index)

# Proof of Work (PoW) / Proof of Stake (PoS) / Proof Of Care (PoC)
Coin combining PoW and PoS and PoC

## Used in
* TamaGucci

[Go to Index](#index)

# Proof of Stake (PoS) / Proof of Disintegration (PoD)
B3 is the first coin to develop and implement Fundamental Nodes (FN). A Fundamental Node is similar to a regular masternode in terms of the service it provides to the network but the coins used to purchase a Fundamental Node are destroyed. This reduces the overall supply of the coin over time as more Fundamental Nodes are added to the network. Fundamental Nodes receive 60% of the block reward while those staking receive 40%.

## Used in
b3coin https://b3coin.io/
## Read more
Whitepaper https://b3coin.io/

[Go to Index](#index)

# Proof-of-Stake (POS) / Proof-of-Presence (PoP)
1. Reward for generating blocks (Proof-of-Stake, POS). This involves running a full node, unlocked and with the user's stake applied to generate blocks. Users who run a block generating node generally need to have at least a moderate amount of token on their account
2. Reward for storing the blockchain (Proof-of-Presence, POP). Only the most recent blocks file is distributed amongst all p2p nodes, previous blocks files are not needed for normal p2p operations. Token incentives users to store and make available previously archived block files.

## Used in
HEAT

## Read more
Whitepaper https://heatledger.com/HEATWhitepaper.pdf

[Go to Index](#index)

# Leasing Proof of Stake (PoS/LPoS)
 LPoS is an enhanced version of Proof-of-Stake. In a regular Proof-of-Stake system, each node that holds a certain amount of cryptocurrency is eligible to add the next block to the blockchain but in the LPoS system, on the Waves Platform, users can lease their balance to full nodes. WithLPoS, the user will have the ability to Lease WAVES form the wallet to different contractors which can pay a percentage as a reward. The larger the amount that is leased to a full node, the higher the chances of that full node being selected to produce the next block. If that full node is selected to produce the next block, the leaser will then receive a percentage of the transaction fee that is collected by the full node. In a LeasedProof-of-Stake environment, users can choose between running a full node or leasing their stake to a full node with receiving rewards. This system allows anyone to participate in the Waves network maintenance. User can leas his waves through leasing on any computer or mobile device that has an internet browser since Waves provides a lite client solution that does not require Miners, that are leasing their balance to store the whole Blockchain or to have the wallet running

## Used in
* Nxt
* Waves

[Go to Index](#index)

# Direct Acyclic Graph

# Tangle (DAG)
 Tangle is the DAG consensus algorithm used by Iota. In order to send an Iota transaction, you need to validate two previous transactions you’re received. The two-for-one, pay-it-forward consensus strengthens the validity of transactions the more transactions are added to the Tangle. Because the consensus is established by the transactions, theoretically, if someone can generate 1/3 of the transactions they could convince the rest of the network their invalid transactions are valid. Until there’s enough transaction volume that creating 1/3rd of the volume becomes unfeasible, Iota is sort-of “double-checking” all of the network’s transactions on a centralized node called “The Coordinator”. Iota says The Coordinator works like training wheels for the system, and will be removed once the Tangle is big enough.

![What is Tangle](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/tangle1.png)

This is directed, asynchronous graph (DAG) representing each individual transaction. You’ll notice that each transaction references exactly two other transactions to the left.

## Used in
* IOTA
## Pros
* Low transaction fees (PoW on 2 other Tx)
* Extremely small transactions
* Scalability
* Lightweight
* Quantum-secure (Use trinary, or balanced ternary computations instead of the standard binary computations performed by classical computers)

## Cons
* No Smart Contracts yet
* Vulnerable (only 34% of the total hashing power required)

## Read more
* iota1_4_3.pdf https://assets.ctfassets.net/r1dr6vzfxhev/2t4uxvsIqk0EUau6g2sw0g/45eae33637ca92f85dd9f4a3a218e1ec/iota1_4_3.pdf
* The Coordinator https://domschiener.gitbooks.io/iota-guide/content/chapter1/current-role-of-the-coordinator.html

[Go to Index](#index)

# Block-lattice - Directed Acyclic Graphs (DAGs)
The Block-lattice is a structure where every user (address) gets their own chain that only they can write to, and everyone holds a copy of all of the chains. Block-lattice transform a shared global ledger(like in Bitcoin) into a set of non-shared asynchronous ledgers, which speed up transactions time.

![block-lattice1.png](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/block-lattice1.png)
Blockchain consists of ordered units called blocks . Blocks contain headers and transactions. Each block header, amongst other metadata, contains a reference to its predecessor in the form of the predecessor's hash. The initial state is hard-coded in the first block called the genesis block. Unlike other blocks, the genesis block has no predecessor.

![block-lattice2.png](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/block-lattice2.png)
In contrast to blocks, a DAG structure stores transactions in nodes, where each node holds a single transaction. In Nano, every account is linked to its own account-chain in a structure called the block-lattice equivalent to the account's transaction/balance history. The structure of the block-lattice is displayed in Figure 2. Each account is granted an account chain. An account chain can be considered as a dedicated blockchain, just for a single account. Nodes are appended to an account-chain, each node representing a single transaction on the account chain. Similar to the genesis block in blockchain, a DAG holds a genesis transaction. The genesis transaction defines the initial state. In Nano, instead of having a single transaction that transfers value, two transactions are needed to fully execute a transfer of value. A sender generates a send transaction, while a receiver generates a matching receive transaction, as depicted in Figure 3. When a send transaction is issued, funds are deducted from the balance of the sender's account, and are pending in the network awaiting for the recipient to generate the corresponding receive transaction. While in this state, transactions are deemed unsettled. When the receive transac- tion is generated, the transaction is settled. The downside of this approach is that a node has to be online in order to receive a transaction.

![block-lattice3.png](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/block-lattice3.png)
Transaction handling in the block lattice. S represents a send transaction, R represents a receive transaction. 

Every transaction is broken down into both a **send block** on the sender’s chain and a **receive block** on the receiving party’s chain. A send transaction will deduct funds from a sender’s balance, whilst a receive transaction will add funds to a receiving account’s balance. If the account owner misbehaves, then the rest of the network will vote against the invalid block and it will be rejected.

Each account chain can only be updated by the accounts owner. This is because each block in the chain must be signed by the accounts private key. The rest of the node network will still check and verify that every block is valid and make sure there are no double spends and that people don't increase their balance more than they are supposed to.

Nano **secures its ledger** through the use of **delegated proof of stake (dPoS)**:
With dPoS, users have the ability to choose a representative node to vote on their behalf, acting as a voting proxy. A representative node fulfills tasks such as verifying signatures for blocks that are processed, and in the event of conflicting transactions, voting for the valid transaction. The voting process is balance-weighted, meaning that the weight of a representative’s vote is directly proportional to the amount of Nano that have been linked to it. The greater the number of Nano linked to a representative, the more its vote will be worth. This is possibly more secure than POW coins which rely on 51% of the hashing power: anyone who launches a 51% attack on a DPOS coin would have to own 51% of all coins.

Nano use Proof of Work (PoW) to avoid spammers as there is no transaction fees on the network. Each block has a small amount of work associated with it, approximately about 5 seconds to generate, and 1 microsecond to validate. This forces a malicious actor to dedicate a significant amount of computing power to carry out an attack, whilst requiring only a small amount of computing power by everyone else. Furthermore, it is also even possible for these spam transactions to be pruned away, limiting the amount of storage that can be consumed from this type of attack.

## Attacks
* Penny-spend attack: attackers inflate the number of chains node must keep track of by sending negligible amounts to a wide array of empty wallets.
* Double spend by a malicious user. Both versions of the double spend need to be signed by the users private key. It is easy to identify the accounts that are responsible for spam attacks and then blacklist them for a certain period. 
* read more in [Nano wiki](https://github.com/clemahieu/raiblocks/wiki/Attacks)

![Visualization of block lattice](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/block-lattice.png)

## Used in
* Nano (first to introduced) https://www.mycryptopedia.com/raiblocks-explained/ (previously Raiblocks https://raiblocks.net/)

## Pros
* Less intensive storage requirements by means of database pruning since each user’s blockchain tracks their account balance, rather than their transaction amounts.
* User’s blockchain can be updated asynchronously to the rest of the block lattice.
* faster transaction times: the entire network no longer has to process every single transaction that is made. 
* No transaction fees on the network

## Cons
* No smart contracts
* No monetary incentives for running a full node
* Nano is a deflationary currency (a currency that constantly increases in value)

## Read more
[Nano Whitepaper](https://raiblocks.net/media/RaiBlocks_Whitepaper__English.pdf)  

# LFT
LFT is a continuation of Tendermint to improve BFT consensus algorithms, it is currently what ICON uses as its consensus algorithm. LFT reduces communication overhead by consolidating messages from the network

## Used in
ICON
## Read more
ICON http://icon.support/a-primer-to-lft-loop-fault-tolerance-consensus-algorithm/

[Go to Index](#index)

# Modified Federated Byzantine Agreement (mFBA)
 FBA organises nodes into groups call quorums whereby overall consensus is met by: Quorum consensus among a certain amount of nodes (within a specific quorum); then Consensus among a certain number of quorums to finally determine the final consensus.

![mFBA](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/mFBA.png)

## pros
* Decentralized control
* Low latency
* Flexible trust
* Asymptotic security
## Read more
Medium https://medium.com/@boscoin/dpos-mfba-c84bae2e21ae

[Go to Index](#index)

# Federated Byzantine Agreement
The general idea is that every Byzantine general, responsible for their own chain, sorts messages as they come in to establish truth. In Ripple the generals (validators) are pre-selected by the Ripple foundation. In Stellar, anyone can be a validator so you choose which validators to trust.

## Used in
Stellar
Ripple

## pros
* High throughput, 
* low transaction cost, 
* network scalability
## Read more
Stellar Whitepaper https://www.stellar.org/papers/stellar-consensus-protocol.pdf

# Practical Byzantine Fault Tolerance
PBFT works in asynchronous environments like the Internet and incorporates several important optimizations that improve the response time of previous algorithms by more than an order of magnitude.

## Used in
Hyperledger Fabric
## pros
* High transaction throughput
## Cons
Centralized/permissioned
## Read more
* http://pmg.csail.mit.edu/papers/osdi99.pdf

[Go to Index](#index)

# Delegated Byzantine Fault Tolerance
 The dBFT is called the Delegated Byzantine Fault Tolerant, a Byzantine fault-tolerant consensus mechanism that enables large-scale participation in consensus through proxy voting. The holder of the NEO token can, by voting, pick the bookkeeper it supports. The selected group of bookkeepers, through BFT algorithm, reach a consensus and generate new blocks. Voting in the NEO network continues in real time, rather than in accordance with a fixed term.

##Used in
* Neo
## Read more
* Neo implementation https://github.com/neo-project/docs/blob/master/en-us/index.md#neo-technology-implementation

[Go to Index](#index)

# Byzantine Fault Tolerance (BFT)
The classical problem in distributed computing that is usually explained with Byzantine generals.

## Used in
* Hyperledger https://www.hyperledger.org/
* Dispatch https://t.me/dispatchlabs
* Ripple https://ripple.com/
## Pros
* High throughput; low cost; scalable
## COns
* Semi-trusted
## Read more
* Whitepaper https://web.archive.org/web/20170205142845
* Whitepaper http://lamport.azurewebsites.net/pubs/byz.pdf

[Go to Index](#index)

# Magi's proof-of-work (mPoW)
 The magi's proof-of-work (PoW) protocol, in addition to required computational works to be done to deter denial of service attacks, is also a network-dependent rewarding model system. The mPoW rewards participants who solve complicated cryptographical questions not only to validate transactions but also to create new blocks and generate coins. The amout of coins generated are constantly monitored by the mPoW protocol and tuned on the basis of an attraction-repulsion model: 1) incremental rewarding to stimulate network activities during passive mining phase, and 2) decremental rewarding to mitigate redundant mining sources during agressive mining phase. mPoW can effectively govern the magi's network and limit it under a certain scale, enabling the general devices to be capable of mining magi.

## Used in
* MAGI https://www.m-core.org/
## Read more
* Whitepaper https://arxiv.org/abs/1409.7948

[Go to Index](#index)

# Magi's proof-of-stake (mPoS)
 Aims to achieve distributed consensus through operations in addition to mPoW. mPoS is designed such that it rejects potential attacks through accumulating a large amount of coins or offline staking time, either of which leads to security concerns. Similar to mPoW's operation, mPoS is constructed in accordance with the concept of the attraction-repulsion model. Magi hybridizes mPoW with mPoS, and integrate both consensus approaches in order to acquire benefits from the two mechanisms and create a more robust payment system.

## Used in
MAGI https://www.m-core.org/
## Read more
Bitcointalk https://bitcointalk.org/index.php?topic=735170.msg9991269#msg9991269

