# Delayed Proof of Work \(dPoW\)

Delayed Proof of Work \(dPoW\) is a hybrid consensus method that allows one blockchain to take advantage of the security provided through the hashing power of a secondary blockchain. This is achieved through a group of notary nodes that add data from the first blockchain onto the second, which would then require both blockchains to be compromised to undermine the security of the first.

Delayed Proof of Work \(dPoW\) is a hybrid consensus method that allows one blockchain to take advantage of the security provided through the hashing power of a secondary blockchain. This is achieved through a group of notary nodes that add data from the first blockchain onto the second, which would then require both blockchains to be compromised to undermine the security of the first. The first to make use of this consensus method is Komodo, which is attached to the Bitcoin blockchain.

#### Used in

* [Komodo](https://komodoplatform.com) end-to-end blockchain solutions. DPoW consensus mechanism does not recognize The Longest Chain Rule to resolve a conflict in the network, instead the dPoW looks to backups it inserted previously into the chosen PoW blockchain. The process of inserting backups of Komodo transactions into a secure PoW is “notarization.” Notarisation is performed by the elected notary nodes. Roughly every ten minutes, the notary nodes perform a special block hash mined on the Komodo blockchain and take note of the overall Komodo blockchain “height”. The notary nodes process this specifc block so that their signatures are cryptographically included within the content of the notarized data. There are sixty-four “notary nodes” elected by a stake-weighted vote, where ownership of KMD represents stake in the election. They are a special type of blockchain miner, having certain features in their underlying code that enable them to maintain an effective and cost-efcient blockchain and they periodically receives the privilege to mine a block on “easy difculty.” [Whitepaper](https://komodoplatform.com/en/whitepaper/2018-02-14-Komodo-White-Paper-Full.pdf)

#### pros

* Energy efficient
* Increased security

**Cons**

* Limited to blockchain using PoW or PoS

