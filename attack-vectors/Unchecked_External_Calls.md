In Solidity, there are multiple ways to call an external contract and send ether. The function `transfer` reverts if the transfer fails. However, the functions `call` and `send` return false. Programmers may mistakenly expect `call` and `send` to revert, and fail to check for their return value.

- [DASP: Unchecked Low Level Calls](https://www.dasp.co/#item-4)

- [Sigmaprime: Unchecked CALL Return Values](https://blog.sigmaprime.io/solidity-security.html#unchecked-calls)

- [Trail of Bits: Unchecked External Calls](https://github.com/crytic/not-so-smart-contracts/tree/master/unchecked_external_call)
