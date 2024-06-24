# Token Smart Contract
## Overview
This smart contract is my submission for the Metacrafters ETH Proof: Beginner EVM Course. The contract implements a basic token system with minting and burning functionalities. It includes public variables to store token details, a mapping to track balances, events for logging actions, and functions to mint and burn tokens, as well as to check user balances.

## Description
The smart contract, Token, consists of the following features:

1 Public Variables:
tokenName: Stores the name of the token, which is set to "Prabhat".
tokensymbol: Stores the abbreviation of the token, which is set to "P@".
totalsupply: Stores the total supply of tokens.
2 Mapping:
Accountbalances: Maps addresses to their respective token balances.

3 FUnctions:
Mint: Logs the minting of tokens. Burn: Logs the burning of tokens.

mint(address to, uint _valuof): Increases the total supply of tokens and the balance of the specified address by the given amount. Emits a Mint event. burn(address from, uint _valueof): Decreases the total supply of tokens and the balance of the specified address by the given amount, provided the address has enough tokens to burn. Emits a Burn event.

## Code Explanation
### Variables
Token Name (tokenName): This variable stores the name of the token, which is set to "Prabhat".

Token Abbreviation (tokensymbol): This variable stores the abbreviation of the token, which is set to "P@".

Total Supply (totalsupply): This variable tracks the total supply of the tokens. Initially, it is set to 0.

### Mapping
Balances (Accountbalances): This mapping associates each address with its corresponding token balance. The key is an address, and the value is the balance of tokens that address holds.

### Functions
Mint Function (mint): This function increases the total supply of tokens by the specified amount and credits the same amount to the balance of the given address. It also emits a Mint event.

Burn Function (burn): This function decreases the total supply of tokens by the specified amount and deducts the same amount from the balance of the given address. The function checks if the address has enough tokens before proceeding with the burn. It also emits a Burn event.
