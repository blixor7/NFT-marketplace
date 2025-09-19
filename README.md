# NFT Marketplace

A decentralized NFT marketplace built on Ethereum, enabling minting, trading, and collecting of digital assets.

## Features

- Mint NFTs: Create and list digital assets on the blockchain
- Buy & Sell: Trade NFTs with secure blockchain transactions
- Wallet Integration: Support for multiple wallets including MetaMask and Fortmatic
- Multi-Network: Deployed on Mumbai testnet with network switching
- IPFS Storage: Decentralized storage for NFT metadata and assets
- Transaction History: Complete history of all NFT transactions
- Responsive Design: Optimized for desktop and mobile devices

## Tech Stack

- Frontend: Next.js, Tailwind CSS
- Smart Contracts: Solidity, Hardhat
- Blockchain: Ethereum (Mumbai Testnet)
- Storage: IPFS (via Infura)
- Wallets: MetaMask, Fortmatic
- Development: ESLint, Prettier, Husky

## Prerequisites

- Node.js (version specified in .nvmrc)
- npm
- MetaMask browser extension

## Installation

1. Clone the repository
   ```bash
   git clone https://github.com/blixor7/nft-marketplace.git
   cd nft-marketplace
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Set up environment variables
   ```bash
   cp .env.local.example .env.local
   # Add your Infura project ID and secret to .env.local
   ```

4. Start local development network
   ```bash
   npx hardhat node
   ```

5. Deploy contracts (in a new terminal)
   ```bash
   npx hardhat run scripts/deploy.js --network localhost
   ```

6. Run the development server
   ```bash
   npm run dev
   ```

7. Open your browser and navigate to http://localhost:3000

## Testnet Setup

To use the Mumbai testnet:

1. Add Mumbai Testnet to MetaMask
   - Network Name: Mumbai
   - RPC URL: https://matic-mumbai.chainstacklabs.com
   - Chain ID: 80001
   - Currency Symbol: MATIC
   - Block Explorer: https://mumbai.polygonscan.com/

2. Get test MATIC from the Polygon Faucet

## Usage

1. Connect your wallet using the connect button
2. Switch to Mumbai testnet when prompted
3. Mint NFTs by uploading your artwork and adding details
4. List NFTs for sale by setting your desired price
5. Browse the marketplace to discover and collect NFTs
6. Buy NFTs with a simple click and confirm the transaction

## Project Structure

```
nft-marketplace/
├── components/          # React components
├── contracts/           # Smart contracts
├── hooks/               # Custom React hooks
├── pages/               # Next.js pages
├── public/              # Static assets
├── scripts/             # Deployment scripts
├── styles/              # CSS styles
├── utils/               # Utility functions
└── test/                # Smart contract tests
```

## Contributing

1. Fork the project
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## License

This project is licensed under the MIT License.

## Troubleshooting

Common issues:
- Ensure you're on the correct network (Mumbai testnet)
- Make sure you have test MATIC for transactions
- Check that your MetaMask is connected to the site

## Support

If you have any questions or issues, please open an issue on GitHub.


