# Proof of Retrievability \(POR\)

A proof of Retrievability \(POR\) is a compact proof by a file system \(prover\) to a client \(verifier\) that a target file F is intact, in the sense that the client can fully recover it. As PORs incur lower communication complexity than transmission of F itself, they are an attractive building block for high-assurance remote storage systems. It can be really useful as a consensus algorithm for Cloud computing systems.

Permacoin proposed a modification to Bitcoin that repurposes its mining resources to achieve a more broadly useful goal: distributed storage of archival data. Unlike Bitcoin and its proposed alternatives, Permacoin requires clients to invest not just computational resources, but also storage. This scheme involves an alternative scratch-off puzzle for Bitcoin based on Proofs-of-Retrievability \(PORs\). Successfully minting money with this SOP requires local, random access to a copy of a file. Given the competition among mining clients in Bitcoin, this modified SOP gives rise to highly decentralized file storage, thus reducing the overall waste of Bitcoin.

## Used in

* Microsoft
* [PermaCoin](https://www.cs.umd.edu/~elaine/docs/permacoin.pdf)

## Read more

* [Wikipedia](https://eprint.iacr.org/2008/175.pdf)

