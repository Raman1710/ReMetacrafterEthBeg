# ReMetacrafterEthBeg

# Assignment Contract

This Solidity contract represents an assignment contract that allows the creation, destruction, and tracking of tokens.

## Contract Details

The contract has the following state variables:

- `tokenName`: A public string variable representing the name of the token.
- `tokenAbbrv`: A public string variable representing the abbreviation of the token.
- `totalSupply`: A public unsigned integer variable representing the total supply of tokens.
- `balances`: A public mapping that maps addresses to unsigned integer values, representing the token balances of different addresses.

## Functionality

The contract provides the following functionalities:

- `constructor`: Initializes the contract with the token name, abbreviation, and initial supply. It sets the initial supply as the balance for the contract deployer.

- `mint`: Allows the contract owner to mint (create) new tokens. It increases the total supply and adds the specified amount to the balance of the given address.

- `burn`: Allows the contract owner to burn (destroy) tokens. It reduces the total supply and subtracts the specified amount from the balance of the given address. It includes a check to ensure that the address has sufficient balance before burning.

## Usage

To use this contract, follow these steps:

1. Deploy the contract on the Ethereum blockchain.
2. Specify the token name, abbreviation, and initial supply during deployment.
3. The contract deployer will initially have the total supply of tokens.
4. The contract owner can call the `mint` function to create new tokens and assign them to specific addresses.
5. The contract owner can call the `burn` function to destroy tokens and reduce the total supply.

## License

This code is distributed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Version Pragma

This code is written in Solidity version 0.8.9. Make sure to use a compatible Solidity compiler when deploying and interacting with the contract.

