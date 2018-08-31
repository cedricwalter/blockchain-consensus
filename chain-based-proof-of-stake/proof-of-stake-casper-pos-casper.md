# Proof of stake Casper \(PoS Casper\)

## Algorithm

* validators stake a portion of their Ethers as stake.
* validators start validating the blocks. when they discover a block which they think can be added to the chain, they will validate it by placing a bet on it.
* If the block gets appended, he validators will get a reward proportionate to their bets.
* Malicious validator acts trying to do a “nothing at stake”, the will immediately be punished, and all of their stake is going to get slashed.

## Pros

* all Pros of Proof of stake
* punish validator trying to do a “nothing at stake” attack, 
* punishing miners who go offline, unintentionally or not,

## Used in

* Casper the Friendly Finality Gadget \(FFG\), hybrid PoW/PoS that will be implmented first and ease transtion to full PoS. blocks are mined using POW, every 50th block a POS checkpoint where finality is assessed by a network of validators will be used.
* Casper the Friendly GHOST: Correct-by-Construction \(CBC\): full PoS

