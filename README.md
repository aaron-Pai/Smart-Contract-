# Panther AI Token (PAI)

## Overview

The Panther AI token (symbol: PAI) is an ERC20 compliant smart contract built on the Ethereum blockchain. The total supply of Panther AI is set to 500,000,000 tokens, and the contract incorporates a feature to charge a small fee on transfers, which goes to the owner of the contract.

## Features

- **Total Supply**: 500,000,000 PAI tokens
- **Decimals**: 18
- **Owner Fee**: 2% on each transfer
- **Burn Functionality**: Allows users to burn their tokens, reducing the total supply
- **Ownership Transfer**: The ability to transfer ownership of the contract

## Contract Functions

### IERC20 Functions

The Panther AI token implements the following functions as part of the ERC20 standard:

- `totalSupply()`: Returns the total supply of tokens.
- `balanceOf(address account)`: Returns the balance of a specified address.
- `transfer(address recipient, uint256 amount)`: Transfers tokens to a specified address.
- `allowance(address owner, address spender)`: Returns the remaining number of tokens that a spender is allowed to spend on behalf of an owner.
- `approve(address spender, uint256 amount)`: Approves a spender to spend a specified amount of tokens on behalf of the message sender.
- `transferFrom(address sender, address recipient, uint256 amount)`: Transfers tokens from one address to another using the allowance mechanism.

### Additional Functions

- `burn(uint256 _value)`: Allows the caller to burn a specified amount of their tokens, reducing the total supply.
- `changeOwner(address newOwner)`: Transfers ownership of the contract to a new address.
- `changeOwnerFee(uint256 newFeePercent)`: Changes the percentage fee taken from transfers.

## Events

The contract emits the following events:

- `Transfer(address indexed from, address indexed to, uint256 value)`: Triggered when tokens are transferred.
- `Approval(address indexed owner, address indexed spender, uint256 value)`: Triggered when an approval is made.
- `OwnershipTransferred(address indexed previousOwner, address indexed newOwner)`: Triggered when the ownership is transferred.
- `FeePercentChanged(string feeType, uint256 oldPercent, uint256 newPercent)`: Triggered when the owner fee percentage is changed.
- `Burn(address indexed burner, uint256 value)`: Triggered when tokens are burned.

## Getting Started

To deploy the Panther AI contract, you will need:

1. An Ethereum wallet (e.g., MetaMask) with sufficient ETH for gas fees.
2. A development environment like [Remix](https://remix.ethereum.org/) or [Truffle](https://www.trufflesuite.com/truffle).
3. The Solidity compiler version ^0.8.9.

### Deployment Steps

1. Copy the contract code into your development environment.
2. Compile the contract.
3. Deploy the contract to the Ethereum network.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For inquiries, please reach out to [your.email@example.com].
