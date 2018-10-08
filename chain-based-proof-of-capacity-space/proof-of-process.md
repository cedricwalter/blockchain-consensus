# Proof of Process

Proof of Process is a protocol that allows participants to trust a common process by decoupling the proof of data from the actual source data in a way that yields a single proof that represents all steps of the process.

A process is any sequence of steps in time. Whenever there is a movement of information, ideas, conversations, goods or products, there is a process. 

Traditionally, when institutions want to share their set of processes with one other, they must create common bridges to share their data. Those bridges usually consist of APIs, firewalls, and access management systems.

A process is a sequence of steps in which actors perform specific actions at specific times relative to prior steps or introduce new factual elements and process actors in the sequence.

All steps need not include the same set of actors, and the interaction between actors can be asynchronous as long as the interactions can be grouped together into sequential steps.

Additionally, any step can fork into multiple branches without any need to reconcile them into a single branch. There can be parallel steps in different branches if they are performed at the same time. As time always moves one direction, there can never be circular steps within the same branch.

Examples of processes can be found in almost every human to human and human to machine interaction. Just a handful of examples from this ocean include:

* Trade and settlement processes
* Software as a Service \(SaaS\)
* Online multi-player games
* Board games like chess and Battleship

## Algorithm

1. Extract trust by deriving proofs of the four key factual elements to address the four information security concerns for each step of the process:
   * What: data integrity through cryptographic hashing
   * Who: actor non-repudiation through digital signatures
   * When: proof of anteriority through trusted time-stamping or common time
   * Where: proof of context through cumulative proof via hash chain
2. Generate a single proof for each step
3. Publish the final proof in a distributed fashion through a network in which truth is established through a consensus mechanism

## Used in 

[Stratum](https://stratumn.com/technology/)

## Links

* [https://proofofprocess.org/](https://proofofprocess.org/)
* [http://share.proofofprocess.org/pdf/Proof-of-Process-May-2017.pdf](http://share.proofofprocess.org/pdf/Proof-of-Process-May-2017.pdf)

