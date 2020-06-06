## Welcome to the SperaxBDLS Protocol Documentation. This Doc is for anyone who wants to learn about Sperax!


### 1.1 What we do: 

Sperax builds TRUSTED infrastructure for decentralized economy. We mission to deliver accessible decentralised financial services for everyone. With our original blockchain design, Sperax BDLS consensus protocol ensures highest-level security and performance. On top of it, Sperax issues a native multi-currency stablecoin, the first in the public blockchain ecosystem, to bridge the gap between Internet users and crypto-native applications. <br /><br />
For more, please see our [website](https://sperax.io/), [BDLS package](https://godoc.org/github.com/Sperax/bdls), [whitepaper](https://sperax.io/speraxWhite.pdf), [Blogs](http://medium.com/sperax), [twitter](https://twitter.com/sperax_io), [Telegram](http://t.me/sperax).


### 1.2 Who are we: 

Speras was initiated and incubated by BitAsset Labs and NewStyle Capital. This project is proposed by Prof. Yongge Wang, an outstanding cryptographer from the University of North Carolina. Prof. Wang is the inventor of Post-Quantum Cryptographic technique RLCE, which is accepted as the candidate for NIST (National Institute of Standard Technology) standard.

Sperax is a hardware-based solution to improve privacy protection and TPS with innovative consensus mechanisms Proof of True Randomness (PoTR). This project achieves more decentralized than EOS and, meanwhile, has better performance than Ethereum. There are many innovations in Sperax, as follow:
* Community democracy and decentralization: no super nodes/users, realize global one-machine-one-vote elections;
* High performance and scalability: STPS reaches 10 thousand, while more than 2 thousand different projects runs on SperaX and more than 20 million people initiates transactions and submits smart contracts on the chain;
* Anti-quantum security and trust: lattice encryption and trusted computing chips resist quantum computing attacks and establish strong trust relationships among users;
* Privacy protection: account information, addresses, detail transaction and personal information are reliably protected;
* Secure virtual machine: use intelligent formal verification and WebAssembly instruction set standards to improve the security and execution efficiency of smart contracts;
* Economical and environmentally friendly: The competition for mining does not consume unnecessary energy and achieve green environmental protection.

Sperax project has established research and development teams both in China and the United States to conduct collaborative research and development. Moreover, we have completed the feasibility research of key technologies, simulation and testing of key modules, and detail design. Currently, SperaX team is developing key modules for testnet, which will be launched soon. 


### 1.3 How SperaxBDLS solves real-world Blockchain problems?  

| Problems In Designing A Secure PoS Blockchain  | Discover Sperax BDLS |
| ------------- | ------------- |
| **Hard to ensure unpredictability and verifiable fairness of node identity** <br /> In a PoS based consensus protocol, validators are selected to generate or vote for new blocks based on whether they satisfy certain conditions. These conditions are generally determined by the coins each node controls on the network. It is important to ensure the fairness of selection. However, though quantities like future block hashes, block difficulty, or timestamps seem to be ideal sources of randomness on chain, they are vulnerable to manipulation by miners. | **Secure and Unpredictable random beacon or RANDAO** <br /> <br />RANDAO not only has the characteristics of unpredictability, but it is also more accessible and provably fair. RANDAO’s protocol adopts a commit-reveal process that presents a joint random number, generated from the random strings committed by various participants in a given window of time. After a user gets this shared random number via RANDAO, one can then generate his/her own random number via some hash function.|
| **Hard to design a secure protocol in the open internet Environment** <br />Most current BDLS protocols apply the gossip-based broadcast protocol, based on the existence of reliable peer-to-peer communication channels, for any pair of participants one might select. This requirement is generally equivalent to a complete network topology that only exists in closed environments. This assumption is definitely not the case in more realistic scenarios on the open Internet where we interact. Open networks are particularly susceptible to DoS attacks. | **Security design in the type II partial synchronous networks** <br /><br />Among partially synchronous networks, there are two widely accepted main types, illustrated here. In the type II network, a realistic one, Denial of Service (DoS) attacks are allowed and no reliable broadcast channels are assumed before GST. We may assume that the network alternates between good and bad synchronous periods. SperaxBDLS adopts block-lock mechanisms & block self-proof mechanisms to ensure security against such potential forks, proving liveness and safety of the BDLS protocol.|
| **Hard to handle the problem of deadlock in a partial sync network** <br />Liveness guarantees that all the nodes eventually agree on some value and move on. However, in the realistic network, many attacks can be launched in the format where a malicious leader sends different messages to different nodes. Some popular BDLS protocols may reach deadlock when the network is partially sync. This deadlock is not resolved when the network regains synchronization because their liveness is not robust enough to survive in a realistic Internet environment.|  **High efficiency consensus algorithm design** <br /><br />Scalability is one angle to evaluate blockchain systems. Another way is to understand the complexity of the messages passed. Although in general the performance of PoS consensus varies with the implementation, it can also be evaluated on the order of O(n2). In terms of the communication processes in SperaxBDLS however, there are only two unicast and two broadcast processes, with a O(4n) message complexity, which contributes to a linear consensus efficiency.|<br /> <br /><br /><br />


### 2.1 Token Economy
The common practice for constructing a public blockchain stack is to build up the Layer 1 chain and then develop decentralised applications on top of it. There are technologies that help to facilitate more optimal network transactions (Layer 0). There are scalability and privacy solutions added to a public blockchain system to enhance performance and reduce cost (Layer 2).

In order to enable a truly decentralised economic ecosystem and incentivise developers to join, **Sperax issued two tokens - SPA and stable coin.** 

| SPA  | Stable coin |
| ------------- | ------------- |
|SPA is the native utility token for the Sperax blockchain. It fuels the ecosystem and reflects the value of the network. SPA also grants token holders the right to participate in the governance process in the system. <br /> <br /> Read token economics paper >>>| Sperax stable coin is a fiat-pegged stablecoin issued on the Sperax blockchain. It is also the first native stablecoin in the ecosystem. Sperax stable coin could lower the barrier of blockchain adoption for users.<br /> <br /> Read stability analysis paper >>>|

### 2.2 Use cases
:one:<ins>Payment Systems</ins>

Sperax offers a global payment system based on stablecoins. Since it is based on a single currency, Sperax stablecoin could be used in respective markets to fulfill the need for payment similar to credit cards or mobile-based payment solutions. We work with payment gateways and merchants for the infrastructure so that SST could be more widely accepted. 


:two:<ins>Global remittance and transfer</ins>

Sperax stablecoin network could support fast global transfers at a low cost. In designing the Sperax stablecoin network, we took into account the best practices of the current global currency transfer processes and leveraged on the features of blockchain technology to reduce the time and cost. Liquidity service providers act like the money transfer companies in our stablecoin network. 


:three:<ins>Decentralised financial services</ins>

Financial applications can build on our infrastructure. All the single-currency stablecoins are also issued on chain; considering that Sperax blockchain is compatible with the Ethereum Virtual Machine, a lot of the decentralised financial applications could also be supported by the Sperax stablecoin system. Sperax Foundation will build the first group of protocols to support basic currency features such as compound interest, lending and borrowing, token swaps etc. More complex financial products could be added by developers.

### 3.1 Find a bug and get rewards! 
We invite all blockchain enthusiasts to find security vulnerabilities and help us keep our protocol safe. <br />
Contact bounty@sperax.io if you spot anything at any time. Also, stay tuned for upcoming grants
  
For details, see [here](https://sperax.io/developer). 
