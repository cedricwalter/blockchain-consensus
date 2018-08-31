# Blockchain Consensus?

At the core of the Blockchain disruption are consensus algorithm:

> Consensus algorithms enable network participants to agree on the contents of a blockchain in a distributed and trust-less manner.
>
> “Consensus decision-making is a group decision-making process in which group members develop, and agree to support a decision in the best interest of the whole. Consensus may be defined professionally as an acceptable resolution, one that can be supported, even if not the “favourite” of each individual. Consensus is defined by Merriam-Webster as, first, general agreement, and second, group solidarity of belief or sentiment.” Wikipedia

And the consensus algorithm plays a crucial role in maintaining the safety and efficiency of blockchain. Using the right algorithm may bring a significant increase to the performance of blockchain application.

The trilemma claims that blockchain systems can only at most have two of the following three properties: 1. Decentralization \(defined as the system being able to run in a scenario where each participant only has access to O\(c\) resources, i.e. a regular laptop or small VPS\) 2. Scalability \(defined as being able to process O\(n\) &gt; O\(c\) transactions\) 3. Security \(defined as being secure against attackers with up to O\(n\) resources\)

Each consensus algorithm has its own application scenario. There is no absolute good or bad. The choice of which consensus to use for implementing the blockchain depends on the type of network and data.

For a transaction to be valid on most cryptocurrency networks, the transaction needs to collect a certain number of confirmations \(often equals to an inclusion in a block of a blockchain\) from the network. E.g 10 confirmations means to see a specific transaction in one block and 9 consecutive blocks.

