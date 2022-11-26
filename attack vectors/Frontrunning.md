# Transaction Ordering / Frontrunning

Miners can see transactions for a short time before they get included in a block, and exploit this information. They can also alter the order of transactions within a block. Users also have some influence over this process by setting gas prices. This can often pose a security risk, especially in systems where users are bidding or otherwise competing for something.

- [Sigmaprime: Block Timestamp Manipulation](https://blog.sigmaprime.io/solidity-security.html#block-timestamp)
