# Common Attacks

We list security that are essential for a permission-less consensus algorithm designed for a decentralized ledger system

### 51% attack

In PoS, you would need a majority of all minted coins to conduct such an attack, In PoW, you would need a majority of mining power to conduct such an attack,

### Transaction censoring.

With PoW, a block miner can “choose” not to mine a block containing certain addresses, thereby censoring that address from the network.


#### Sybil attacks

The pBFT mechanisms are susceptible to Sybil attacks, where one entity(party) controls many identities. 
As the number of nodes in the network increase, sybil attacks become increasingly difficult to carry out. But as pBFT mechanisms have scalability issues too, the pBFT mechanism is used in combination with other mechanism(s).
<sub><sup>https://www.geeksforgeeks.org/practical-byzantine-fault-tolerancepbft/</sup></sub>

### Adversary resistance

Indicates the threshold of byzantine nodes that can be tolerated by the consensus algorithm.  

### Sybil resistance

Specifies if the consensus algorithm implements an anti-sybil mechanism. For example, the consensus algorithm should have a mechanism to prevent the generation of sybil identities in a permission-less environment. 

### Accountability & non-repudiation

 Indicates if the consensus protocol implements an identity system and cryptographic signatures. 

### Denial of Service resistance

Specifies if the consensus algorithm implements a denial of service defense mechanism. For instance, some leader based consensus algorithms are susceptible to DoS attacks. 

### Censorship resistance

Indicates if the consensus algorithm is censorship resistant. For example, it precludes external entities from trying to censor transactions.
