# Proof-of-authority \(PoA\)

In PoA-based networks, transactions and blocks are validated by approved accounts, known as validators. alidators run software allowing them to put transactions in blocks. The process is automated and does not require validators to be constantly monitoring their computers. It, however, does require maintaining the computer \(the authority node\) uncompromised. With PoA individuals earn the right to become validators, so there is an incentive to retain the position that they have gained. By attaching a reputation to identity, validators are incentivized to uphold the transaction process, as they do not wish to have their identities attached to a negative reputation.

This is considered more robust than PoS, as:

* In PoS, while a stake between two parties may be even, it does not take into account each party’s total holdings. This means that incentives can be unbalanced.
* PoW uses an enormous amount of computing power, which, in itself lowers incentive

## Establishing authority

The three main conditions that must be fulfilled for a validator to be established are: 1. Identity must be formally verified on-chain, with a possibility to cross-check the information in a publicly available domain 2. Eligibility must be difficult to obtain, to make the right to validate the blocks earned and valued. \(Example: potential validators are required to obtain public notary license\) 3. There must be complete uniformity in the checks and procedures for establishing an authority

## Used in

* [POA.Network](https://poa.network)
* [Ethereum Kovan](https://kovan.etherscan.io)
* [testnet Rinkeby](https://gist.github.com/cryptogoth/10a98e8078cfd69f7ca892ddbdcf26bc)

## Pros

* High throughput; scalable
* No mining mechanism like in PoW, PoA uses identity as the sole verification of the authority to validate,
* PoA is suited for both private networks and public networks
* PoA only allows non-consecutive block approval from any one validator, meaning that the risk of serious damage is minimized.

## **Cons**

* By identifying validators it is a centralized system

## Read more

[Wikipedia](https://en.wikipedia.org/wiki/Proof-of-authority)

