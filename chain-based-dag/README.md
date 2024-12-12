# Chain-based DAG

A significant limitation of a single-chain topology is its ability to accept only one block at a time. But what if the network could accept multiple blocks simultaneously? This would not only increase the number of transactions processed but also reduce the waste incurred when the network discards all branches except one.

| ![image](https://github.com/cedricwalter/blockchain-consensus/assets/71234183/0c424468-4d28-430d-93bb-387f090e8210) |
|:--:|
| *A directed acyclic graph (DAG)* |

Instead of constructing a linear chain, we can represent this more inclusive approach by building a graph. Many people think of a blockchain as a linear chain, but classic single chains like bitocoin and ethereum actually consist of branches and resemble a tree more than a linear chain. This tree-like structure is a type of graph, specifically a directed acyclic graph (DAG). 

A DAG might sound complex, but it simply means:
 
- Blocks (vertices in mathematical terms) in this graph are connected.
- These connections (edges in mathematical terms) have directions — e.g., block A points to block B
- Following these directed connections from any block, you cannot end up at the same block no matter what path you take — i.e., there are no cycles in this graph

# Chanllenges of DAG-based ledger implementation

Let’s investigate some of the problems we face into while making these design decisions.

## 1. Ordering

In a single chain, the relative order of blocks is clear, as each block is linearly ordered with a defined parent. In a block DAG, only a subset of blocks has a clear relative order, while others do not. This is called partial ordering, which is unacceptable in blockchain.

| ![image](https://github.com/cedricwalter/blockchain-consensus/assets/71234183/c7dfd061-43ef-4e78-9c95-b286171493ff) |
|:--:|
| *Blue: clear relative ordering; Orange: ambiguous relative ordering* |

In the illustration above, blue blocks have a clear relative order since they are directly or indirectly connected. If block A points to block B, block A knows about block B at its construction, indicating block B came before block A. However, orange blocks have ambiguous relative ordering, as there are no direct or indirect connections between them. Thus, some blocks have a clear order, while others do not.

Ordering is crucial because different transaction orders can produce very different outcomes. For example, if A has 1 coin, and we have these transactions:

1. A sends B 1 coin
2. A sends C 1 coin
3. D sends A 1 coin

Processing these in different orders results in different outcomes:

- Order (1, 2, 3): transaction 1 succeeds, 2 fails since A now has no more money, 3 succeeds
- Order (2, 3, 1): transaction 2 succeeds, 3 succeeds, 1 succeeds

In blockchain, ordering is a critical attribute for network consensus; thus, partial ordering is unacceptable.

## 2. Randomness and Delay

**Randomness** involves randomly selecting the next node to produce a block. There is no central entity "selecting" the node; it’s a matter of luck which node solves the puzzle first, given comparable hashing power.

Randomness is vital to prevent targeted attacks, bribery, and other malicious activities. If block producers were known ahead of time, they could be incentivized to cheat or collude—e.g., prioritizing their own trades or attempting double-spends. Randomness ensures the network remains fair and honest.

**Delay** refers to the time taken to create a new block in DLT, controlling the block creation frequency. Every block DAG must incorporate a delay.

But why do we need a delay at all? No network can handle infinitely many blocks; each node would eventually run out of bandwidth, storage, memory, or CPU. There aren’t infinite transactions to fill infinite blocks. The block production rate and the number of transactions per block should adjust dynamically to network conditions, but zero delay is never feasible.

## 3. Block Efficiency

When a node is producing a block, it is deciding which transactions the network will process next. At any given time, each node on the network maintains a list of pending transactions which were sent to the network for processing but haven’t made it into a block yet. When a new block is being produced, a node looks at this pending transaction queue and selects a subset to place into the block. 

| ![image](https://github.com/cedricwalter/blockchain-consensus/assets/71234183/799b3d39-3902-4856-aeb0-f65298db0ac6) |
|:--:|
| *Packing a block efficiently* |

Different networks have developed various conventions for transaction selection, mostly driven by economic incentives.

If there are no severe network issues, each full node should have similar pending transaction queues, as critical information circulates quickly in a peer-to-peer (P2P) network. Nodes generally have heard about the same set of transactions, building similar pending transaction queues.

If every node sees nearly the same set of pending transactions, they will produce blocks containing similar sets of transactions. This redundancy is undesirable, as redundant transactions represent wasted work, which is inefficient. 
