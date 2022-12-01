# Signature Replay

If a smart contract system performs any sort of signature verification, it may be vulnerable to signature replay attacks. (Keep in mind that any signature sent to a contract via calldata will be publicly available.) Keeping track of processed signatures in storage is a simple way to prevent such attacks. Furthermore, in some cases, signatures may be malleable, i.e. an attacker may be able to modify them (so that they may be replayed) without destroying their validity.

- [SWC Registry: Missing Protection Against Signature Replay Attacks](https://swcregistry.io/docs/SWC-121)
- [SWC Registry: Signature Malleability](https://swcregistry.io/docs/SWC-117)
