# CryptoPay - Blockchain Payment Application

A decentralized payment application built with React and Ethereum smart contracts, inspired by Venmo. Send and receive cryptocurrency payments with ease while maintaining full transparency on the blockchain.

## 🚀 Features

- **Secure Wallet Integration**: Connect with MetaMask wallet for secure transactions
- **Real-time Transactions**: Send and receive payments instantly on the blockchain
- **Transaction History**: View all past transactions with timestamps and details
- **Modern UI**: Clean, responsive design with smooth animations
- **Smart Contract Integration**: Deployed on Ethereum blockchain for transparency
- **Activity Feed**: Track all transactions in real-time

## 🛠️ Tech Stack

### Frontend
- **React 18** - Modern React with hooks
- **JavaScript** - ES6+ features
- **CSS Modules** - Scoped styling
- **Framer Motion** - Smooth animations
- **Heroicons** - Beautiful icons
- **Tailwind CSS** - Utility-first CSS framework

### Blockchain
- **Solidity** - Smart contract development
- **Ethers.js** - Ethereum JavaScript library
- **Truffle** - Development framework
- **MetaMask** - Wallet integration

### Development Tools
- **React Scripts** - Build and development tools
- **Web3 Provider** - Blockchain connectivity
- **JavaScript Time Ago** - Relative time formatting

## 📋 Prerequisites

Before running this application, make sure you have:

- **Node.js** (v14 or higher)
- **npm** or **yarn** package manager
- **MetaMask** browser extension
- **Ethereum testnet** (Goerli, Sepolia, or local network)

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone <repository-url>
cd cryptopay
```

### 2. Install Dependencies
```bash
npm install
# or
yarn install
```

### 3. Smart Contract Setup

#### Install Truffle (if not already installed)
```bash
npm install -g truffle
```

#### Deploy Smart Contracts
```bash
cd smart_contract
truffle compile
truffle migrate --network <your-network>
```

#### Update Contract Address
Update the contract address in `src/utils/constants.js` with your deployed contract address.

### 4. Environment Setup
Create a `.env` file in the root directory:
```env
REACT_APP_CONTRACT_ADDRESS=your_deployed_contract_address
```

### 5. Start the Application
```bash
npm start
# or
yarn start
```

The application will open at `http://localhost:3000`

## 🏗️ Project Structure

```
cryptopay/
├── public/                 # Static assets
├── src/
│   ├── components/         # React components
│   │   ├── activity/       # Activity feed components
│   │   └── transaction/    # Transaction form components
│   ├── context/           # React context for state management
│   ├── styles/            # CSS modules
│   └── utils/             # Utility functions and constants
├── smart_contract/        # Solidity smart contracts
│   ├── contracts/         # Smart contract source files
│   ├── migrations/        # Deployment scripts
│   └── build/            # Compiled contracts
└── package.json          # Dependencies and scripts
```

## 🔧 Smart Contract

The application uses a simple but effective smart contract for managing transactions:

### Key Functions
- `addToBlockchain()` - Records new transactions
- `getAllTransactions()` - Retrieves transaction history
- `getTransactionCount()` - Returns total transaction count

### Events
- `Transfer` - Emitted when a new transaction is created

## 💡 Usage

### 1. Connect Wallet
- Click "Connect Wallet" to link your MetaMask account
- Ensure you're connected to the correct network

### 2. Send Payment
- Enter recipient's wallet address
- Specify the amount in ETH
- Add an optional message
- Click "Send" to initiate the transaction

### 3. View Transactions
- All transactions are displayed in the activity feed
- See sender, receiver, amount, and timestamp
- Transactions are permanently recorded on the blockchain

## 🔒 Security Features

- **Wallet Integration**: Secure connection through MetaMask
- **Transaction Validation**: All transactions are validated by the blockchain
- **Immutable Records**: Once recorded, transactions cannot be altered
- **Gas Fee Protection**: Users control gas fees for transactions

## 🌐 Network Support

The application supports:
- **Ethereum Mainnet** (for production)
- **Goerli Testnet** (for testing)
- **Sepolia Testnet** (for testing)
- **Local Development Networks**

## 🧪 Testing

### Run Tests
```bash
npm test
```

### Smart Contract Testing
```bash
cd smart_contract
truffle test
```

## 📦 Building for Production

```bash
npm run build
```

This creates an optimized production build in the `build` folder.

## 🚀 Deployment

### Frontend Deployment
Deploy the `build` folder to your preferred hosting service:
- **Vercel**
- **Netlify**
- **AWS S3**
- **GitHub Pages**

### Smart Contract Deployment
```bash
cd smart_contract
truffle migrate --network mainnet
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

This application is for educational and demonstration purposes. Always verify smart contracts and conduct thorough testing before using in production. Cryptocurrency transactions are irreversible, so use with caution.

## 🆘 Support

If you encounter any issues:

1. Check the [Issues](https://github.com/your-repo/issues) page
2. Ensure MetaMask is properly installed and configured
3. Verify you're connected to the correct network
4. Check that you have sufficient ETH for gas fees

## 🔗 Useful Links

- [Ethereum Documentation](https://ethereum.org/developers/)
- [MetaMask Documentation](https://docs.metamask.io/)
- [Truffle Documentation](https://trufflesuite.com/docs/)
- [React Documentation](https://reactjs.org/docs/)

---

**Happy Coding! 🚀**