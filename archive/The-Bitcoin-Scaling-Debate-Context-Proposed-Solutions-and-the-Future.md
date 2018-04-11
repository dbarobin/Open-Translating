# The Bitcoin Scaling Debate: Context, Proposed Solutions, and the Future

![](https://i.imgur.com/zCSz3H0.png)

[Source](https://scalingbitcoin.org/) 

A familiar critique of Bitcoin is that “it does not scale” in the sense that, as it is currently implemented, the network is not capable of supporting a global payments system that requires many thousands of transactions per second. At the moment, this is true; Bitcoin can support [up to 7 transactions per second](https://link.springer.com/chapter/10.1007%2F978-3-662-53357-4_8) as compared to the 2,000 transactions per second typically processed by Visa (with [the potential to scale to an estimated 56,000 per second](https://usa.visa.com/dam/VCOM/download/corporate/media/visa-fact-sheet-Jun2015.pdf) ).

**This critique is incomplete, however, because it does not address whether Bitcoin *has the potential to scale.* The more interesting questions to ask are:**

* Is it possible for Bitcoin to scale to process more than 7 transactions per second?
* If Bitcoin can scale to support more transactions per second, how?
* If there is more than one viable solution, which is the best one?
The Bitcoin scaling debate has been going on almost as long as the cryptocurrency itself has existed. This piece will provide context for the Bitcoin scaling debate, then review the proposed solutions and look to the future to determine if Bitcoin can scale to process thousands of transactions a second and, if so, how.

It is also important to keep perspective and recognize that Bitcoin can still be highly valuable even if it is unable to process thousands of transactions a second. Arguably, Bitcoin has already proved significant value by demonstrating over almost a decade to be resilient to attacks.

Over the years, many different proposals have been presented as solutions to increase Bitcoin’s limited transaction rate. One of the most popular and persistent proposals has been for an increase in the block size used by Bitcoin, which is currently 1MB. Transactions are grouped together into a block and validated by nodes on the network, which means that a larger block size allows for more transactions to be batched and processed per block (each block is registered [roughly every 10 minutes](https://coincenter.org/entry/how-long-does-it-take-for-a-bitcoin-transaction-to-be-confirmed) ). Historically, Bitcoin’s block size was set at 1MB as a means of limiting spam transactions and DDoS attacks (though there is no conclusive statement on this; [it has been reported that Satoshi incorporated a 1MB block size into the codebase without notice then later provided these reasons when questioned](https://en.bitcoin.it/wiki/Block_size_limit_controversy) about the decision). Changing the block size, however, has long been controversial as a larger block size also reduces the number of miners who can successfully compete to validate transactions. As explained by [BitcoinWiki](http://therefore/,%20larger%20blocks%20lead%20to%20less%20hashers%20running%20full%20nodes,%20which%20leads%20to%20centralized%20entities%20having%20more%20power,%20which%20makes%20Bitcoin%20require%20more%20trust,%20which%20weakens%20Bitcoins%20value%20proposition.), “Larger blocks make full nodes more expensive to operate. Therefore, larger blocks lead to less hashers running full nodes, which leads to centralized entities having more power, which makes Bitcoin require more trust, which weakens Bitcoins value proposition.” For this reason, some in the community are concerned that increasing the block size of Bitcoin would put the decentralized nature of the network at risk.

More recently, Bitcoin soft forked ( [here is an explanation of cryptocurrency forks](https://hackernoon.com/an-explanation-of-cryptocurrency-forks-65d79efe214c) ) to incorporate Segregated Witness (SegWit), which Wikipedia explains as, “an update aimed at solving [transaction malleability](https://en.wikipedia.org/w/index.php?title=Transaction_malleability&amp;action=edit&amp;redlink=1), a known weakness in bitcoin’s security. Segregated Witness is a system by which the signature data is segregated from other transaction data. Segregated Witness has been proposed as a solution for scaling, and has impacts in two ways. It changes how data is stored in each bitcoin block. SegWit provides a boost in transaction capacity while remaining compatible with earlier versions of bitcoin software. It fixes transaction malleability that has been a roadblock for other bitcoin projects. SegWit allows for an easier implementation of the [Lightning Network](https://en.wikipedia.org/wiki/Lightning_Network).”

This ongoing debate led to a hard fork of Bitcoin in August 2017 and the creation of Bitcoin Cash, which replicates the original Bitcoin protocol but increase block sizes to 8MB (find more on the differences [here](https://www.investopedia.com/tech/bitcoin-vs-bitcoin-cash-whats-difference/) ).

As described above, Segregated Witness (SegWit) was implemented as a soft fork to Bitcoin in July 2017, which doubled the amount of information stored in each block. Perhaps more importantly for Bitcoin’s long term scaling potential, SegWit also enables second-layer transaction networks like Lightning Network. As described in the Lightning Network white paper, “The Lightning Network is a decentralized system for instant, high-volume micropayments that removes the risk of delegating custody of funds to trusted third parties. … Micropayments, or payments less than a few cents, are inconsistently confirmed, and fees render such transactions unviable on the network today. The Lightning Network solves these problems. It is one of the first implementations of a multi-party Smart Contract (programmable money) using bitcoin’s built-in scripting. The Lightning Network is leading technological development in multiparty financial computations with bitcoin.” Lightning Network introduces a solution to Bitcoin’s scaling problem by enabling transactions to take place “off chain” which removes burden from the network. As the white paper continues, it is implemented as follows, “Funds are placed into a two-party, multisignature “channel” bitcoin address. This channel is represented as an entry on the bitcoin public ledger. In order to spend funds from the channel, both parties must agree on the new balance. The current balance is stored as the most recent transaction signed by both parties, spending from the channel address. To make a payment, both parties sign a new exit transaction spending from the channel address. All old exit transactions are invalidated by doing so. The Lightning Network does not require cooperation from the counter party to exit the channel. Both parties have the option to unilaterally close the channel, ending their relationship. Since all parties have multiple multi-signature channels with many different users on this network, one can send a payment to any other party across this network.” Lightning Network essentially brings a smart contract-like capability to Bitcoin transactions in a way that allows transactions to take place off chain.

Lightning is still at an early development stage but has shown promise in potentially reducing the transaction load faced by the Bitcoin network. Lightning Network also introduces the technology for other second-layer off-chain approaches, like Plasma for Ethereum. These second-layer networks show the most concrete progress towards scaling Bitcoin’s transaction rate.

Inevitably, increasing the block size will be reintroduced as a solution just as it has for the past few years. The debate will continue about just how much risk increasing block size creates for a potential loss of decentralization. One important note, however, about the practicality of increasing the block size used is that increasing the block size only improves transactions per second linearly. Increasing Bitcoin’s block size to 8MB (as Bitcoin Cash has done) would only enable a theoretical 56 transactions per second (7/txs * 8x increase in block size) while global payment networks like Visa regularly process 2,000 transactions a second. This means, then, that increasing block size appears to be a near term solution to a larger structural problem that might better be addressed by solutions like a second-layer network.

It is too early to tell if Bitcoin will be able to scale to accommodate thousands of transactions a second or if the community even collectively agrees it should. If it does end up scaling, it will be fascinating to see if the changes required come from modifications of the underlying blockchain or if they come from solutions “up the stack”, like second-layer networks, that maintain the traditional Bitcoin blockchain layer but build on top of it. History suggests that Bitcoin developers strongly prefer maintaining the current block size and protocol and would much rather see adaptations built on top to accommodate transaction volume. Additionally, new developments like SegWit may enable solutions that cannot be anticipated.

**I’m trying something new:** if you’d like to chat about cryptocurrencies or anything else technology related drop me a line at philjglazer@gmail.com.

**Note: I do not and will not provided investment advice or recommendation.**

![](https://i.imgur.com/qcnJnaU.png)

[The Bitcoin Scaling Debate: Context, Proposed Solutions, and the Future](https://hackernoon.com/the-bitcoin-scaling-debate-context-proposed-solutions-and-the-future-579f9373e24b)