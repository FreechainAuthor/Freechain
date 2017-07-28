# _**Freechain**_
-----------------

Please read the pdf white paper under https://www.dropbox.com/s/0z267djvhv1s6dg/Freechain_V01.pdf?dl=0

If you want to support this project financially please send any amount of bitcoins to 167BDaSPqCntEX8xZsAQzpwaoZZkStdYz6

# Summary

During the last years many blockchains have emerged for record keeping as it came clear the bitcoin blockchain will never be able to host financial transactions and data records both. Most of these blockchains are touted for business use cases by well funded startups. The value of their tokens are fluctuating heavily on exchanges due to speculative frenzy. This in turn makes the use of these blockchains less user-friendly as the future costs of using them is hard to predict.

It is important to understand that no blockchain can exist without a token to charge the users to put data on that blockchain. But it is possible to minimize the speculative attractiveness of such a token. The token has effectively to be de-monetized. This means the token shall not resemble a (digital) currency anymore. Freechain will have a token which will differ in the following ways from most other blockchain tokens to prevent speculation:

*	It is not possible to transfer the token from one address to another (except fees which are collected by the miner).
*	Tokens held by an address longer than 1’000’000 Blocks (approximately 2 years; target block time is 1 minute) will not be spendable and essentially worthless even if present in the blockchain.
*	Every new block mined must send the earnings (miner reward and transaction fees) to new addresses not used before. This is the only way to generate new addresses in the blockchain.
*	An address can never be topped up.
*	The mining reward is increasing over time. This will prevent speculative mining. Users should mine tokens only shortly before they need them to store data on the blockchain.

Freechain is open source and aims to be fully decentralized. Especially the mining of Freechain shall be decentralized as the points above encourage each user to mine his own token needs.

The representation of physical and virtual objects (“coloured coins”) is possible with Freechain. A syntax proposal is given in chapter  7 below. Certain aspects which have to be considered when using Freechain to represent physical and virtual objects are discussed. 

It should be clear that by sacrificing the token transmittal feature of transactions, certain use cases will not be possible with Freechain. Remittances, smart contracts or decentralized applications based on smart contracts are not foreseen to be implemented. For these features the use of existing blockchains such as bitcoin and ethereum are recommended. However it is possible to store code in a transaction which can be executed by anybody using a suitable interpreter or compiler. 


# 1	Using Freechain

A main goal of Freechain is that users who want to use Freechain generally  mine the tokens they need themselves:

*	If a user doesn’t have enough computing power to solve a block and collect the mining reward himself he should join a mining pool.  The user generates a new address and transmits it to the pool. The private key to the address is kept safe by the user. The pool uses the address as one of the reward addresses. When the pool solves a block the user gets credited a fraction of the mining earnings (reward and transaction fees) proportional to his computing power. The user gets notified by the pool and can then use the amount on his address. If he wants to continue mining with the pool he must generate a new address and transmit it to the pool.
*	If not enough tokens can be mined by a user because he does not have enough computational power, he should never directly buy an address with some token. The miner selling the address could sell it to other persons or use it for storing data in the blockchain himself. Either way the user looses some or all of the purchased token.
*	Instead this user should use a cloud mining contract to acquire more tokens. The user generates a new address and transmits it to the contract miner. The private key to the address is kept safe by the user. The miner uses the address as one of the reward addresses. When the miner solves a block the user gets credited the amount as agreed in the contract. The user gets notified and can then use the token on his address. The cloud mining contract is best stored in a smart contract (e.g. ethereum)  to make sure the user really gets his token and the miner gets paid after mining it.
*	Users are discouraged to hoard tokens because they will loose their value after 1’000’000 Blocks (approximately 2 years). Additionally the mining reward is increasing over time therefore it’s more economical to mine later. They should only (cloud) mine tokens when they intend to use them shortly. Freechain tokens are meant to live from hand to mouth. 
*	Traditional exchanges where users can buy and sell tokens cannot trade Freechain tokens because they cannot be transferred between addresses. It is expected that a new form of marketplace will appear which is rather a platform that bring users and cloud miners together and help them setting up the mining contract.

