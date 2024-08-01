# 100xDevs Web3.0 Roadmap

## 0 - 1

### Foundation (~2 Weeks):

1. Why blockchains? What do they provide?
2. What is decentralization?
3. RPC’s, Common RPC methods.
4. Wei vs Ether, lamports vs SOL.
5. Cryptography, hashing, Encryption - Keccak-256, Ed25119.
6. Gas & Transactions.
7. Public and private keys, mnemonic phrases, creating your own private keys.
8. What are Tokens, Non Fungible Tokens.
9. Basic cryptography.
10. Signing messages using private keys.
11. Devnet vs Mainnet environments.
12. Airdropping.
13. Understanding block explorers (etherscan, solscan).

**End Goal:**

1. Create a CLI wallet.
2. Generate private and public keys using CLI’s.
3. Airdrop some native token.
4. Do some transactions using CLI (Send Tokens).
5. Explore transactions on explorers.

============================================

## Wallets (~3-4 Weeks):

1. Why do you need a wallet? What are wallet extensions?
2. How do they secure your private key?
3. Connecting to RPCs from wallets.
4. Native tokens vs ERC20 (or token program)
5. Showing token balances, NFT balances.
6. How do wallets interact with dApps (overview).
7. Signing messages vs Signing transactions.
8. Common Derivation Path.
9. Creating a website similar to https://www.mynearwallet.com/
10. Create a wallet impersonator that lets you impersonate someone.

**End Goal:**

1. Use an existing wallet, get comfortable with its UX.
2. Create a React app that lets you create wallets and impersonate them.

============================================

## dApps and Transactions (~5-6 Weeks):

1. Understanding commonly done transactions on chain:
   a. Sents.
   b. Swaps.
   c. Smart contract interactions.
2. Parsing transactions to show data in a wallet.
3. Logs, events, and indexed parameters in Ethereum.
4. Create a wallet aggregator/portfolio tracker/airdrop notifier.
   - Examples: https://matrica.io/ OR https://www.assetdash.com/

**End Goal:**

1. Understanding a lot of common transaction formats, parsing them.
2. Creating a portfolio/airdrop tracker.

============================================

## DEXs and Swap Functionality (~7-8 Weeks):

1. Understanding what are DEXs.
2. Liquidity pools.
3. Automated market makers.
4. Creating your own token & Creating a pool for it.
5. Adding swap functionality to your wallet, letting users choose from popular markets.

**End Goal:**

1. Adding swap functionality to your wallet.
2. Adding transaction parsing so all swaps are visible in your wallet.

============================================

## 1 - 100

### Solidity and Smart Contracts (~2 Weeks):

1. What are smart contracts?
2. Solidity syntax, data model on ETH.
3. Remix vs Truffle, Ganache vs Foundry.
4. OpenZeppelin.
5. Bytecode, ABIs and EVM.
6. Writing contracts:
   a. Creating ERC20
   b. Extending ERC721
   c. Writing an Escrow contract
   d. Creating a restricted NFT mint.
7. Exploring common contracts.

**End Goal:**

1. Writing smart contracts.
2. Local development of Solidity.
3. Web2 + Web3 use case of adding custom minting logic.

============================================

### Creating a dApp (~3-4 Weeks)

1. Creating a React project with web3 signing, learn about adapters, connecting to dApps.
2. Creating a web2 backend with verification (Python/Node.js)
3. Create frontend for NFT mint with allowlist.
4. Create frontend for escrow contract.

**End Goal:**

1. Adding frontends to your dApps.
2. ETH adapters.

============================================

### Rust and Solana Smart Contracts (~5-8 Weeks):

1. Rust complete bootcamp.
2. Solana CLI, Solana token program.
3. Data model in Solana, PDAs.
4. PDAs in action, creating a web2 use case in web3. Postgres tables vs PDAs.
5. Create an escrow contract.
6. Deep dive into the Solana token program, associated token account program.
7. Attaching metadata to tokens and NFTs.
8. Exploring common contracts.

**End Goal:**

1. Writing smart contracts in Solana.
2. Local Solana development.

============================================

### Creating a dApp (~9-10 Weeks):

1. Creating a React project with web3 signing.
2. Solana wallet adapter.
3. Create an Initial coin offering contract.
4. Create a frontend that lets users get a token allocation based on their share of the launch investment.

**End Goal:**

1. Adding frontend to your dApps.

============================================

### Indexing Blockchains (~11-12 Weeks):

1. Understanding how to get payments the right way in web2 app.
2. Understanding indexing of the blockchain on ETH.
3. Sweeping wallets, gas optimisations.

**End Goal:**

1. Indexing blockchain
2. Accepting payments the right way.

============================================

### Building an Exchange/Gambling Website:

1. Creating an order-book/create game logic.
2. Allowing deposit and withdrawal logic.
3. Storing the private key, hot and cold wallets, sweeping deposits, Shamir's secret sharing.

**End Goal:**

1. Creating an exchange like Binance.
   OR
2. Creating a gambling website like Stake.com

============================================

## Free Resources

1. [Alchemy University Courses](https://www.alchemy.com/university/courses/ethereum)
2. [Solana Program Library](https://github.com/solana-labs/solana-program-library)
3. [Soldev App Course](https://www.soldev.app/course)
