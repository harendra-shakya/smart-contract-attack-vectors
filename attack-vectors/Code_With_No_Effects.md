In Solidity, it's possible to write code that does not produce the intended effects. Currently, the solidity compiler will not return a warning for effect-free code. This can lead to the introduction of "dead" code that does not properly performing an intended action.

For example, it's easy to miss the trailing parentheses in `msg.sender.call.value(address(this).balance)("");`, which could lead to a function proceeding without transferring funds to msg.sender. Although, this should be avoided by checking the return value of the call.
