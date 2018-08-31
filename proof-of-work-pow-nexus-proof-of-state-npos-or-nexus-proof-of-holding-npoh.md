# Proof of Work \(PoW\) / Nexus Proof of State \(nPoS\) or Nexus Proof of Holding \(nPOH\)

Nexus uses 3 consensus channels to maximize decentralization and provide fast, secure transactions. Each channel has an independent difficulty algorithm, amongst other checks and balances, to prevent a single channel from monopolizing block production and compromising the security of the network. Nexus channels include a Prime channel \(CPU Mining\), a Hashing channel \(GPU Mining\), and Nexus Proof of Holding \(nPOH\). Nexus takes the proof-of-stake system developed by Peercoin, and combines it with a Trust-based weighting system to create the Proof-of-Holding consensus mechanism. Nodes receive a Trust rating that is established by their contributions to the network, which increases over time. Nodes with greater Trust are granted an increased minting rate, which increases from 0.5% to 3% within one year, the longer you build Trust on the network. 3 consensus channels: Prime \(CPU\), Hashing \(GPU\), and Nexus Proof of Holding \(nPOH\)

#### Used in

* [Nexus](https://nexusearth.com)

#### Pros

* Key signature scheme to keep an account’s public keys obscured even when making transactions \(This is made possible by moving away from addresses based on public key hashes, and implementing a new system called Signature Chains\).
* quantum resistance \(Nexus uses a combination of SHA3 hashing algorithms combined with 571 bit private keys and 512/1024 bit proof of work\)
* multiple consensus channels greatly reduces the risk of a 51% attack \(attacker would need to control all 3 channels\)
* OnChain scalability Transaction processing is distributed across multiple channels working synergistically to increase transaction throughput as resources increase. Individual channels verify transactions, consolidate verified transactions into Merkle trees, and add finished blocks onto the blockchain. The Unified Time protocol enables transaction processing, trust locks, and block locks to be consistent throughout time. The potential of Nexus 3DC is limited only by node count and represents the most energy-efficient consensus system to date.

#### Read more

* [whitepaper](https://nexusearth.com/nexus-white-paper)

