# Proof of Devotion

Similar to POI, the PoD selects the accounts with high influence. All accounts are ranked according to their liquidity and propagation \(Nebulas Rank\).

#### Algorithm

* Top-ranked accounts are selected 
* Chosen accounts pay deposit and are qualified as the blocks Validators \(Validators Set is dynamic, changes in Set may occur after Epoch change.\)
* Algorithm pseudo-randomly chooses block Proposer 
* After a new block is proposed, Validators Set \(each Validator is charged a deposit\) participate in a round of BFT-Style voting to verify block \(1. Prepare stage -&gt; 2. Commit Stage. Validators should have &gt; 2/3 of total deposits to validate Block\) 
* Block is added. Block rewards : each Validator rewarded with 1 NAS.

#### Used in

* Nebula
  * [whitepaper](https://nebulas.io/docs/NebulasTechnicalWhitepaper.pdf)
  * [Github](https://github.com/nebulasio/wiki/wiki)