# 2	Tokens and rewards

Users which currently don't need tokens to store data on the blockchain are encouraged to mine only with a small fraction of their spare computing power. This helps to keep the network distributed and healthy. This behaviour is called “non-profit  mining”. The costs for the user are negligible if the user's computer is running and connected to the internet anyway. But why should anybody do this for free?

Many people around the globe donate computing power and disk space to projects of the BOINC network in a philanthropic intent without financial compensation. Well known is for example the SETI@Home project to search for extra terrestrial intelligence. It is expected that many people will donate a little bit of spare computing power and disk space to Freechain since a non-profit oriented blockchain is a fundamental achievement for humanity.

This non-profit approach for large participant mining is new for blockchain technology altogether. It may pose some challenges for the network (e.g. latency, bandwidth etc) to have so many active miners but overall it is seen as a clear benefit. Non-profit miners are more likely to obey the rules and act honest compared to profit miners. Non-profit miners are encouraged to mine themselves and not via a pool as their aim is to keep the network distributed and healthy.

Non-profit miners should only mine with a small amount of spare computing power as long as they don’t need more tokens to store their own data in Freechain. This way the difficulty is not raised too much for other users who need tokens.
If a user needs more tokens for storing his own data in Freechain he can ramp up the mining effort to increase the chance of winning a block and join a mining pool if needed. This behaviour is called “power mining”.

Non-profit miners are encouraged not to sell any tokens they don’t need themselves. Instead they should reduce the computing power they use for Freechain until they need more tokens or when they detect that the network is attacked (see chapter 6 below). Unused tokens will become invalid after approximately 2 years. This is not a problem for the network as there is always fresh supply of tokens. If a non-profit miner does not want to have his tokens invalidated he can donate the tokens (in fact sharing the private keys to the addresses holding them) to a charity organization that wants to store data in the blockchain.

## 2.1	Rewards

The reward for a solved block is 1 full token in the beginning and then increases. It can be split on several addresses but all addresses must be new i.e. have never been used in the blockchain before. After 50’000 blocks the reward increases by 1%. After 500’000 blocks (approximately 1 year) the reward has increased 10 times by 1%. The block reward is then
1.01^10 = 1.1046 token
This will lead to significant inflation but the exact inflation is not easy  to predict because tokens are worthless/unusable after 1’000’000 blocks (approximately 2 years). If the users spend all tokens before they invalidate the inflation and tokens in circulation are shown in the [see graph in the pdf white paper].

The inflation is extremely high in the beginning but will stabilize after 30 years  at approximately 10.5%. The high inflation in first years  should deter speculative mining in the beginning even if utilization of Freechain is progressing very quickly i.e. all tokens are used before they expire. If no tokens are used before they expire the inflation and tokens in circulation are shown in the [see graph in the pdf white paper].

The inflation stabilizes after 3 years at approximately 10.5%. If no tokens are used before they invalidate it is a sign that Freechain isn’t gaining traction quickly and therefore a modest inflation is sufficient to deter speculative mining. Note that in this case no transaction fees are paid and collected by miners. If a part of the tokens is used before they expire the curves are in between but the inflation stabilizes after some years at 10.5% as well.

The tokens in circulation go to infinite. This will deter investors definitely but is no problem for users who want to store data in the blockchain. 

The block reward grows by a factor of 10 approximately every 23 years. Should the numbers become too large, a merge of 1’000 tokens into 1 can be performed after 69 years for practical purpose. The block reward would at the same time shrink by a factor of 1000.

## 2.2	Fees

As Freechain can theoretically survive only with non-profit mining - the only necessity to have tokens is to charge users to put data on the blockchain. Therefore the transaction fees are of great importance.

The space in Freechain for 1 transaction is much less limited than in bitcoin (with the OP_return function currently only 80 bytes are accepted by the bitcoin client). A transaction in Freechain can be at maximum 1/1000 from the current block size limit (in the beginning 10 MiB/1000 = 10 KiB). However a user can submit many transactions in a short time and fill up significant amount of data in a block. Since there is always too little space for some people/applications, the fees are very important to limit the amount of data a user can store.

