It is possible to create a contract with code size returned by extcodesize equal to 0. This can lead to bypass of 0-address check in a contract, which may lead to lost of fund or locking of funds.

- [Solidity By Example: Bypass Contract Size Check](https://solidity-by-example.org/hacks/contract-size/)
