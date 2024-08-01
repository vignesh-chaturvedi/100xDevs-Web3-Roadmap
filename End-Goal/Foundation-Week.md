# Ethereum CLI Wallet Guide

## Step 1: Create a CLI Wallet

### Install Geth (Go Ethereum)

First, you need to install Geth, which is a popular Ethereum node implementation. Follow the installation instructions for your operating system from the [official documentation](https://geth.ethereum.org/docs/install-and-build/installing-geth).

```sh
# For Debian-based systems:
sudo apt-get install software-properties-common
sudo add-apt-repository -y ppa:ethereum/ethereum
sudo apt-get update
sudo apt-get install ethereum
```

```sh
# For macOS:
brew tap ethereum/ethereum
brew install ethereum
```

## Step 2: Generate Private and Public Keys

### Using Geth

```sh
# Initialize a new Ethereum account
geth account new

# You will be prompted to enter a passphrase to encrypt your private key.
```

This will generate a new account and display the public address. The private key is stored encrypted in the keystore directory.

### Using eth-keygen

Alternatively, you can use `eth-keygen`, a simple tool to generate Ethereum keys.

```sh
# Install eth-keygen
npm install -g eth-keygen

# Generate a new key pair
eth-keygen

# This will output the private and public keys.
```

## Step 3: Airdrop Some Native Tokens

To airdrop tokens, you need to have access to an Ethereum testnet or mainnet where you have some ETH. For test purposes, use a testnet like Sepolia or Holešky.

1. **Obtain Testnet ETH**: Use a faucet to get some testnet ETH. For Sepolia, you can use [this faucet](https://cloud.google.com/application/web3/faucet/ethereum/sepolia).

2. **Send ETH to New Account**:

```sh
   # Unlock your account
   geth --Sepolia account unlock [your_main_account_address]

   # Send ETH using Geth console
   geth attach
   > eth.sendTransaction({from: 'your_main_account_address', to: 'new_account_address', value: web3.toWei(1, "ether")})
```

## Step 4: Perform Transactions Using CLI (Send Tokens)

### Using Geth

1. **Start Geth Console**:

```sh
geth attach
```

2. **Unlock the Sender Account:**:

```sh
personal.unlockAccount('new_account_address', 'password')
```

3. **Send ETH:**:

```sh
eth.sendTransaction({from: 'new_account_address', to: 'recipient_address', value: web3.toWei(0.1, "ether")})
```

### Using ethers.js

1. **Install ethers.js**:

```sh
npm install ethers
```

2. **Create a Script:**:

```js
// send-tokens.js
const { ethers } = require("ethers");

// Connect to the network
const provider = new ethers.providers.InfuraProvider(
  "rinkeby",
  "your_infura_project_id"
);

// Private key of the sender
const privateKey = "your_private_key";
const wallet = new ethers.Wallet(privateKey, provider);

// Define the transaction
const tx = {
  to: "recipient_address",
  value: ethers.utils.parseEther("0.1"),
};

// Send the transaction
wallet.sendTransaction(tx).then((txObj) => {
  console.log("txHash", txObj.hash);
});
```

3. **Run the Script:**:

```sh
node send-tokens.js
```

### Summary

- **Create CLI Wallet**: Use geth account new or eth-keygen.
- **Generate Keys**: Automatically done when creating the wallet.
- **Airdrop Tokens**: Use a faucet for testnet ETH and eth.sendTransaction in the Geth console.
- **Send Transactions**: Use Geth console commands or a script with ethers.js.

## Summary

- **Create CLI Wallet**: Use `geth account new` or `eth-keygen`.
- **Generate Keys**: Automatically done when creating the wallet.
- **Airdrop Tokens**: Use a faucet for testnet ETH and `eth.sendTransaction` in the Geth console.
- **Send Transactions**: Use Geth console commands or a script with ethers.js.