It has to be anticipated that there is frequently more demand to put data on the blockchain than there is available block space. This, if not properly handled would lead to an unsatisfactory user experience. There is no question that if many users want to put a lot of data on the blockchain, the fees will rise as space is limited.
The data which is most valuable to the users or at least the data where users are willing to pay the most should be stored in the blockchain. If a user decides after transmitting a transaction that he is willing to pay higher fees for his data he can use the feature “replace by fee” which is explained in the next chapter.
The minimum fee is such that a full block will yield the same amount of fees as the standard mining reward (1 token). To calculate the minimum fee the formula is therefore

Fee (in Token) = size of the transaction (MiB) * current mining reward (in Token) 
                                                        current maximum block size (MiB)
                                                        
If there are more transactions awaiting than block space, the profit oriented miners will prefer the transactions with higher fees. However the bitcoin client sets a priority for transactions which considers the age of the transaction in an attempt to not let unconfirmed transactions getting too old.

The older a not processed transaction gets the higher the priority becomes. Bitcoin transaction priority is calculated as a value-weighted sum of input age, divided by transaction size in bytes:

Priority in bitcoin = sum(input_value * input_age)/size_in_bytes

Freechain does not have input values (except the fee itself) therefore in the Freechain Client the priority is depending on the fee and the transaction age itself:

Priority in Freechain = sum(fee_value * transaction_age)/size_in_bytes

It has to be noted that transaction age is not an absolute value, it depends on when the miner receives the transaction. It is anticipated that non-profit miners will stick to the default priority setting. Profit oriented miners however, as in bitcoin mining, may choose to take over only the transactions with the highest fee per size ratio. 

Why is the age of the input token not considered as in bitcoin? This would pose an incentive to use (and possibly hoard or buy) old tokens and would be detrimental to demonetizing the token. Instead the age of the transaction is used. 

## 2.3	Replace by Fee (RBF)

Already in the early versions of bitcoin existed a mechanism which is called “replace by fee”. The RBF mechanism in bitcoin was disabled due to security concerns by Satoshi himself in 2010 and activated again in Bitcoin Core 0.12.0 in 2016. It is explained in more detail in https://en.bitcoin.it/wiki/Transaction_replacement

The purpose of RBF is to speed up the confirmation of a transaction by increasing the fee after the transaction has been broadcasted already. If a protocol does not allow this mechanism explicitly, an updated transaction would be seen as a double spend attack and network nodes would not accept the updated transaction. Therefore it is important to have this feature described in detail here. For Freechain this feature is even more important because it is expected that at times there is much higher demand to store data in Freechain than available block space. In such a situation it must be possible for users to speed up the confirmation of their transaction by increasing the fee after the transaction has been transmitted already.

There has been a lot of controversy in the bitcoin community about this topic. The logical solution to only update the transaction with a higher fee input is called first seen safe (FSS). The transaction content and outputs must otherwise remain identical.  FSS RBF is not easy to implement in the bitcoin protocol and impractical for users due to the bitcoin transaction structure. Furthermore it would reduce the anonymity of bitcoin because the change address is clearly visible for all network participants. Refer also to this article for further reading: http://blog.greenaddress.it/2015/12/09/why-replace-by-fee-is-good-for-bitcoin/

In Freechain it is much easier to use FSS RBF. The transaction data content is not allowed to be modified. Allowed changes are only the fee amount and the change amount. Since in Freechain no value transfer is allowed, the input address is always the output address for the change. If the input address does not hold enough value to increase the fee, another input address can be added. In such a case the added address must receive the change and the first input address must be depleted completely.
 
# 3	Block structure

The maximum allowed block size is 10MiB in the beginning and then follows almost Nielsen’s Law for Bandwidth and Moore’s law for computing power:  The block size will double every 1’000’000 Blocks (approximately 2 years). This results in exponential growth which is needed for large user adoption but should be manageable from a hardware perspective.

