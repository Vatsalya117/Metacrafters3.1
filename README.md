# Solidity Contracts for Registering Organizations and Adding Stakeholders
This project consists of a set of Solidity smart contracts designed to manage non-fungible tokens (NFTs) on the Ethereum blockchain. The functionality includes registering organizations, adding stakeholders, and managing a vesting schedule for tokens.

## Table of Contents
#### Introduction
#### Contract Details
#### Public Variables
#### Functions
#### Getting Started
#### Authors
#### Help

## Introduction
These Solidity smart contracts facilitate the registration of organizations and the management of stakeholders. The contracts also support the minting and burning of tokens, alongside managing the total supply and balances.

## Contract Details
 ### Public Variables
 tokenName: The name of the token (e.g., "ALPHA").
 
 tokenAbbreviation: The abbreviation of the token (e.g., "Beta").
 
 totalSupply: The total supply of the token.
 
 balances: A mapping that associates addresses with their token balances.

## Functions
mint(address _address, uint256 _value): Increases the total supply by _value and adds _value tokens to the balance of the specified _address.

burn(address _address, uint256 _value): Decreases the total supply by _value and deducts _value tokens from the balance of _address, provided the balance is sufficient.

## Solidity Version:

pragma solidity ^0.8.0; specifies the version of the Solidity compiler that should be used to compile the contract. In this case, it requires version 0.8.0 or higher.

#### To start using these contracts, follow these steps:

Install Dependencies: Ensure you have a working Ethereum development environment. You can use tools like Truffle or Hardhat.

Compile the Contract: Use the Solidity compiler to compile your contract.

Deploy the Contract: Deploy your contract to the Ethereum network or a local blockchain.

Interact with the Contract: Use the provided HTML/JavaScript interface to interact with your contract. Ensure you replace placeholder values with actual contract addresses and ABI.

#### Solidity Contract Explanation: OrganizationRegistry

The OrganizationRegistry contract provides a comprehensive system for managing organizations and their stakeholders on the Ethereum blockchain. It includes functionalities for registering organizations, adding stakeholders, and checking various stakeholder details such as their whitelisted status and vesting periods. The contract leverages OpenZeppelin's Ownable module to restrict certain functions to the contract owner, ensuring secure and controlled access to critical operations.

#### Solidity Contract Explanation: Vesting

Checks if the sender is whitelisted and if the vesting period has ended.
Retrieves the organization's token address and gets the token balance of the contract.
Transfers the token balance to the sender.
#### Summary
The Vesting contract provides a mechanism for stakeholders to claim tokens from whitelisted organizations after the vesting period. It leverages functionalities from OrganizationRegistry and OpenZeppelin's contracts for authorization and token transfer operations.

### Help
If you encounter any issues or have questions, please refer to the documentation or contact the contributors.


### Authors
Vatsalya Mishra

https://github.com/Vatsalya117







