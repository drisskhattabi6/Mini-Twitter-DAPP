# Mini Twitter DApp

## Project Overview

The **Mini Twitter DApp** is a decentralized application that enables users to publish, like, dislike, and edit posts on a blockchain-based social media platform. Built on Ethereum using Web3.js, the DApp is designed to demonstrate how decentralized platforms operate by providing basic social media functionalities on the blockchain. Users connect their Ethereum wallets to authenticate and interact with posts, ensuring transparent and immutable interactions. The DApp prioritizes decentralization, user ownership, and secure, tamper-proof content storage.

![DApp](img.png)

## Key Features

- **Wallet Connection**: Users can connect their Ethereum wallet (e.g., MetaMask) to authenticate and interact with the DApp.
- **Publish Posts**: Users can create posts, which are stored immutably on the blockchain.
- **Post Interactions**: Users can like and dislike posts, with the reactions being securely tracked on the blockchain.
- **Edit Posts**: Users can edit posts they have authored, ensuring only the original creator can make changes.
- **Account Switching**: Users can switch between Ethereum accounts, allowing interactions from different wallet addresses.

## Project Structure
``` bash
Mini-Twitter-DAPP
├── interface
│   ├── index.html      # Frontend interface for the application
│   └── style.css       # CSS File
├── MiniTwitter.sol     # Solidity smart contract for managing posts
└── report.pdf          # Project report with detailed explanations
```

## Prerequisites
- **Node.js and yarn** (for JavaScript dependencies)
- **Hardhat** (for deploying and testing the smart contract)
- **MetaMask** (for interacting with the contract through a local wallet)
- **Web3.js**: The DApp uses Web3.js for blockchain interactions.
- **REMIX IDE**
- **XAMPP**


## Installation Steps

1. **Clone the Repository**  
   Clone the project from your source repository:
   ```bash
   git clone https://github.com/drisskhattabi6/Mini-Twitter-DAPP.git
   cd Mini-Twitter-DAPP
   ```

3. **Set Up Hardhat for Local Development**  
   Initialize Hardhat if not already set up: This will give you 20 accounts for Testing
   ```bash
   mkdir hhproject && cd hhproject
   mkdir chain && cd chain
   yarn add hardhat
   yarn hardhat
   yarn hardhat node
   ```

4. **Set Up MetaMask to Connect to the Hardhat Local Network**  
   - Open **MetaMask** in your browser.
   - Go to **Add Network** and enter the following details:
     - **Network Name:** Hardhat Local
     - **New RPC URL:** `http://127.0.0.1:8545`
     - **Chain ID:** 31337
   - Import a test account from the Hardhat local network by copying a private key from the terminal (from step 3) and pasting it into MetaMask.

5. **Compile and Deploy the Smart Contract (solidity file) in REMIX IDE on MetaMask**  


7. **Run the Interface in XAMPP**  
   Go to the XAMPP installation folder, copy the interface folder in the 'htdocs' folder in XAMPP, run XAMPP and open 'http://localhost/interface/'

8. **Testing and Interactions**  
   You can now interact with the smart contract from the web interface, post messages, and interact through MetaMask.


## How It Works

1. **Smart Contract**: The core functionality, including post publishing, editing, and reactions, is implemented in a Solidity smart contract. The smart contract ensures that posts and user interactions are stored securely and remain immutable.
2. **Web3.js Integration**: The Web3.js library allows the DApp to interact with the Ethereum blockchain, enabling functions like wallet connection, transaction processing, and data retrieval.
3. **MetaMask Wallet**: Users authenticate by connecting their MetaMask wallet, which serves as their user ID and allows them to interact with the DApp securely.

## Usage Instructions

1. **Connect Wallet**: Click the "Connect Wallet" button to authenticate with MetaMask.
2. **Publish a Post**: Enter your message and click "Publish" to add your post to the blockchain.
3. **React to Posts**: Use the "Like" or "Dislike" buttons to react to posts.
4. **Edit Your Post**: If you authored a post, you can edit it directly from the UI.
5. **Switch Account**: Switch between accounts using MetaMask and select a different address for interactions.

## Challenges Addressed

- **User Feedback**: Clear status updates and error handling provide feedback on connection status, transaction processing, and any interaction errors.
- **Account Switching**: The DApp prompts users to select accounts directly from MetaMask to streamline user experience.
- **Transaction Delays**: Real-time user feedback is given during transaction processing, enhancing the app's responsiveness.

## License

This project is open-source and available under the MIT License.