As Moore’s law may not continue forever, the miners shall have a veto right to prevent the doubling of the block size. If 30% of the 50’000 blocks before the rise are tagged by the miners to not increase the block size the block size will not increase for another 1’000’000 Blocks. Note that the miners must take action to prevent increase of the block size not vice versa.
Because Freechain is specifically designed for record keeping and time stamping, the transaction is somewhat shorter than in bitcoin protocol (no need for the OP_return tag).

In order to scale Freechain to a large enough database and reduce the need of full nodes, every user can select to store only full blocks where he has transactions in it. From blocks he has no transactions in it he will only store the block headers. This will probably be the preferred method for mobile devices and users with limited storage capacity.

If a user wants to prove a certain data record, it is sufficient to disclose the transaction itself, the hash of the transaction and all the hashes along the merkle tree up to the merkle root. The merkle root is stored in the block header which every user should have locally available down to the genesis block. This is similar to the simplified payment verification approach described by Satoshi Nakamoto in the bitcoin white paper.

The Freechain Client will not accept empty or too low filled blocks when there are too many unconfirmed transactions. This flaw known from the bitcoin blockchain is prohibited in Freechain. The Freechain client denies blocks if these conditions are fulfilled

*	The block is smaller than 99% of the current maximum block size and
*	Unconfirmed transactions amount to more than 100% of the current maximum block size

# 4	Mining and proof algorithm

## 4.1	Proof of Work against Proof of Stake

Proof of stake algorithm is more energy efficient but seen as less safe. The algorithm to choose who’s to mine the next block is perceived as a potential weakness. Furthermore the “nothing at stake” problem is not easy to solve, refer also to https://en.wikipedia.org/wiki/Proof-of-stake#Criticism 

For these reasons a proof of stake approach is dismissed for Freechain.

## 4.2	Proof of Work algorithm

The proof of work algorithm must be such that specialized hardware doesn’t bring a significant advantage. If the same algortihm as in bitcoin (SHA-256) would be used, the users with access to ASIC hardware would have such a tremendous advantage that normal users wouldn’t have any chance to win a block. For Freechain it’s planned to use a memory hard algorithm similar to Zcash or ethereum. These algorithms are designed in a way that the memory bandwidth is the bottleneck, not the computing power. Therefore adding computing power by ASIC without adding memory bandwidth doesn’t bring an advantage.

Recent advancements in the field of memory hard PoW algorithms have improved the speed and memory requirements for verification (“Equihash: Asymmetric Proof-of-Work Based on the Generalized Birthday Problem”, Biryukov and Khovratovich, 2016). It is expected that there are further developments on optimized PoW algorithms therefore the PoW algorithm may be updated in a later stage. 

Freechain will only be attractive for large professional miners when they can sell their hash power in cloud mining contracts. When most users run the PoW Algorithm to meet their own demand of tokens ideally only relatively few cloud mining contracts are ordered. This way Freechain mining will remain a niche market for large professional miners and there is less incentive to develop specialized hardware for it’s PoW algorithm.

# 5	Inadequate content filtering vs censorship

A big problem is if users store data on the Freechain blockchain with inadequate content e.g. anything which violates human rights. This problem is generic to all public blockchains but worse in Freechain since it allows larger amounts of data in one transaction. It is the opinion of the author that as for the internet itself, search and service providers should provide efficient filters to hide inadequate content from users/readers by default. If a user turns off such filtering it is at his own responsibility. Nevertheless the blockchain should not be a help to distribute and store inadequate content in eternity. On the other hand content filtering is a sort of censorship and who decides what content shall be stored and what not? A balanced approach is described as follows:

Every miner / user / full node is free to prune inadequate content out of a block and only keep neutral aspects of the block such as the merkle tree, the transaction signatures and the block header. The transaction signatures shall be designed in a way that allows to verify that the transaction has been signed by somebody who has the private keys to the input addresses even if the transaction data content has been deleted.

Censoring lists powered by wiki collaboration can help miners/users/ full nodes to prune inadequate transaction data shortly after the block is mined based on the transaction hash. This way not every user has to scan the blocks for inadequate data himself.

