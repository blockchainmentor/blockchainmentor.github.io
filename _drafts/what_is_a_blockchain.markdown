## What Is A Blockchain?

A blockchain, also known as a distributed ledger, is a series of time-stamped transactions.  It can be thought of as a database, where the "data" is limited to transactions of some asset, possibly with some included data or comment with each transaction.

### Paper Ledger

Imagine a personal ledger on a piece of paper.  Each line of the page would hold a transaction, and each transaction would would include details of which account the funds were sent from and who the recipients were.

![ledger book](/content/images/2016/06/640px_paper_ledger.jpg)
 <small>Photo: Andreas Praefcke - Own work, Public Domain, https://commons.wikimedia.org/w/index.php?curid=3818975 </small>

### Electronic Ledger

This same ledger concept can be stored electronically in one or more files.  Accounting software, spreadsheets, and other financial programs keep transactions in files on a hard drive in a computer.

![spreadsheet](/content/images/2016/06/electronic_ledger_example.png)
A database is a general purpose store of data that can store transactions, and most advanced financial programs use some type of database to store their data.

The data in a database can be stored many different ways on the underlying storage medium, and the data can be represented to programs and to the user in varying ways.  But for simplicity, we can think of a database as a collection of spreadsheets.

### Blockchain

A blockchain is like an electronic ledger or database.  It stores time stamped transactions in files on computer hard drives.  

![simple blockchain diagram](/content/images/2016/06/simple_blockchain_diagram.png)

While the content and storage method is similar to electronic ledgers and databases, the blockchain is unique for several reasons.

* **storage location**: many copies stored around the world
* **additive only**: data is never deleted or modified, it is only added to the end
* **tamper-proof**: written data is cryptographically signed in such a way that it is infeasible to change historical data throughout the network
* **permission to write**: only one member of the network can write a block at any given time, and the rules that control this permission are established and built into the system
  
#### Storage Location

Your spreadsheet is stored on your PC's hard drive, or perhaps even in "the cloud".  You might keep a backup copy at another location, but you are the only user/maintainer of that file.

A database, such as in a typical company, might be stored on a server hard drive.  It might be backed up to another drive or storage device.  It could even be replicated (live) on another server elsewhere in the world.  But as with your spreadsheet, it will only be maintained by the company that owns it.

Public blockchains are stored as exact copies of data on many computers owned by many different people around the world.  The more participants there are in the network, the more copies of the blockchain there are.  Bitcoin and other cryptocurrencies have a built-in incentive system that encourages participants, so the network grows in member nodes and in resilience.

#### Additive Only

Your spreadsheet can be modified by you or whomever has access to it.  Records of the past can be changed or deleted, accidentally or on purpose.  Thus, without maintaining historical copies of the file, it is possible that history could be changed.

Databases likewise can be modified - unless additional rules are put in place to prevent this.  Even still, people with administrative access can usually change the rules and then modify or delete data.

A public blockchain that is built and maintained using a protocol like Bitcoin can never be changed - it can only be added to.  Plus, the data that is added to the blockchain must be validated and agreed upon by a majority of the participating nodes.

#### Tamper-proof

The way the data is written in the blockchain makes it exceedingly difficult to modify data in the past.  Each block that is written (and a block is just a collection of validated transactions) includes a cryptographic hash value that refers to the previous block.  Changing the data of a block would make the hash value change, but that hash value was already written into the following block.  Thus, changing a block from the past would require changing every block after it.  This becomes infeasible because of the rules related to write permission.

#### Permission to Write

Since multiple nodes are all maintaining exact copies of the blockchain, it is necessary to manage which node is writing blocks.  The Bitcoin system dictating which node gets write permission for the next block is called **proof-of-work**.

As [transaction processing](http://www.blockchainmentor.com/how-are-transactions-processed-mining/) nodes (miners) receive new transactions, they validate and then pack those transactions into a block.  Then they begin a repetitive computational process - a puzzle of sorts - that ends when one of the nodes finds an answer that meets the Bitcoin rules.  That node is then the "winner" and is allowed to write the next block.

This process of gaining permission to write is very time consuming.  In the Bitcoin design, the algorithm that controls the permissioning is designed such that each new block takes about 10 minutes of *proving work* (repetitive puzzle solving) to reach a successful result and be allowed to write a block.

### Future Benefit

Public blockchains, as defined by modern cryptocurrencies, are not particularly special from a storage or content perspective.  However, the rules that dictate their creation and use are new and novel.  It is these rules that enable countless new possibilities and promise improvements in many areas of business and society.

----
[^1]: Other cryptocurrencies with public blockchains have some rule system to ensure that data written to the blockchain is properly managed and validated.

