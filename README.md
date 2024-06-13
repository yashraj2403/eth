# My Token contract
Overview
MyToken is a simple ERC-20-like token contract implemented in Solidity. The token is named "META" with the abbreviation "MTA". The contract allows for the minting and burning of tokens, updating the total supply and the balances of token holders accordingly.

Features
Token Name: META
Token Abbreviation: MTA
Total Supply: Tracks the total supply of tokens.
Balances: Maintains a mapping of addresses to their token balances.

## Getting started
mint

function mint(address _address, uint _value) public

The mint function allows the creation of new tokens. When called, it increases the total supply of tokens and credits the specified address with the minted tokens.

Parameters:

_address: The address to which the newly minted tokens will be credited.
_value: The amount of tokens to be minted.
Usage:


mint(0xYourAddress, 100);
burn


function burn(address _address, uint _value) public
The burn function allows for the destruction of existing tokens. When called, it decreases the total supply of tokens and debits the specified address by the burned tokens, provided the address has sufficient balance.

Parameters:

_address: The address from which the tokens will be burned.
_value: The amount of tokens to be burned.
