## Transaction Processing, aka Mining
The computers that process transactions on the Bitcoin network are called *miners*. [^n]

## What Does A Miner Do?

These transaction processing computers (miners) provide several services:

* validating transactions
* validating new blocks proposed by other miners
* writing transaction blocks to the blockchain

In exchange for providing these services, they are sometimes rewarded with bitcoins. The mining rewards occur often enough to justify the expense of time, electricity, and computing resources. [^n]

## Who owns these computers?

Individuals, companies, organizations... anyone can run a bitcoin mining computer since the mining software is free (open source).

There are technical and resource concerns that dissuade most people from getting involved as miners, but it can be a profitable venture for some.  And thanks to the special rules of the bitcoin system, there should always be enough profitability to encourage a healthy number of bitcoin mining computers to be active.

## Simplified Mining Process

1. Miner receives new transactions.
2. Miner validates the transactions against the blockchain history.
3. Miner groups valid transactions into a "block". [^n]
4. Miner performs special *proof-of-work* calculations. [^n]
5. If the miner arrives at a calculation that satisfies the proof-of-work rules, it then broadcasts its block and solution to the other miners on the bitcoin network.
6. Other miners receive the proposed block, then validate the transactions and the block calculation, announcing their acceptance if valid.
7. Once a positive consensus is reached (at least 51% of miners agree), the new block is accepted and written by each miner to their copy of the blockchain.
8. Miners all move on to the next batch of un-processed transactions

![Bitcoin Mining Process](/content/images/2016/06/bitcoin_mining_process.png)

**Transaction validation**: new transactions are validated before being accepted.  This is easy to do since all transaction history is in the blockchain.  The current balance of any account can be accurately calculated by scanning the blockchain for transactions to and from the account in question.  If an account balance has enough to cover a transaction and the receiving account exists, then it's a valid transaction.

**Proof-of-work** and **consensus**: the complex, computationally expensive calculations required by the bitcoin system mean that it is very difficult (time and energy consuming) to get the privilege to write a new block.  This makes it practically impossible for a rogue miner to create invalid blocks that satisfy the proof-of-work requirements.  And since a consensus of the other miners is required to validate one's proof-of-work result, an attempt at creating fake or untrue data would not be accepted. [^n]

## Summary

Bitcoin mining is transaction processing following strict rules.  The novelty of this system is in the rules and in the reward mechanism that encourages people to participate in the mining activities.

We will see in future posts how these rules and mechanisms work, and we will explore alternative views of other blockchain systems.

--------
[^n]: It is an unfortunate misnomer, for several reasons.  The *miner* is first and foremost a transaction processor.  Secondly, it is a consensus validator.  Finally, while it does gain a reward of new coins for a successful job done, those coins are not dug out of the ground or even created - there is merely a valid increase in the miner's bitcoin balance.
[^n]: For bitcoin mining, very specialized hardware is necessary to be competitive (successful).  This hardware tends to consume significant amounts of electricity.  Multiple websites offer "profitability calculators" that accept parameters, such as electricity cost, hash rate (a measure of a miner's processing speed), recent global algorithm difficulty (which by design can vary), current bitcoin price, etc.  These calculators can provide a reasonable estimate of bitcoin mining rewards vs operational costs.
[^n]: In simple terms, a block is just a collection of transactions plus a reference to the previous permanent block.
[^n]: Proof-of-work is a mathematical set of operations that requires some amount of time (effort) to generate a desired result.  The details relative to the Bitcoin system are rather complex, but the idea is that it is so difficult/time-consuming to get the privilege to write a block (which must be deemed valid), it is infeasible for someone to change existing blocks (history).  It's actually much more complex, but there will be a future post on this topic.
[^n]: Consensus just means that the majority of miners must agree that a proposed block (and proof-of-work solution) are valid.
