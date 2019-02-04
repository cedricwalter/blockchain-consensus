---
description: >-
  Friendly Finality Gadget (FFG), hybrid PoW/PoS. FFG is a Proof of Stake
  algorithm implementing stake slashing for bad behavior like chain halts and
  censorship. Foreseen for Ethereum 2.0
---

# Casper the Friendly Finality Gadget \(FFG\)

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

* Casper the Friendly Finality Gadget \(FFG\), hybrid PoW/PoS that will be implmented first and ease transtion to full PoS. blocks are mined using POW, every 50th block a POS checkpoint where finality is assessed by a network of validators will be used.  Read [Vitalik’s note on hybrid PoW/FFG](https://vitalik.ca/files/casper_note.html), his [medium post on minimal slashing conditions](https://medium.com/@VitalikButerin/minimal-slashing-conditions-20f0b500fc6c) and the [FFG paper](https://arxiv.org/abs/1710.09437).
* Casper the Friendly GHOST: Correct-by-Construction \(CBC\): full PoS

### Resources

* [https://hackernoon.com/what-to-expect-when-eths-expecting-80cb4951afcd](https://hackernoon.com/what-to-expect-when-eths-expecting-80cb4951afcd)

