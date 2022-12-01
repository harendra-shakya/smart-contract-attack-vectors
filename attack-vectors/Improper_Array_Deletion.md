In Solidity, we remove an element from an array using the “delete” function. However, the length and sequence of the array may not remain as expected. If we delete the array index x, we will see that the array length remains the same, just that the value at index x has been set to zero.

## Remediation:

Instead of “delete” and “.length=0”, use push and pop functions to interact with array elements.

- [Improper Array Deletion](https://blog.solidityscan.com/improper-array-deletion-82672eed8e8d)
