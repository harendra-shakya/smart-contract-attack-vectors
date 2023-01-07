# Smart contract attack vectors

The Goal of this repo is to have possible smart contract vulnerabilities and resources to learn.

Feel free to submit a pull request, with anything from small fixes to docs or tools you'd like to add.

[![Support Project](https://img.shields.io/badge/Support-Project-critical)](https://github.com/harendra-shakya/support/blob/main/README.md)

## List of Security Vulnerabilities

- [Access Control](attack-vectors/Access_Control.md)
  - [Authentication With tx.origin](attack-vectors/Access_Control.md/#authentication-with-txorigin)
  - [Default Visibility](attack-vectors/Access_Control.md/#default-visibility)
  - [Signature Verification](attack-vectors/Access_Control.md/#signature-verification)
  - [Unprotected Ether Withdrawal](attack-vectors/Access_Control.md/#unprotected-ether-withdrawal)
  - [Unprotected SELFDESTRUCT Instruction](attack-vectors/Access_Control.md/#unprotected-selfdestruct-instruction)
  - [Missed Modifier](attack-vectors/Access_Control.md/#missed-modifier)
  - [Incorrect Modifier Names](attack-vectors/Access_Control.md/#incorrect-modifier-names)
  - [Overpowered Roles](attack-vectors/Access_Control.md/#overpowered-roles)
- [Account Existence Check for low level calls](attack-vectors/Account_Existence_Check_for_low_level_calls.md)
- [Arbitrary Jumps with Function Variables](attack-vectors/Arbitrary_Jumps_with_Function_Variables.md)
- [Assert Violation](attack-vectors/Assert_Violation.md)
- [Bypass Contract Size Check](attack-vectors/Bypass_Contract_Size_Check.md)
- [Code With No Effects](attack-vectors/Code_With_No_Effects.md)
- [Complex Modifiers](attack-vectors/Complex_Modifiers.md)
- [DOS](attack-vectors/DOS.md)
  - [Unexpected Revert](attack-vectors/DOS.md/#unexpected-revert)
  - [Block Gas Limit](attack-vectors/DOS.md/#block-gas-limit)
  - [External Calls without Gas Stipends](attack-vectors/DOS.md/#external-calls-without-gas-stipends)
- [Dirty Higher Order Bits](attack-vectors/Dirty_Higher_Order_Bits.md)
- [Entropy Illusion / Insecure Randomness](attack-vectors/Entropy_Illusion.md)
- [Experimental Language Features](attack-vectors/Entropy_Illusion.md)
- [External Contract Referencing](attack-vectors/External_Contrac_Referencing.md)
- [Flash Loan Attacks](attack-vectors/Flash_Loan_Attack.md)
- [Floating Point Arithmetic](attack-vectors/Floating_Point_Arithmetic.md)
- [Frontend (Off Chain) Attacks](<attack-vectors/Frontend_(Off_Chain)_Attacks.md>)
  - [Short Address Attack](<attack-vectors/Frontend_(Off_Chain)_Attacks.md/>)
- [Force Feeding](attack-vectors/Force_Feeding.md)
- [Function Selector Abuse](attack-vectors/Function_Selector_Abuse.md)
- [Griefing](attack-vectors/Griefing.md)
- [Hiding Malicious Code](attack-vectors/Hidden_malicious_code.md)
- [Historic Attacks](attack-vectors/Historic_Attacks.md)
  - [Constructor Names](attack-vectors/Historic_Attacks.md/#constructor-names)
  - [Call Depth Attack](attack-vectors/Historic_Attacks.md/#constructor-names)
  - [Solidity Abi Encoder v2 Bug](attack-vectors/Historic_Attacks.md/#solidity-abi-encoder-v2-bug)
- [Improper Array Deletion](attack-vectors/Improper_Array_Deletion.md)
- [Incorrect Interface](attack-vectors/Incorrect_Interface.md)
- [Insufficient Gas Attacks](attack-vectors/Insufficient_Gas_Attacks.md)
- [Integer Arithmetic](attack-vectors/Integer_Arithmetic.md)
- [Loop through long arrays](attack-vectors/Loop_through_long_arrays.md)
- [Message call with hardcoded gas amount](attack-vectors/Message_call_with_hardcoded_gas_amount.md)
- [Miner Attacks](attack-vectors/Miners_Attack.md)
  - [Transaction Ordering / Frontrunning](attack-vectors/Miners_Attack.md/#transaction-ordering--frontrunning)
  - [Timestamp Manipulation](attack-vectors/Miners_Attack.md/#timestamp-manipulation)
- [Offline Owner](attack-vectors/Offline_Owner.md)
- [Oracle Manipulation](attack-vectors/Oracle_Manipulation.md)
- [Outdated Compiler](attack-vectors/Outdated_Compiler.md)
- [Payable Multicall](attack-vectors/Payable_Multicall.md)
- [Precision Loss in Calculations](attack-vectors/Precision_Loss_in_Calculations.md)
- [Privacy Illusion](attack-vectors/Privacy_Illusion.md)
- [Proxy Storage Collision](attack-vectors/Proxy_Storage_Collision.md)
- [Reentrancy](attack-vectors/Reentrancy.md)
- [Right-To-Left-Override control character (U+202E)](<attack-vectors/Right-To-Left-Override_control_character_(U%2B202E).md>)
- [Sandwich Attacks](attack-vectors/Sandwich_Attack.md)
- [Signature Replay](attack-vectors/Signature_Replay.md)
- [Unchecked External Calls](attack-vectors/Unchecked_External_Calls.md)
- [Uninitialized Storage Pointers](attack-vectors/Uninitialized_Storage_Pointers.md)
- [Unprotected Upgrades](attack-vectors/Unprotected_Upgrades.md)
- [Unsafe Delegatecalls](attack-vectors/Unsafe_Delegatecall.md)
- [Unused Variable](attack-vectors/Unused_Variable.md)
- [Use of Deprecated Solidity Functions](attack-vectors/Use_of_Deprecated_Solidity_Functions.md)
- [Variable Shadowing](attack-vectors/Variable_Shadowing.md)
- [Writes to Arbitrary Storage Locations](attack-vectors/Writes_to_Arbitrary_Storage_Locations.md)
- [Wrong inheritance](attack-vectors/Wrong_inheritance.md)

#

## [CTFs](tools-and-ctfs/CTFs.md)

## [Security Tools](tools-and-ctfs/Web3_Security_Tools.md)

# Other useful resources

- [The Auditors Book](https://theauditorbook.com/)

- [CryptoFin Solidity Auditing Checklist](https://github.com/cryptofinlabs/audit-checklist)

- [SWC Registry](https://swcregistry.io/)

- [Trail of Bits Reference List](https://github.com/crytic/awesome-ethereum-security)
