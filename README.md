# ETHassessment_Supleo

## Simple Overview
The `MyToken` Solidity contract is a basic implementation of a cryptocurrency token on the Ethereum blockchain. It allows for the creation (minting) and destruction (burning) of tokens, providing a simple framework for managing token balances and supply.

## Description
This Solidity smart contract defines a basic cryptocurrency token with a name ("META"), an abbreviation ("MTA"), and a starting total supply of zero. The contract uses a mapping to track the token balances of different addresses. It includes two main functions: mint and burn. The mint function allows the creation of new tokens, increasing both the total supply and the recipient's balance. The burn function enables the destruction of tokens, reducing both the total supply and the balance of the specified address, but only if the address holds enough tokens to cover the burn. This contract provides a simple framework for token creation and management on the Ethereum blockchain.

## Getting Started

### IDE

To deploy and interact with this contract, you will need:
- An Ethereum development environment like [Remix IDE](https://remix.ethereum.org/).
- The Solidity compiler version `^0.8.26` or higher.

1. Download or copy the `MyToken.sol` file to your local development environment.
2. Ensure you have an Ethereum wallet (e.g., MetaMask) 
### Executing program

To deploy the contract in Remix:

1. Open [Remix IDE](https://remix.ethereum.org/).
2. Create a new file and paste the Solidity code from `MyToken.sol`.
3. Select the appropriate compiler version (`0.8.26` or higher) from the "Solidity Compiler" tab and compile the contract.
4. Go to the "Deploy & Run Transactions" tab, select the contract, and deploy it.
5. Once deployed, you can interact with the `mint` and `burn` functions through the Remix interface:

### Example Usage
Users can interact with the token using the following commands:
```solidity
// Mint 1000 tokens to a specific address
mint("0x5B38Da6a701c568545dCfcB03FcB875f56beddC4", 1000);

// Burn 500 tokens from a specific address
burn("0x5B38Da6a701c568545dCfcB03FcB875f56beddC4", 500);
```
Or you may use the interface of [Remix IDE](https://remix.ethereum.org/) Deploy & run transactions.

![image](https://github.com/user-attachments/assets/15ad72ea-b64d-4ada-817f-159a6111a05f)

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.

## Acknowledgments

- Special thanks to the MetaChris, Metacrafters community and Ethereum community for their resources and documentation.
- Inspiration from various open-source cryptocurrency projects that helped shape this token implementation.
