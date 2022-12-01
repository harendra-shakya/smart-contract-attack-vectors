A contract interface defines functions with a different type signature than the implementation, causing two different method id's to be created. As a result, when the interfact is called, the fallback method will be executed.

- [Trail of Bits: Incorrect Interfaces](https://github.com/crytic/not-so-smart-contracts/tree/master/incorrect_interface)