The above described censoring is considered fair because although inadequate data will not disappear completely unless the very last node has removed it from his local blockchain at least it will be stored fewer times and has therefore smaller redundancy. On the other hand the censoring cannot erase content of a minor group of users.  The author believes this is the best compromise between user freedom and user protection.

Imagine one single user wants to store some really sick data all other users/nodes/miners find inadequate. If all other users remove this data from their local blockchains there is no redundancy at all. Moreover this user has to provide the content himself every time another user wants to read this transaction. This way most benefits of a blockchain disappear for this particular data. The only leftover in the pruned blockchains is a hash proving this data existed at that time. This benefit could have been achieved by the user in a cheaper and better way by only saving the hash of the data in the first place. If law enforcement wants to prosecute said user because the content is a criminal act it is easy to locate said user because no other user will broadcast this transaction content.

It is to be hoped that above facts deter users to publish inadequate data. After all, blockchains are a very democratic data structure.

# 6	Security

As one address can never be topped up, active users will use several addresses over time. These addresses are randomly generated, so how can others be sure that the transactions were published by the same user? This problem becomes more aggravated if users buy tokens directly from miners or resell the address to a second user after having used only a fraction of the tokens (although that’s not recommended).

It is encouraged that every user adds an originator signature to his transactions. This is the transaction content encrypted with a separate private key (not the private key to the input address). The public key for this signature can be disclosed off-chain (i.e. website of a company or email) or kept private and only shared with auditors / authorities or disclosed on request. The public key for this originator signature should remain constant over longer periods of time to make auditing plausible. If the private key is stolen the owner should file a transaction in clear text with the clear message that this key combination is compromised and a new pair will be used. After such a transaction all transactions signed with this key can be disregarded.

If the private key is lost (not stolen but forgotten) this entity also looses credibility in the blockchain world. It shows they don’t follow minimum data protection guidelines and can therefore not be trusted. Of course they can issue a new pair and distribute the new public key off-chain but their reputation has suffered a major blow.

Further developments on hierarchical deterministic key generation (see “Hierarchical deterministic Bitcoin wallets that tolerate key leakage”, Gutoski and Stebila, 2015) will make it much easier and safer to manage private and public keys in larger organizations by using master keys. Progress in this field shall be considered in the  Freechain client.

## 6.1	51% Attack

A 51% attack (http://en.bitcoinwiki.org/Bitcoin_weaknesses#51.25_attack) is at first glance not so dangerous for Freechain as for another blockchain. Double-spending of tokens is economically not interesting because the receiver of the spent tokens is always a miner as they cannot be transferred to another address. In the best case a 51% attacker can transfer his tokens to himself!

However the risk of double issuing contradicting records has to be considered. It is important to understand exactly what a 51% attacker can and what he cannot do. The first and foremost requirement is that a 51% attacker can only succeed if the victim (or a third party!) has no objective reason to distrust the attacker. Consequently the attacker cannot violate any of the rules a blockchain is based on. This excludes therefore the following possibilities:

*	An attacker cannot spend tokens from other addresses where he has no private key for.
*	Alter the Freechain software without consensus.
*	Cannot issue false records with somebody else’s originator signature where he has no private key for.
The following actions are possible for a 51% attacker:
*	disconfirm others’ blocks confirming only their own, thus receive 100% of all new tokens.
*	block any transaction at his discretion.
*	create 2 (or more!) competing versions of the blockchain. If he has enough hash power and time he can go further back in time and produce an alternate chain which when it has reached equal length as the true chain cannot be revealed as the attack chain by a third party. This is probably the most dangerous scenario for Freechain and blockchains in general.

### 6.2	Defense mechanisms against a 51% attack

In this chapter defense mechanisms against the various actions a 51% attacker can perform are discussed.

### 6.2.1	If a 51% attacker does not confirm other blocks thus receives all new tokens

Most users will not even notice this. Because new addresses have to be used for the miner reward at every block the blockchain itself will not show any irregularities. Attentive users might notice an increase of orphaned blocks or that the blocks which become orphaned sometimes are broadcasted earlier than the blocks that belong to the blockchain. There are now two possibilities:

a)	The users and miners discover there’s an attack. They rally to build a true (longer) blockchain than the attacker. In a conventional blockchain where mining is only done for profit the miners have very little motivation for increasing their hash power in such a situation. They have to invest additional money (for electricity, hardware or mining contracts) for more hash power to defeat the attacker at a time when the token price and thus their revenues are dwindling.
Freechain is in a better situation. Non-profit users which normally only use spare computational power (or even a small fraction thereof) can easily increase their hash power. When motivated communities are being attacked they always start to defend themselves. It’s within human nature. Therefore it must be expected that non-profit users will voluntarily increase their hash power once an attack has been identified. The attacker will soon not have a majority of the network’s hash power anymore and the attack is over.

