# DOS (Denial of Service)

This is a broad category of attacks where an attacker may render a contract inoperable, temporarily or permanently.

- [DASP: Denial of Service](https://www.dasp.co/#item-5)
- [Sigmaprime: Denial of Service](https://blog.sigmaprime.io/solidity-security.html#dos)
- [Trail of Bits: Denial of Service](https://github.com/crytic/not-so-smart-contracts/tree/master/denial_of_service)

## Unexpected Revert

An attacker may be able to exploit the fact that `transfer`(alternatively `require(addr.send(amount))`) reverts on failure to prevent a function from ever completing execution.

- [Consensys Best Practices: DOS with Unexpected Revert](https://consensys.github.io/smart-contract-best-practices/attacks/denial-of-service/#dos-with-unexpected-revert)
- [SWC Registry: DOS with Failed Call](https://swcregistry.io/docs/SWC-113)

## Block gas limit

In cases where the users of a system can manipulate how much computation (gas) is necessary for the execution of some function, it may be possible to DOS the system by causing the required gas to exceed the block gas limit. This is often the case in systems that loop over an array or mapping that can be enlarged by users at little cost.

- [Consensys Best Practices: DOS with Block Gas Limit](https://consensys.github.io/smart-contract-best-practices/attacks/denial-of-service/#dos-with-block-gas-limit)
- [SWC Registry: DOS with Block Gas Limit](https://swcregistry.io/docs/SWC-128)

## External Calls without Gas Stipends

In some cases, developers may want to make a transfer and continue execution regardless of the result. One way to achieve this is with `call.value(v)()`, however this may allow the recipient to consume all the gas of the calling function, preventing execution from continuing. See example 1 here:

- [Sigmaprime: Denial of Service](https://blog.sigmaprime.io/solidity-security.html#dos)
