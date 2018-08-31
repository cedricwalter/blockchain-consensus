# Direct Acyclic Graph Tangle \(DAG\)

Tangle is the DAG consensus algorithm used by Iota. In order to send an Iota transaction, you need to validate two previous transactions you’re received. The two-for-one, pay-it-forward consensus strengthens the validity of transactions the more transactions are added to the Tangle. Because the consensus is established by the transactions, theoretically, if someone can generate 1/3 of the transactions they could convince the rest of the network their invalid transactions are valid. Until there’s enough transaction volume that creating 1/3rd of the volume becomes unfeasible, Iota is sort-of “double-checking” all of the network’s transactions on a centralized node called “The Coordinator”. Iota says The Coordinator works like training wheels for the system, and will be removed once the Tangle is big enough.

![What is Tangle](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/tangle1.png)

This is directed, asynchronous graph \(DAG\) representing each individual transaction. You’ll notice that each transaction references exactly two other transactions to the left.

#### Used in

* IOTA

  **Pros**

* Low transaction fees \(PoW on 2 other Tx\)
* Extremely small transactions
* Scalability
* Lightweight
* Quantum-secure \(Use trinary, or balanced ternary computations instead of the standard binary computations performed by classical computers\)

#### Cons

* No Smart Contracts yet
* Vulnerable \(only 34% of the total hashing power required\)

#### Read more

* [iota1\_4\_3.pdf](https://assets.ctfassets.net/r1dr6vzfxhev/2t4uxvsIqk0EUau6g2sw0g/45eae33637ca92f85dd9f4a3a218e1ec/iota1_4_3.pdf)
* [The Coordinator](https://domschiener.gitbooks.io/iota-guide/content/chapter1/current-role-of-the-coordinator.html)

