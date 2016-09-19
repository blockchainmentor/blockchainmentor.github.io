## Bitcoin Wallet

One of the first and perhaps most surprising things to learn about blockchain currencies like Bitcoin is that the coins are not actually stored in a wallet.  In fact, the "coins" do not exist anywhere!

## Where do bitcoins come from?

We [recall](http://www.blockchainmentor.com/what-is-bitcoin/) that bitcoin miners (transaction processing computers) get rewards for doing their work.  These rewards create new bitcoins.  But to be more precise, coins are not actually created; instead, the balance of a bitcoin miner's account is legitimately increased by a set amount [^n].  The miner can then transfer those coins to another person's account, and that's how bitcoins begin to circulate.  

## If bitcoins are not stored in the wallet, what is?

One or more private keys is stored in the wallet.  A private key, corresponding to a public bitcoin address, is required to *sign* a transaction.  Without a valid signature, a transaction would be rejected.  This is how all accounts and balances can be public, but only the owner of an account can spend coins out of that account.  It is similar to traditional online banking systems such that whomever has access to the login information can send money out of the account.

## Protecting Private Keys

Since access to private keys allows sending money out of an account, and since private keys are stored in the wallet, it is very important to protect the wallet from unauthorized access.  
Most wallet programs provide options for password protecting and encrypting the wallet files.  Despite having extra password protection, software key-loggers and other malware can still pose a risk.  Alternative safety measures can be taken (such as paper wallets), but that will be described in a future post.

Just as it is important to prevent unauthorized access to a wallet, it is important to protect that wallet from accidental deletion (hard drive failure, human error, etc.).  **Loss of a private key means loss of an account**, since the private key is necessary to spend money in the associated account.  Once the private key to an account is gone, any bitcoins in that account are effectively frozen - visible to the world, yet unusable by anyone!

## Spending Money

So you have your private keys, and you want to spend some money out of one of your accounts -- how do you do that?  Wallet programs also include the capabilities necessary to initiate and broadcast transactions to the bitcoin network.  With your wallet program, once you have entered the appropriate password and unlocked your keys you can specify an outgoing transaction from one of your accounts to someone else's account (address).

Once you send that transaction, your wallet program will broadcast it to the bitcoin network so the miners (transaction processors) can validate it and write it to the blockchain.

When the transaction is sent and validated by the miners, the money is gone from your account.  There is no way to reverse this.  Convincing the receiving party to return the funds is the only way to "undo".  Thus, it is important to review a transaction before sending it!

## Receiving Money

Wallet programs can also create new accounts which you can receive bitcoins to.  In a future post we will explain why it is wise to create multiple accounts rather than always using the same account (hint: storing large amounts of bitcoin in a single account is not recommended).  

The terminology and user interface may vary, but basically you tell your program that you wish to receive a payment.  The program will generate a new pair of public and private keys, storing the private key in the data file and displaying the public key for you to share with the person who is going to send money to you.  This public key can be shared as text, such as `1fS666DjXRVwWViMWPAGHsQzDrMYorWMf` or as a QR code that your wallet program might generate for you:
 
![](/content/images/2016/06/bitcoin_qr_phone_small.png) [^n]

Remember that all transactions are just records in the blockchain?  That means that accounts can receive bitcoins without the owner of the account having their wallet open.  The wallet program will update its visible balance once it is opened and it finishes synchronizing itself with the bitcoin network.

## Online Wallets

Many companies and organizations offer online wallets.  They can have a number of benefits as well as drawbacks.  Since many online wallets are not hosted by government backed and insured companies, it is possible to lose all the money in accounts stored with them.  This has happened several times in Bitcoin history and will likely happen in the future.  Unlike traditional banks where there may be a way to recover the funds, there is no recourse in the bitcoin world.

Despite that risk, it can be useful to store some money in online wallets.  Think of it as you would think of your physical wallet in your pocket.  You will go out with enough cash to cover an evening or a few days of general expenses.  You will probably not go out with all the money you own in your wallet (unless you are in a difficult period and your personal wealth is particularly low!)

An online wallet is available to you anywhere you have access to a computer and the internet.  The online wallet may be stored with an online exchange, enabling you to exchange one currency for another (such as Bitcoin -> USD, or BTC -> ETH [^n]).

## Phone Wallets

A wallet stored on your smartphone is similar to a wallet stored on your computer.  The protection mechanism may be different, such as allowing a fingerprint to unlock the wallet, but the safety concerns are similar.

One big benefit to a phone wallet is that it enables you to pay for goods or services while out, using your phone.  For example, if your local coffee cafe accepts bitcoin, you can open your wallet app, scan the shop's Bitcoin QR code, and easily send a payment.

## Paper Wallets

There are various definitions of a paper bitcoin wallet, but in minimal form it is just a private key written on a piece of paper.  There are more elaborate variations, but as explained above the private key is the critical information that must be protected.

In the case of a paper wallet, handling and storage should be treated as other unique, valuable documents are.  Burying a 100 USD note in the dirt would be unwise, and so would burying a hand-written private key on a Post-it note.

## Summary

* Your bitcoins = your private key(s).  Protect those keys accordingly.
* A bitcoin wallet = private keys + some functionality related to sending coins and displaying balance, transactions, etc.
* Multiple types of wallets exist, and current best practices often involve using many different types of wallets for different purposes.

--------
[^1]: The current reward is 25 BTC, but this will be halved to 12.5 BTC in July, 2016 as per the Bitcoin system rules.  This halving occurs approximately every four years.
[^2]: This is the Blockchain Mentor donation wallet, so feel free to send a test Satoshi [^n] if you wish :).
[^3]: Ethereum, a blockchain cryptocurrency that will be described in a future post.
[^4]: A Satoshi is 0.00000001 BTC - one hundredth of a millionth BTC - the smallest fraction of a Bitcoin that can be processed.
