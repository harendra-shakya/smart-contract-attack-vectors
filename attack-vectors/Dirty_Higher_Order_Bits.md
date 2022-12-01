If `keccak256(msg.data)` or some similar hash functionality is used (for example to log past calls), be aware that functions of types that don't occupy 32 bytes may be called with identical arguments but different hashes.

- [Solidity Documentation: Minor Details](https://solidity.readthedocs.io/en/latest/security-considerations.html#minor-details)
