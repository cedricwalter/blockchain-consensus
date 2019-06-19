---
description: 'Hot-Stuff the Linear, Optimal-Resilience, One-Message BFT Devil'
---

# HotStuff

### Algorithm

> HotStuff, a leader-based Byzantine fault-tolerant replication protocol for the partially synchronous model. Once network communication becomes synchronous, HotStuff enables a correct leader to drive the protocol to consensus at the pace of actual \(vs. maximum\) network delay--a property called responsiveness--and with communication complexity that is linear in the number of replicas. To our knowledge, HotStuff is the first partially synchronous BFT replication protocol exhibiting these combined properties. HotStuff is built around a novel framework that forms a bridge between classical BFT foundations and blockchains. It allows the expression of other known protocols \(DLS, PBFT, Tendermint, Casper\), and ours, in a common framework. Our deployment of HotStuff over a network with over 100 replicas achieves throughput and latency comparable to that of BFT-SMaRt, while enjoying linear communication footprint during leader failover \(vs. quadratic with BFT-SMaRt\). [https://arxiv.org/abs/1803.05069](https://arxiv.org/abs/1803.05069)

Authors researchers [Maofan Yin](https://arxiv.org/search/cs?searchtype=author&query=Yin%2C+M), [Dahlia Malkhi](https://arxiv.org/search/cs?searchtype=author&query=Malkhi%2C+D), [Michael K. Reiter](https://arxiv.org/search/cs?searchtype=author&query=Reiter%2C+M+K), [Guy Golan Gueta](https://arxiv.org/search/cs?searchtype=author&query=Gueta%2C+G+G), [Ittai Abraham](https://arxiv.org/search/cs?searchtype=author&query=Abraham%2C+I)

### Whitepaper

* [https://arxiv.org/pdf/1803.05069](https://arxiv.org/pdf/1803.05069) 

### Pros

* HotStuff use a single message type for proposing, a single message type for voting, and simple Commit and Preferred Branch Rules.

> HotStuff makes BFT more scalable by an order of magnitude, as the algorithm’s view-change complexity is made quadratically faster — a function of simply the number of nodes in the network, as opposed to a function of the number of nodes squared, as is the case in PBFT. \([https://medium.com/@cypherium/what-is-hotstuff-and-why-is-it-a-big-deal-213f39696763](https://medium.com/@cypherium/what-is-hotstuff-and-why-is-it-a-big-deal-213f39696763)\)

### Used in 

* [Cypherium](https://cypherium.io/)

### Read more

* [https://blockchainschool.epfl.ch/wp-content/uploads/2019/02/sbws19-malkhi.pdf](https://blockchainschool.epfl.ch/wp-content/uploads/2019/02/sbws19-malkhi.pdf)
* [https://dahliamalkhi.wordpress.com/2018/10/24/hotstuff-three-chain-rules/](https://dahliamalkhi.wordpress.com/2018/10/24/hotstuff-three-chain-rules/)
* [https://dahliamalkhi.wordpress.com/2018/03/13/casper-in-the-lens-of-bft/](https://dahliamalkhi.wordpress.com/2018/03/13/casper-in-the-lens-of-bft/)