b)	Nobody discovers there’s an attack or only an insignificant small number of users/miners believe there’s an attack. No resistance will form against the attack. After a certain amount of time the users will run out of tokens and switch to power mining to generate more tokens. The users will increase their hash power until the attacker doesn’t have a majority of the network’s hash power anymore and the attack is over.

### 6.2.2	If a 51% attacker blocks any transaction at his discretion

In this case the attacker must make sure no blocks from other miners are put in the blockchain. All blocks from other miners must become orphaned blocks. This is therefore a very similar situation as described in the previous section. However it’s not possible that nobody discovers there’s an attack. At least the user(s) whose transaction(s) get(s) blocked will realize it quickly. The user(s) can notify the community or developers about their blocked transactions and every full node can confirm that some transactions are not processed although they should have become priority due to their fee and age. This will make it evident that an attack is happening and there will quickly form a resistance against the attacker. The non-profit miners will increase their hash power as necessary. The attacker will soon not have a majority of the network’s hash power anymore and the attack is over.

### 6.2.3	If a 51% attacker creates another, longer branch of the blockchain

It is unimaginable that in such a situation the miners will not notice an attack. In fact the Freechain client identifies this situation automatically if two alternative versions of the blockchain are broadcast with both branches larger than 2 blocks. There will quickly form a resistance against the attacker. The non-profit miners will increase their hash power as necessary. The attacker will soon not have a majority of the network’s hash power anymore and the attack is over.

The honest miners can distinguish the true from the attack chain by comparing the receipt time of the blocks of the two branches.  This is in essence the core function of a blockchain – witnessing the time when an information was present. Since the consensus is then formed by the majority of the hash power agreeing on one version (one branch) the democratic nature of blockchains becomes evident.

### 6.2.4	If a 51% attacker tries to maintain 2 (or more) competing versions of the blockchain

The following attack is quite theoretical. Skip it if you’re not familiar with blockchain security.

This attack is using the same technique of broadcasting blocks some time later than they were mined as the selfish mining strategy (see “Majority is not Enough: Bitcoin Mining is Vulnerable”, Eyal and Sirer, 2013). However the selfish mining doesn’t have the aim to destabilize the blockchain but only to maximize the profits of an individual miner or mining pool compared to honest mining. Attacks to destroy the blockchain have been described as Goldfinger attack named after the James Bond movie “Goldfinger” (see “The Economics of Bitcoin Mining, or Bitcoin in the Presence of Adversaries”, Kroll et al, 2013).

[see graph in the pdf white paper]

Imagine a terrorist (or terrorist group) who wants to destabilize the blockchain by maintaining two branches in parallel (refer to the figure above). He waits until a second block is broadcast shortly after the first block with the same block height H. This second block normally would end up as orphaned block as the miners will continue the chain with the first block. However the terrorist, having 51% of the hashpower, mines a block following this second block. He is likely to be quicker to bring up a block on this second chain than the other miners on the first chain. In the optimum case the attacker releases his block shortly before the honest miners working on the first chain release a block for the first chain. 

