## Introduction

Solidity, the primary language for writing smart contracts on blockchain platforms like Celo, has a feature known as events that allow you to log certain actions within the contract. This challenge focuses on implementing a transaction log using Solidity events.

## Problem Statement\*

Create a contract for a simple token transfer with a transaction log. The requirements are as follows:

1. The contract should maintain a ledger of token balances for each address.
2. It should have a function to transfer tokens from one address to another.
3. An event named "Transfer" should be emitted every time a token transfer occurs.
4. The "Transfer" event should log the sender's address, the recipient's address, and the amount of tokens transferred.
5. A function should be present to query the token balance of a specific address.

## Hints

- Use `mapping` in Solidity to create the ledger of token balances.
- The `msg.sender` global variable can be used to denote the sender in a transaction.
- Solidity's `event` keyword can be used to define the "Transfer" event.
- The `emit` keyword is used to trigger an event.
- Remember to update the sender and recipient's balance in the transfer function after emitting the event.

## Evaluation Criteria

- **Correctity**: The contract should compile without errors and meet all requirements.
- **Readability**: The contract should be easy to understand, with comments explaining the code.
- **Testability**: You should also provide examples of how to test each function of the contract.

Please note, while this challenge focuses on event logging, it does not cover important aspects like security, gas optimization, or contract upgradability, which are crucial for real-world contract deployment on the Celo platform.

To deepen your understanding of Celo smart contracts and Solidity, consider reading through the Celo and Solidity tutorials.

## Submission

Please reply with a link to your PR on GitHub, including your token transfer contract and transaction log. Also, include any notes or comments you think are necessary for understanding your design and choices. Lastly, provide a brief explanation about how each function of the contract should be tested.
