# Miners Attack

## Transaction Ordering / Frontrunning

Since miners always get rewarded via gas fees for running code on behalf of externally owned addresses (EOA), users can specify higher fees to have their transactions mined more quickly. Since the Ethereum blockchain is public, everyone can see the contents of others' pending transactions. This means if a given user is revealing the solution to a puzzle or other valuable secret, a malicious user can steal the solution and copy their transaction with higher fees to preempt the original solution. If developers of smart contracts are not careful, this situation can lead to practical and devastating front-running attacks.

- [Dasp: Front running](https://www.dasp.co/#item-7)
- [Sigmaprime: Race Conditions / Front-Running](https://blog.sigmaprime.io/solidity-security.html#race-conditions)
- [SWC Registry: Transaction Order Dependence](https://smartcontractsecurity.github.io/SWC-registry/docs/SWC-114)

## Timestamp Manipulation

Many contracts use block timestamps for various purposes. Keep in mind that miners can slightly adjust them to their advantage.

- [Sigmaprime: Block Timestamp Manipulation](https://blog.sigmaprime.io/solidity-security.html#block-timestamp)
- [SWC Registry: Timestamp Dependence](https://smartcontractsecurity.github.io/SWC-registry/docs/SWC-116)
