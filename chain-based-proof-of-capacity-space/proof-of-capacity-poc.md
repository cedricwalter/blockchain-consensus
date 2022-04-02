# Proof of capacity \(PoC\)

Miners use computer storage instead of the more common energy-expensive method proof-of-work \(PoW\) which involves permanent computational operations. 

Signum mining style solves all these problems \(and is also ASIC-resistant\) by allowing HDD mining – miners secure the network with their disk space. It can be seen as a “condensed Proof-of-Work”: you compute once \(a process called plotting\) and cache the results of your work on hard disk space. Then mining only requires to read through your cache – your HDD is idle most of the time and reads through the plot files only for a few seconds for each block.

The term plotting is a name for dedicating storage space to be used for calculations in the Signum network. A Plot is a file containing pre-computed hashes that can be used to forge blocks for the Signum blockchain. The plots are later used by mining software and can be thought of as the miner’s hash rate.

## Algorithm

1. **Plotting:** Miners pre-generate chunks of data \([_plots_](https://signum.community/signum-plotting-technical-information)\), containing all the computations necessary to forge blocks.
2. **Reward assignment:** Miners join a pool by defining it as beneficiary who will get the SIGNA reward should they find a block.
3. **Mining:** The mining software automatically reads through the plots and tries to [forge each block](https://signum.community/signum-mining).

## Terms

* **Shabal** is the name of the crypto/hash function used in Burstcoin. Shabal is a rather heavy and slow crypto in relation to many other like i.e. SHA256. Because of this it makes it a good crypto for Proof of capacity coins like Burstcoin. This is because we store the precomputed hashes while it is still fast enough to do smaller live verifications. Signum uses the 256bit version of Shabal also known as Shabal256.
* **Hash / Digest** A hash or digest in this context is a 32Byte \(256bit\) long result of the Shabal256 Crypto.
* **Nonce** When generating a plot file, you generate something that is called nonces. Each nonce contains 256 Kilobyte of data that can be used by miners to calculate Deadlines. Each nonce will have its own individual number. This number can range between 0-18446744073709551615. the number is also used as a seed when creating the nonce. Because of this each nonce has its own unique set of data. One plot file can contain many nonces.
* **Scoop** Each nonce is sorted into 4096 different places of data. These places are called scoop numbers. Each scoop contains 64byte of data which holds 2 hashes. Each of these hashes are xored with a final hash \(we get to final hash in generating a nonce chapter\).
* **Account ID** When you create your plot file it will be bound to a specific Signum account. The numeric account ID is used when you create your nonces. Because of this all miners have different plot files even if they use the same nonce numbers.

## Used in

* **Signum**
  * The Signum mining system relies on the existing free space on your hard drive, instead of energy hungry CPUs and GPUs. 
  * Anyone can mine with the same chances since hard disks are easily available at low cost.
* **SpaceMint** employs a consensus protocol based on a non-interactive variant of proof-ofcapacity \(called proof-of-space\), where participants generate and commit to a unique hard-to-pebble graph.
* **Permacoin** repurposes Bitcoin’s PoW with a more broadly useful task: providing a robust, distributed storage. In PermaCoin, eligibility for the leader election requires participants to also store segments of a large ﬁle. The ﬁle is distributed by an authoritative ‘dealer’ who signs ﬁle blocks. To provides censorship-resistant ﬁle storage, the ﬁle is fully recoverable from the participants in the event of a dealer failure or shutdown.


## **Pros**

* Livial energy consumption.
* Fairer than PoS, since disks are cheap and available = lower barrier entry
* Fast low cost blockchain transactions

## **Cons**

## Attacks and Mitigation

