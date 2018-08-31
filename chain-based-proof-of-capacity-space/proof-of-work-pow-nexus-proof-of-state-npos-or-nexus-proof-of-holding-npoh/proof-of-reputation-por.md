# Proof of Reputation \(PoR\)

POR is an upgraded, stronger, and more secure form of Proof of Authority \(POA\). In POA the transactions and blocks are validated by approved accounts known as validators. POA has typically been used in private networks and most recently a few companies that have adopted it to use individuals as the validators whose identities are publicly disclosed and at stake.

Proof of Reputation \(PoR\) consensus model depends on the reputation of the participants to keep the network secure. A participant \(a block signer\) must have a reputation important enough that they would face significant financial and brand consequences if they were to attempt to cheat the system. POR uses companies as validators not individuals.

Once a company proves reputation and passes verification, they may be voted into the network as an authoritative node and at this point, it operates like a Proof of Authority network \(PoA\), where only authoritative nodes can sign and validate blocks.

A company caught cheating would not only be risking its reputation. It would be risking its entire market cap and the reputation of the officers and shareholders of the company. It would have significantly more to lose than any one individual.

**Authorized Signers** Authorized signers are trusted nodes that create blocks, sign them, and distribute them to other nodes. A list of authorized signers will be maintained on the blockchain. Only authorized nodes can sign blocks and all blocks are verified that this is true by checking the signer is in the authorized list. The signing algorithm is essentially the same signature algorithm as PoW but with a different set of headers. PoW-specific headers will be removed and additional headers added to enable voting. Given N authorized signers, a signer may only sign a block every \(N/2\) + 1. This ensures that someone would need to control &gt; 50% of signers to perform a malicious attack. Authorized signers will be rewarded in Coins per block signed.

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

