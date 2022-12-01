Local variables in solidity functions default to `storage` or `memory` depending on their type. Uninitialized local storage variables can point to unexpected storage locations in the contract, leading to intentional or unintentional vulnerabilities.

- [Sigmaprime: Uninitialized Storage Pointers](https://blog.sigmaprime.io/solidity-security.html#storage)
- [SWC Registry: Uninitialized Storage Pointer](https://smartcontractsecurity.github.io/SWC-registry/docs/SWC-109)
