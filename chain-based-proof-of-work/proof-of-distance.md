# Proof of Edit Distance

## Algorithm

Edit distances are a class of algorithms that score how close two strings are to each other. For instance the _an Edit Distance_ for “ETH” and “ETC” is “0.8222” where two identical strings would score a “1”. There are many algorithms also in the string similarity space including the _Levenshtein Distance_, _Smith-Waterman Gotoh_ _Distance,_ and the _Ratcliff-Obershelp Distance._

### Using Proof of Edit distance for forging new blocks

Miners compete to find a string that when hashed in a normalization process is above a minimum distance threshold. This string could then be the hash of an intermediary-blockchain and the header hash for the next block.

Let Minimum Distance Threshold by “t”, String to find “B”, and Edit Distance Function “ED”. Such that for each blockchain header hash “h” satisfies:

> ED\( H\(h\), H\(B\) \) &lt; t

Or in the case of merging two blockchains:

> ED\(H\(h1\),H\(B\)\) &lt; t && ED\(H\(h2\),H\(B\)\) &lt; t === true

To find the new block in an intermediary-blockchain,  the miner would iterate through a random charset or number, hashing strings until it finds a hash that is above the threshold for all of the blocks. 

## Pros

**Proof of Edit Distance is mining algorithm agnostic.**

Any hash or string structure can be provided as an input which means that as long as the blockchain has unique hashes it can be easily added to the Proof of Edit challenge. 

## Cons



## Used in 

* [Block Collider](https://www.blockcollider.org/)

## Links

* [Block collider whitepaper](https://s3.amazonaws.com/blockcollider/blockcollider_wp.pdf)
* [Medium](https://blog.blockcollider.org/building-a-blockchain-singularity-with-proof-of-edit-distance-1d60c328de7a)