Now miners are in an economic dilemma. Should they follow the first or second chain? Due to latency and bandwidth issues, they cannot be sure that the first chain is the correct one. If the second chain does not have obvious flaws this could be the legitimate chain as well. If miners end up on the wrong chain their rewards will be worthless. Profit miners can therefore decide to stop their expenses (save electricity) until a dominant chain has formed and then resume mining. This would inevitably be the wrong medicine. The attacker’s share of the network hash power increases therefore it’s easier for him to keep the 51% attack ongoing.

The terrorist can expect most miners to follow economic rules and switch to mine on the second chain because that block of height H+1 was broadcasted first. Therefore he mines a block back on the first chain and releases another block shortly before the other miners working on the second chain release a block for the second chain. The attacker can now always balance the two chains out so there come to exist two (or more) versions of the blockchain in parallel with the same length. This situation if kept on for longer will result in people loosing faith in the blockchain rapidly. 

Should an attacker obtain network superiority (see “Theoretical Bitcoin Attacks with less than Half of the Computational Power”, Bahack, 2014) the effort to perform this attack becomes significantly lower. Network superiority means to control a majority of network nodes and is estimated to cost only a fraction of obtaining half of the hash power. E.g. in bitcoin there are currently approximately 6000 nodes. To obtain the majority an attacker must bring up at least 6000 nodes himself. These nodes do not need significant computing power and can be run on virtual machines. If an average price of 100$ is assumed for running a node, the costs to achieve network superiority is 600’000$. The costs to achieve half of the hash power are discussed in the next chapter and more than 100 times bigger than the costs for network superiority.

This scenario is worse than all previous scenario’s because it may be difficult to detect there is an attack happening. People will start blaming the latency, bandwith or block size and in the confusion it’s hard to detect that an attacker is behind it. In the worst case the established mining pools might even accuse each other of not informing the other mining pools directly about solved blocks to gain advantage (so called selfish mining). Attackers can hide very well because a block can easily be mined in Australia but then broadcast from Zimbabwe. Critics and journalists will feast on these events and it could be a major blow to the token price.

Bitcoin miners as well as bitcoin payment processors are well advised to monitor the network for an attack if 2 (or more) competing forks emerge with a length of more than 2 blocks. However well an attacker is trying to disguise there’s an attack it is possible to detect it with high diligence. Direct communication channels between the large mining pools will help greatly to identify such an attack.

The Freechain client identifies this situation automatically when two (or more) alternative versions of the blockchain are broadcast with both branches larger than 2 blocks. There will quickly form a resistance against the attacker. The non-profit miners will increase their hash power as necessary. The attacker will soon not have a majority of the network’s hash power anymore and the attack is over.

What if the non-profit miners cannot mobilize enough hash power by their own resources? Nowadays if motivated communities are being attacked but they are not strong enough to defend themselves they pledge for help (e.g.  www.avaaz.org  and other examples).  There is a big share of good willed people out there that are willing to help motivated communities under attack without compensation. Some of these people may start becoming non-profit miners, others may donate money which can be used for cloud mining contracts or spread the information further. In the end an attacker faces not only the community against him but in essence many helpers across the globe. When the attack finally is over the community gets larger and stronger.

### 6.2.5	Attacks to the Freechain client software

