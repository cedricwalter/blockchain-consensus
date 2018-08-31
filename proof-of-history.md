# Proof of History

Instead of trusting the timestamp on the transaction, you could prove that the transaction occurred sometime before and after an event. The Proof of History is a high frequency Verifiable Delay Function. A Verifiable Delay Function requires a specific number of sequential steps to evaluate, yet produces a unique output that can be efficiently and publicly verified.

Proof of History is a sequence of computation that can provide a way to cryptographically verify passage of time between two events. It uses a cryptographically secure function written so that output cannot be predicted from the input, and must be completely executed to generate the output. The function is run in a sequence on a single core, its previous output as the current input, periodically recording the current output, and how many times its been called. The output can then be re-computed and verified by external computers in parallel by checking each sequence segment on a separate core. Data can be timestamped into this sequence by appending the data \(or a hash of some data\) into the state of the function. The recording of the state, index and data as it was appended into the sequences provides a timestamp that can guarantee that the data was created sometime before the next hash was generated in the sequence. This design also supports horizontal scaling as multiple generators can synchronize amongst each other by mixing their state into each others sequences.

## Description

The system is designed to work as follows. With a cryptographic hash function, whose output cannot be predicted without running the function \(e.g. sha256, ripemd, etc.\), run the function from some random starting value and take its output and pass it as the input into the same function again. Record the number of times the function has been called and the output at each call. The starting random value chosen could be any string, like the headline of the New York times for the day.

For example: PoH Sequence Index Operation Output Hash 1 sha256\(”any random starting value”\) hash1 2 sha256\(hash1\) hash2 3 sha256\(hash2\) hash3

Where hashN represents the actual hash output. It is only necessary to publish a subset of the hashes and indices at an interval.

Index Operation Output Hash 1 sha256\(”any random starting value”\) hash1 200 sha256\(hash199\) hash200 300 sha256\(hash299\) hash300

As long as the hash function chosen is collision resistant, this set of hashes can only be computed in sequence by a single computer thread. This follows from the fact that there is no way to predict what the hash value at index 300 is going to be without actually running the algorithm from the starting value 300 times. Thus we can thus infer from the data structure that real time has passed between index 0 and index 300.

In the example in Figure 2, hash 62f51643c1 was produced on count 510144806912 and hash c43d862d88 was produced on count 510146904064. Following the previously discussed properties of the PoH algorithm, we can trust that real time passed between count 510144806912 and count 510146904064.

![PoH sequence](https://raw.githubusercontent.com/cedricwalter/blockchain-consensus/master/images/poh-sequence.png)

Check solana-whitepaper.pdf for more details how PoH is implemented and how it scale [https://raw.github.com/cedricwalter/blockchain-consensus/master/whitepaper/PoH-Solana-whitepaper.pdf](https://raw.github.com/cedricwalter/blockchain-consensus/master/whitepaper/PoH-Solana-whitepaper.pdf)

## Used in

* Solana

  **Read more**

* [whitepaper](https://solana.com/solana-whitepaper.pdf)

