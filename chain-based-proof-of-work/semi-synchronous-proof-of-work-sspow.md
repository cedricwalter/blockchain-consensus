# Semi-Synchronous Proof of Work \(SSPoW\)

from Purple Whitepaper:

> The consensus algorithm of Purple is called Semi-Synchronous Proof of Work, or SSPoW for short. It is a variation of Satoshi’s original Proof of Work model of consensus\[2\]. It’s design is to remove the bottleneck that the Proof of Work algorithm imposes on the transaction throughput of the network. This is done by decoupling the choosing of validator nodes, which is done via Proof of Work from the actual transaction validation process. When a node finds a valid Proof of Work, it is advanced into the validator pool where it has an allocated period in which it can validate transactions. This is done asynchronously while
>
> the choice of validator nodes \(PoW\) is synchronous. In this way, the consensus mechanism becomes semi- synchronous, greatly increasing the throughput of the network while providing a safety control mechanism
>
> which can be adjusted based on the current network conditions. The algorithm works by establishing a byzantine partial causal ordering on the network events that are sent between the validator nodes and by transforming it into a total order which is assured to be consistent as long as less than a third of the validators are either byzantine or unresponsive. However, the Total Ordering Algorithms assume that the communication medium between the nodes is reliable so it falls on the CA side of the CAP spectrum. Another step must be included in the algorithm in order to provide partition tolerance. If a network partition happens and this step is not provided, each partition will consider that the nodes from the other partition have crashed and will remove them from their configuration producing a fork of the ledger state. 3.1. Validator pool Transactions are validated by nodes that are in the validator pool. In order to participate in the validation process, nodes have to issue network events, in a deterministic order. A network event issued by a node contains pending transactions which the node wishes to include in the ledger. When nodes join the pool, they are placed on a circle which is represented by the interval \[0, 1\). Each validator in the pool owns a share of this circle which is represented by a sub-interval of \[0, 1\). The order in which the nodes are placed on the circle determines the order in which they are required to issue events. The node owning the lowest share of the interval is always required to be the first to issue an event. When a node joins the pool, the node with the largest share must give half of their share to the joining node. If a node leaves the pool, a node is deterministically chosen to receive the leaver’s share. Pending transactions are deterministically partitioned among all curent validators in order to prevent two nodes from validating the same transaction. A validator node receives the transaction fees of all the transactions that it has processed as reward if it isn’t found to be byzantine or crashed.

read more in Purple whitepaper

{% file src="../.gitbook/assets/purple-whitepaper.pdf" caption="Purple whitepaper" %}

### Used in

Purple

* Whitepaper - [https://purpleprotocol.org/whitepaper/](https://purpleprotocol.org/whitepaper/)
* Website - [https://purpleprotocol.org/](https://purpleprotocol.org/)
* Github - [https://github.com/purpleprotocol](https://github.com/purpleprotocol)
* Twitter - [https://twitter.com/purple\_protocol](https://twitter.com/purple_protocol)
* Reddit - [https://www.reddit.com/r/purpleprotocol/](https://www.reddit.com/r/purpleprotocol/)
* Facebook - [https://www.facebook.com/purpleprotocol/](https://www.facebook.com/purpleprotocol/)
* Medium - [https://medium.com/purple-protocol](https://medium.com/purple-protocol)
* Discord - [https://discord.gg/5ZVZnKd](https://discord.gg/5ZVZnKd)
* Telegram - [https://t.me/purple\_protocol](https://t.me/purple_protocol)