If an attacker does not possess 51% hash power of the network he could still try to bring confusion to the network, for example regarding the block size debate. Some miners will inevitably feel disadvantaged with larger blocks due to bandwidth and latency constraints. They will always argue and opt for small blocks. If the attacker now deliberately produces more orphaned blocks this will act as a strong argument for these miners. Orphaned blocks are a key metric for a blockchain (see e.g. https://blockchain.info/charts/n-orphaned-blocks ). In a similar way an attacker could try to influence consensus debates for other topics which require a change to the Freechain software. These attacks will have much less severe impacts than the 51% attacks but it’s important to keep it in mind if a group of people wants to change (or preserve!) the code and argument with blockchain metrics.

Freechain is not immune against attacks to the Freechain client software by such methods. However it is easier to find consensus among developers and miners if the token is demonetized and many users are mining in non-profit mode or for their own requirements only.

# 7	Object representation (“coloured coins”)

Freechain can be easily used for physical or virtual object representation, also known as coloured coins. Physical objects that are predestined for blockchain representation are vehicles, real estate, equipments, luxury goods etc. Virtual objects that are predestined for blockchain representation are licences, permissions, certificates, websites, apps etc.

Every Freechain transaction can have large free text as content (almost 10’000 characters in the beginning). The easiest implementation is done by using tags (tag1=property1;tag2=property2 etc) to define the object. Possible tag names would be

* Name
* Manufacturer / Producer / Issuer
* Seller
* Model
* Owner 
* Lessor
* Operator 
* Lessee 
* Sublessor
* Sublessee
* Partname
* Serialnumber
* Material
* Version
* And many more

The tags can also be abbreviated to save some space. The originator for the transaction would in most cases be the manufacturer / producer / issuer or the seller, sometimes maybe a third party or a government organization. 

As opposed to bitcoin implementation of coloured coins there is no need to keep a certain coin amount on this transaction (UTXO). There is just the ordinary fee for a transaction of this size. The tags as well as their abbreviations must be standardized in order to allow compatibility between all users who want to represent physical or virtual objects in Freechain. 

In order to be a credible representation, the originator of the transaction must sign it with a private key (not the private key to the input address). The public key for this signature can be disclosed off-chain (i.e. website of a company or email) or kept private and only shared with auditors / authorities or disclosed on request. Refer also to chapter 6 above.  The easiest way would be when the originator uses the same key as for record keeping.

## 7.1	Transfer of objects

As it is not possible in Freechain to transfer tokens from one address to another there must be another way to transfer the object from one owner to another. The easiest implementation is when the originator of an object uses a tag such as the following:

* SoldTo
* DonatedTo
* TransferredTo
* LeasedTo
* LeaseBack

The tags can also be abbreviated to save some space. If the object already exists on the blockchain, the originator can refer to this object by using the tag ObjectHash= and the transaction hash representing the object. It is obvious that any transaction that wants to transfer an object without the object originator’s signature is invalid unless the new originator can prove off-chain to be entitled to it (refer also to chapter 6 above about lost or stolen private keys).

# 8	Storing Code in a transaction

As it is not possible to transfer value in Freechain from one account to another it is not possible to program smart contracts in Freechain. Hence decentralized applications based on smart contracts are not foreseen to be implemented. For such features the use of existing blockchains such as ethereum or Crypti are recommended. However it is possible to store code in a transaction which can be executed by anybody using a suitable interpreter or compiler. Initial tags can instruct which compiler/interpreter should be used. 

# 9	Conclusions

A blockchain structure for record keeping has been presented which does not need a currency or speculative asset. It’s main intention is that the users are concurrently also miners and behave in a non profit oriented way, similar to BOINC projects such as SETI@home. 

The token for the blockchain structure is mainly needed to limit the amount of data a user can put on the block chain. The token has been demonetized with several measures to reduce it’s appeal to speculators and investors.

In the Freechain blockchain much larger data amounts can be stored than in the bitcoin blockchain currently. Therefore a possible content filtering has been suggested which protects users from storing and broadcasting inadequate contents while at the same time does not act as absolute censorship. As a result, offensive contents get less of the benefits a blockchain offers.
The security of the Freechain blockchain structure has been discussed considering different attacking scenarios and defense mechanisms against attacks.

Lastly the possibility to use Freechain for physical and virtual object representation is explored. The objects can be defined and transferred to other owners by using tags. Transactions can also be used to store code in plain text which can be executed by a suitable compiler or interpreter.

# Afterword

As the Freechain token is not a currency, it should not bear the word “coin” in it’s name. Since it’s main function is to limit the amount of data a user can put on the block chain a good name for it would be Anti Bloat and Spam Token abbreviated as ABST.

Although having programmed for more than half of my live in different languages such as Visual Basic, Fortran and C++ I do not have the intention of programming Freechain myself due to lack of time and programming skills in the field of cryptography. If you are interested to contribute please add code to this repository.

If you want to support this project financially please send any amount of bitcoins to 167BDaSPqCntEX8xZsAQzpwaoZZkStdYz6


