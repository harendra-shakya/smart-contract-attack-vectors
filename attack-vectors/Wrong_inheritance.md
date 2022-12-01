Solidity supports multiple inheritance, meaning that one contract can inherit several contracts. Multiple inheritance introduces ambiguity called [Diamond Problem](https://en.wikipedia.org/wiki/Multiple_inheritance#The_diamond_problem): if two or more base contracts define the same function, which one should be called in the child contract? Solidity deals with this ambiguity by using reverse [C3 Linearization](https://en.wikipedia.org/wiki/C3_linearization), which sets a priority between base contracts.

That way, base contracts have different priorities, so the order of inheritance matters. Neglecting inheritance order can lead to unexpected behavior.

- [SWC Registry: Incorrect Inheritance Order](https://swcregistry.io/docs/SWC-125)
