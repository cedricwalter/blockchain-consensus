# Federated Byzantine Agreement

The general idea is that every Byzantine general, responsible for their own chain, sorts messages as they come in to establish truth. In Ripple the generals \(validators\) are pre-selected by the Ripple foundation. In Stellar, anyone can be a validator so you choose which validators to trust.

#### Used in

* Stellar - similar to Ripple but with key difference - quorum slice. [link1](https://www.stellar.org/papers/stellar-consensus-protocol.pdf) - [link2](https://www.stellar.org/stories/adventures-in-galactic-consensus-chapter-1/) - [link3](https://medium.com/a-stellar-journey/on-worldwide-consensus-359e9eb3e949)
* Ripple
  * Each node receives transaction from external applications 
  * Each Node forms public list of all valid \(not included into last ledger \(=block\)\) transactions aka \(Candidate Set\) 
  * Nodes merge its candidate set with UNLs\(Unique Node List\) candidate sets and vote on the veracity of all transactions \(1st round of consensus\) 
  * all transactions that received at least 50% votes are passed on the next round \(many rounds may take place\) 
  * final round of consensus requires that min 80% of Nodes UNL agreeing on transactions. It means that at least 80% of Validating nodes should have same Candidate SET of transactions 
  * after that each Validating node computes a new ledger \(=block\) with all transactions \(with 80% UNL agreement\) and calculate ledger hash, signs and broadcasts 
  * All Validating nodes compare their ledgers hash 
  * Nodes of the network recognize a ledger instance as validated when a 80% of the peers have signed and broadcast the same validation hash. 
  * Process repeats. Ledger creation process lasts 5 sec\(?\).

    Each transaction includes transaction fee \(min 0,00001 XRP\) which is destroyed. No block rewards.

    [whitepaper](https://ripple.com/files/ripple_consensus_whitepaper.pdf)

#### pros

* High throughput, 
* low transaction cost, 
* network scalability

  **Read more**

  Stellar Whitepaper [https://www.stellar.org/papers/stellar-consensus-protocol.pdf](https://www.stellar.org/papers/stellar-consensus-protocol.pdf)

