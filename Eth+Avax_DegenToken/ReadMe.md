# DegenToken Smart Contract

This Solidity smart contract implements an ERC20 token with additional NFT functionality for a gaming ecosystem on the Avalanche blockchain. It demonstrates the use of OpenZeppelin libraries, custom NFT structures, and various token management functions.

## Description

The DegenToken contract allows for the creation, transfer, and management of both fungible tokens (DGN) and non-fungible tokens (NFTs) within a gaming context. It showcases fundamental concepts of smart contract development, including:

- ERC20 token implementation
- NFT creation and management
- Ownership control
- Token minting and burning
- NFT marketplace functionality

## Functions

### Token Management

#### mint_DGN(address to, uint256 amount)
- Allows the owner to mint new DGN tokens to a specified address.

#### burn_DGN(uint256 amount)
- Allows users to burn their own DGN tokens.

#### transfer(address to, uint256 amount)
- Overrides the ERC20 transfer function to include logging.

### NFT Management

#### mint_NFT(string memory name, uint256 price)
- Allows the owner to create new NFTs in the marketplace.

#### Burn_NFT(uint256 itemId)
- Allows the owner to remove NFTs from the marketplace.

#### Available_NFTs()
- Returns a list of available NFTs in the marketplace.

#### NFT_Price(uint256 itemId)
- Returns the price of a specific NFT.

#### redeem_NFT(uint256 itemId)
- Allows users to purchase NFTs using DGN tokens.

#### Owned_NFTs()
- Returns a list of NFTs owned by the caller.

#### resellNFT(uint256 itemId)
- Allows users to resell their NFTs back to the marketplace for 90% of the original price.

#### transfer_NFT(address to, uint256 itemId)
- Allows users to transfer their NFTs to other users for 90% of the original price.

## Getting Started

### Executing the Program

To run this program, you can use Remix, an online Solidity IDE. Follow these steps:

1. Go to https://remix.ethereum.org/
2. Create a new file and name it `DegenToken.sol`
3. Copy and paste the provided code into the file
4. Compile the contract by clicking on the "Solidity Compiler" tab and then "Compile DegenToken.sol"

### Deployment

This contract was deployed on the Fuji C-Chain testnet using the following steps:

1. Connect MetaMask to the Remix IDE by selecting "Injected Provider - MetaMask" in the "Environment" dropdown of the "Deploy & Run Transactions" tab.
2. Ensure your MetaMask is connected to the Avalanche Fuji Testnet.
3. Obtain test AVAX from the Avalanche Testnet Faucet (https://faucet.avax.network/) and add it to your MetaMask wallet.
4. Deploy the contract using the "Deploy" button in Remix.
5. Use the deployed contract's functions to interact with the token and NFT ecosystem.

### Monitoring Transactions

To monitor the transactions and contract interactions:

1. Use Snowtrace (https://testnet.snowtrace.io/) to view and verify transactions on the Fuji testnet.
2. Enter the contract address or transaction hash in Snowtrace to see detailed information about the interactions.

## Authors

[Your Name or Username]

## License

This project is licensed under the MIT License.