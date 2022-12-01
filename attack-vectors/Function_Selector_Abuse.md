To call a function on another contract, the standard ABI way to do so is to pass as calldata a function "selector", followed by the encoded arguments. You can read more [here](https://docs.soliditylang.org/en/v0.8.7/abi-spec.html), but a short example follows.

In solidity, a call may look like `otherContract.foo("hello")`, but in reality, the call becomes `address(otherContract).call(abi.encodeWithSignature("foo(string)", "hello"))` which in practice becomes

`0xf31a69690000000000000000000000000000000000000000000000000000000000000020000000000000000000000000000000000000000000000000000000000000000568656c6c6f000000000000000000000000000000000000000000000000000000`

The first 4 bytes `0xf31a6969`, are called the function selector, and consist of the first 4 bytes of the Keccak256 hash of the string "foo(string)". All ABI-compliant contracts on Ethereum begin by looking at these bytes of the calldata and jump to the corresponding function body.

If a contract performs a call to an external contract, and the user can influence *any* part of the method signature (such as the function name, or its type), they can call *any* function on the external contract, simply by manipulating the string until a selector matching the desired one is found.

This was behind the Poly Network hack in August 2021, where an attacker crafted messages on one chain which got processed on another chain. The contracts assumed well-behaved transactions, and the attacker managed to trick the contracts into calling privileged functions on yet other contracts.
