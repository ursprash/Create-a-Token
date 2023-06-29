# Create-a-Token

This is a Solidity smart contract for a basic token called MyToken (META). The contract allows users to mint and burn tokens.

## Requirements

1. The contract has public variables to store the details about the token: `token_name` (Token Name), `token_abbr` (Token Abbreviation), and `total_supply` (Total Token Supply).
2. The contract has a mapping of addresses to balances (`balances`), which keeps track of the token balance for each address.
3. The contract has a `mint` function that takes two parameters: an address and a value. This function increases the total token supply by the given value and increases the balance of the specified address by that amount.
4. The contract has a `burn` function that works in the opposite way of the `mint` function. It takes an address and a value, deducts the value from the total supply, and reduces the balance of the specified address by that amount.
5. The `burn` function includes conditionals to ensure that the balance of the sender is greater than or equal to the amount that is supposed to be burned.

## Usage

1. Deploy the contract to the Ethereum network.
2. Use the following functions to interact with the contract:
   - `mint(address _address, uint _value)`: Mints new tokens by increasing the total supply and the balance of the specified address by the given value.
   - `burn(address _address, uint _value)`: Burns tokens by reducing the total supply and the balance of the specified address by the given value. The function includes conditionals to ensure that the balance of the sender is sufficient for the burn operation.

## License

The contract is licensed under the MIT License.
