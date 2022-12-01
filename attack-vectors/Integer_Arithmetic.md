Neither the EVM nor Solidity (before v0.8) provide builtin error reporting for arithmetic overflow/underflow. Consequently, applications need to check for these cases themselves. Furthermore, one cannot make the (seemingly reasonable) assumption that `x != -x`, because of [this case](https://gist.github.com/endorphin/b9d78601930922aea12ed3ce6a286576).

Note that since Solidity version 0.8, arithmetic operations revert on overflow and underflow. The developer can choose to bypass these checks by using the `unchecked` keyword, for example with `unchecked { x = a + b; }`

- [SWC Registry: Integer Overflow and Underflow](https://smartcontractsecurity.github.io/swc-registry/docs/swc-101)
- [Trail of Bits: Integer Overflow](https://github.com/crytic/not-so-smart-contracts/tree/master/integer_overflow)
