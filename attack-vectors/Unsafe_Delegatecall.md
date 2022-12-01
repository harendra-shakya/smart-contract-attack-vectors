Solidity allows calling external contracts via the DELEGATECALL opcode, which executes the code of an external contract in the persistent context of the present contract. Certain contracts perform DELEGATECALL calls using user-provided call data, which can effectively give full control to an attacker.

-[Sigmaprime: delegatecall](https://blog.sigmaprime.io/solidity-security.html#delegatecall)

- [SWC Registry: delegatecall to Untrusted Callee](https://swcregistry.io/docs/SWC-112)
