These are possible vulnerabilities in frontends to ethereum contracts, not vulnerabilities in the contracts themselves. (Possibly out of scope.)

## Short Address Attack

Short address attacks are a side-effect of the EVM itself accepting incorrectly padded arguments. Attackers can exploit this by using specially-crafted addresses to make poorly coded clients encode arguments incorrectly before including them in transactions. Is this an EVM issue or a client issue? Should it be fixed in smart contracts instead? While everyone has a different opinion, the fact is that a great deal of ether could be directly impacted by this issue. While this vulnerability has yet to be exploited in the wild, it is a good demonstration of problems arising from the interaction between clients and the Ethereum blockchain. Other off-chain issues exist: an important one is the Ethereum ecosystem's deep trust in specific Javascript front ends, browser plugins and public nodes. An infamous off-chain exploit was used in the hack of the Coindash ICO that modified the company's Ethereum address on their webpage to trick participants into sending ethers to the attacker's address.

Frontends should validate any input used to make transactions on chain.

- [Sigmaprime: Short Address / Parameter Attack](https://blog.sigmaprime.io/solidity-security.html#short-address)
- [DASP: Short Address Attack](https://www.dasp.co/#item-9)
