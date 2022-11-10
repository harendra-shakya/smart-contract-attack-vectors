One usually accesses a contract's functionality through its public or external functions. While insecure visibility settings give attackers straightforward ways to access a contract's private values or logic, access control bypasses are sometimes more subtle. These vulnerabilities can occur when contracts use the deprecated tx.origin to validate callers, handle large authorization logic with lengthy require and make reckless use of delegatecall in proxy libraries or proxy contracts.

## Example

In the following example, the contract's initialization function sets the caller of the function as its owner. However, the logic is detached from the contract's constructor, and it does not keep track of the fact that it has already been called.

```
function initContract() public {
	owner = msg.sender;
}
```
