# Sustainability Hub - Decentralized Marketplace

Sustainability Hub is a decentralized marketplace designed to promote eco-friendly and sustainable living. Built on Ethereum, the platform allows users to buy and sell eco-conscious products while ensuring transparency, security, and decentralization.

---

## Objectives

The primary objective of this project was to create a Decentralized Marketplace focused on sustainability. By leveraging Ethereum smart contracts, the platform enables secure and transparent transactions for environmentally friendly products, encouraging users to adopt sustainable practices.

---
## Project Design

### Components

1. **Smart Contract**
   - Written in Solidity using Remix IDE.
   - Manages item listing, purchasing, and querying product data on the Ethereum blockchain.

2. **Frontend**
   - Developed using Next.js for a seamless and interactive user experience.
   - Features functionalities to list items, display eco-conscious product details, and process purchases.

3. **Hosting and Deployment**
   - Smart contracts are deployed on the **Sepolia Ethereum testnet**.
---

## Smart Contract Functionalities

1. **listItem**: Allows sellers to list items with details like title, description, price, and an IPFS image hash.
2. **buyItem**: Enables users to purchase listed items with security checks to validate transactions.
3. **getAllItems**: Retrieves all listed items from the blockchain.
4. **getItemById**: Fetches details of a specific item by its ID.

---
## Technologies & Libraries Used

- **Solidity**: For writing the smart contract.
- **Next.js**: React framework for building the frontend.
- **IPFS (via Pinata)**: Decentralized storage solution for images.
- **Ethers.js**: JavaScript library for interacting with the Ethereum blockchain.
- **Axios**: For handling IPFS image uploads and external HTTP requests.

---
##  Prerequisites

Before getting started, ensure you have the following installed:

- **Node.js** and **npm**: To run the frontend application.
- **MetaMask** (or another Ethereum wallet): To interact with the Ethereum network.

---

##  Installation and Setup

### Step 1: Clone the Repository

```bash
git clone 
cd

### Step 2: Install Dependencies

Run the following commands to install the required NPM packages:

```bash
npm install
npm install ethers
npm install axios

### Step 3: Configure Environment Variables
Create a .env.local file in the root directory of the frontend project and add your Pinata API Key and Pinata Secret Key.

```bash
PINATA_API_KEY=your_pinata_api_key
PINATA_SECRET_API_KEY=your_pinata_secret_key

### Step 4: Update Contract Details

1. Deploy the smart contract using Remix IDE or your preferred tool.
2. Replace the placeholder contract address in constants.json with the deployed contract address.
3. Update the content of Transactions.json with the ABI file generated during smart contract compilation.

### Run the following commands to build and deploy the frontend:

```bash
npm run build
