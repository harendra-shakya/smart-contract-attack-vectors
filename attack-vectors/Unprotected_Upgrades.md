There is a lot that can go wrong with smart contract upgrades, and it would not make sense to list them here. 99% of the time, you should use OpenZeppelin’s upgraded plug-in tools for hardhat or truffle. But if you want a preview, this can help:

1. Storage slots can clash.
2. Information stored via constructors or immutable variables won’t be available in the next contract.
3. Initializers need to be protected.
4. Selfdestruct can prevent upgrades.

- [All you need to know about UPGRADABLE Smart Contracts](https://trustchain.medium.com/all-you-need-to-know-about-upgradable-proxies-865704a28bc7)
