# Create-a-Token
This is a Solidity smart contract for a token called "META" with the abbreviation "MTA". The contract allows for minting (creating) and burning (destroying) tokens. Here are the main components of the contract:

1. Public variables:
   - `token_name`: A string variable to store the name of the token.
   - `token_abbr`: A string variable to store the abbreviation of the token.
   - `total_supply`: An unsigned integer variable to store the total supply of tokens.

2. Mapping variable:
   - `balances`: A mapping that associates addresses with their token balances. The keys are addresses, and the values are unsigned integers representing the balance of each address.

3. Mint function:
   - `mint`: A function that takes an address `_address` and a value `_value` as parameters. It increases the total supply by `_value` and adds `_value` tokens to the balance of the `_address`.

4. Burn function:
   - `burn`: A function that takes an address `_address` and a value `_value` as parameters. It checks if the balance of the `_address` is greater than or equal to `_value`. If it is, it deducts `_value` from the total supply and the balance of the `_address`.

Note that the contract follows the SPDX-License-Identifier MIT, indicating that it is licensed under the MIT License.
