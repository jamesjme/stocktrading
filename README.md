# Share Market Smart Contract

## Overview

The `share_market` Solidity smart contract is a decentralized application designed to emulate a simple share market on the Ethereum blockchain. This contract enables users to buy and sell shares, with the market operations securely managed by a designated owner.


## Getting Started

To interact with this contract, deploy it on a compatible Ethereum Virtual Machine (EVM) using a Solidity compiler version ^0.8.9. After deployment, the deployer automatically becomes the owner of the contract.

### Deployment

Deploy the contract to an Ethereum blockchain. The contract utilizes Solidity version ^0.8.9, so ensure compatibility with your development environment.

## Functions

### `buyShares(uint256 amount)`

Allows the owner to purchase a specified amount of shares. This function is exclusively accessible to the contract owner, ensuring controlled market operations. Additionally, it enforces that the share amount is positive.

### `sellShares(uint256 amount)`

Permits the owner to sell a specified amount of shares. Similar to the `buyShares` function, only the contract owner can invoke this function. It includes additional checks to ensure the share amount is positive and does not exceed the total available shares.

### `getTotalShares() public view returns (uint256)`

Returns the total number of shares available in the market. This read-only function is accessible to all users and does not modify the contract state.

## Error Handling

The contract implements robust error handling mechanisms to maintain the integrity of the share market. In the event of a transaction failure, informative revert messages provide clear details regarding the cause of the failure.

## Usage
 Utilize the `buyShares` and `sellShares` functions to trade shares. Query the total number of shares available using the `getTotalShares` function.

## Security Considerations

- Only the contract owner can execute buy and sell operations, ensuring a controlled and secure market environment.
- The contract incorporates explicit error messages to provide transparency in case of transaction failures, facilitating debugging and preventing unintended actions.

## Author 

James

jmejames270@gmail.com
