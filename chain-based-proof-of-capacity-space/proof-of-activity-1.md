# Proof Of Activity

Combine Proof of Work component with a Proof of Stake.

## algorithm

* Mining first begins in the traditional manner, with miners vying to be the first to solve a puzzle and claim their reward. 
* The difference is that the blocks being mined do not contain transactions. 
* They are simply templates with header information and the mining reward address. 
* Once this nearly blank block is mined, the system switches to a proof of stake protocol. 
* The header information is used to select a random group of validators to sign the block. 
* These are coin holders \(stakeholders\) and the larger the stake a validator holds, the greater the chance they will be selected to sign the new block. 
* Once all the chosen validators sign the block it becomes an actual part of the blockchain. 
* If the block remains unsigned by some of the chosen validators after a given time, it is discarded as incomplete and the next winning block is used. 
* Validators are once again chosen and this continues until a winning block is signed by all the chosen validators. 
* The network fees are split between the winning miner and the validators who signed the block.

## Used in

## Pros

* Criticisms are the same as for both proof of work and proof of stake.

## Read more

