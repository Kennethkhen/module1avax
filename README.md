
# P2PTransaction Smart Contract

## Overview

This is a Solidity smart contract named `P2PTransaction` that facilitates peer-to-peer transactions by allowing users to deposit and transfer tokens. It maintains balances for each account and emits events for deposit and transfer transactions.

## Usage


1. Deploy the contract to your preferred Ethereum network.
2. Interact with the deployed contract using a tool like [Remix](https://remix.ethereum.org/) or your preferred Ethereum development environment.

## Contract Details

- **Name:** P2PTransaction
- **Version:** 1.0.0
- **Solidity Version:** ^0.8.18
- **License:** MIT

## Functions

### `getBalance()`

- **Description:** Retrieves the balance of the caller's account.
- **Returns:** `uint256`: The balance of the caller's account.

### `deposit(uint256 value)`

- **Description:** Deposits tokens into the caller's account.
- **Parameters:**
  - `value` (uint256): The amount of tokens to deposit.

### `transfer(address to, uint256 value)`

- **Description:** Transfers tokens from the caller's account to the specified recipient.
- **Parameters:**
  - `to` (address): The address of the recipient.
  - `value` (uint256): The amount of tokens to transfer.
- **Requirements:** Requires that the caller has sufficient balance to complete the transfer.

## Events

### `Transfer(address indexed from, address indexed to, uint256 value)`

- **Description:** Emitted when tokens are transferred from one account to another.
- `from` (address): The address from which tokens are transferred.
- `to` (address): The address to which tokens are transferred.
- `value` (uint256): The amount of tokens transferred.

### `Deposit(address indexed account, uint256 amount)`

- **Description:** Emitted when tokens are deposited into an account.
- `account` (address): The address of the account where tokens are deposited.
- `amount` (uint256): The amount of tokens deposited.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.


## Disclaimer

This code is provided as-is, without any warranty or support. Use at your own risk.
