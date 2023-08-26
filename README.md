# Decentralized Stablecoin Project

Welcome to the Decentralized Stablecoin project repository! This project aims to create a decentralized stablecoin system that is collateralized by cryptocurrencies such as BTC and ETH. The system maintains a 1:1 peg to USD and utilizes an algorithmic approach for stability.

## About

1. Relative Stability: Anchored or Pegged -> $1.00
   1. Chainlink Price feed.
   2. Set a function to exchange ETH & BTC -> $$$
2. Stability Mechanism (Minting): Algorithmic (Decentralized)
   1. People can only mint the stablecoin with enough collateral (coded)
3. Collateral: Exogenous (Crypto)
   1. wBTC
   2. wETH

## Contracts

### DecentralizedStableCoin.sol

This contract implements the ERC-20 token for the Decentralized Stablecoin (DSC). It includes functions for minting and burning DSC tokens. The contract allows the owner to mint new DSC tokens and users to burn their tokens. The DSC tokens are pegged to USD.

### DSCEngine.sol

DSCEngine is the core contract of the Decentralized Stablecoin system. It handles various operations including depositing collateral, minting and burning DSC tokens, redeeming collateral, and performing liquidations. The system is designed to maintain overcollateralization to ensure stability. The contract utilizes Chainlink price feeds to determine collateral values.

## How to Use

1. Clone the repository to your local machine.
2. Ensure you have a compatible Solidity compiler installed (version 0.8.18).
3. Install required dependencies using npm or yarn:

bash
npm install
 or
yarn install

## Contributing

Contributions to this project are welcome! If you encounter any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. You can find the full license text in the LICENSE file.
