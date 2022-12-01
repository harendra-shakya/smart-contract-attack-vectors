Variable shadowing occurs when a variable declared within a certain scope (decision block, method, or inner class) has the same name as a variable declared in an outer scope. If multiple variables with the same name are declared in different scopes, there may be unintended effects. This is easy to miss in the case where a contract inherits from a contract implemented in a separate file.

- [Trail of Bits: Variable Shadowing](https://github.com/crytic/not-so-smart-contracts/tree/master/variable%20shadowing)
- [SWC Registry: Incorrect Inheritance Order](https://smartcontractsecurity.github.io/SWC-registry/docs/SWC-125)
- [SWC Registry: Shadowing State Variables](https://smartcontractsecurity.github.io/SWC-registry/docs/SWC-119)
