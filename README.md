#AkshatBegContract

## Overview

Built on the Ethereum network, AkshatBegContract is a straightforward token smart contract that resembles an ERC20. The token known as "Akshat Gupta" (abbreviated "AG") with an initial 333 token supply is defined in this contract. The contract permits token minting and burning, allowing for dynamic management of both the overall supply and individual balances.

## Features

- Token Information: The name and abbreviation of the token are among the fundamental details provided by the contract.
- Minting: Increases the overall supply by enabling the creation of new tokens.
- Burning: Permits tokens to be destroyed, reducing the overall supply.

## Contract Information

### State Variables

- tokenName: The token's name. (Open to the public)
tokenAbbr: The token's abbreviation. (Open to the public)
- totalSupply: The whole token supply. (Open to the public)
- balances: A mapping for monitoring the balance of tokens

- ### Functions

#### mint

solidity function mint(address addr,uint amount) external


- Description: Adds to the overall supply by minting new tokens and allocating them to the designated address.
- Parameters:
  - addr: The address that the tokens that are minted will be sent to.
  - amount: The quantity of tokens to be produced.
* Visibility*: external

#### burn

solidity function burn (address addr,uint amount) external


- Description: Reduces the overall supply of tokens by burning them from the designated address.
- Parameters:
  - addr: The address where the burned tokens will come from.
  - amount: The quantity of tokens to be burned.
* Visibility*: external
- Condition: The function determines whether the overall supply exceeds the amount that needs to be burned and whether the address has enough balance to burn.
