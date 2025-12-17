# EchoHarbor

Built for Base

EchoHarbor is a compact Base-aligned repository designed to confirm wallet connectivity, RPC integrity, and explorer visibility across Base networks using official Coinbase tooling.

The project acts as a lightweight validation layer for Base infrastructure and account abstraction–compatible user flows, without introducing application-specific contract logic.

## Networks

Base Mainnet  
chainId (decimal): 8453  
Explorer: https://basescan.org  
RPC: https://mainnet.base.org  

Base Sepolia  
chainId (decimal): 84532  
Explorer: https://sepolia.basescan.org  
RPC: https://sepolia.base.org  

## Application Summary

Primary file: app/echoHarbor.ts

EchoHarbor performs the following steps:
- Initializes an OnchainKit provider for a selected Base network
- Renders wallet connection UX
- Uses a Viem public client for Base JSON-RPC reads
- Fetches RPC chainId, latest block number, and native ETH balance
- Surfaces Basescan explorers for direct inspection

## Project Layout

- app/
  - echoHarbor.ts  
    React entry point combining OnchainKit wallet UX with Base RPC reads.

Additional files typically included:
- package.json
- tsconfig.json
- index.html / main.tsx
- .env (optional)

## Tooling

OnchainKit  
https://github.com/coinbase/onchainkit  

Viem  
EVM client used for Base network reads

## Installation

Requirements:
- Node.js 18+
- Browser environment with wallet support

Install dependencies using your preferred package manager and run the project using a standard React/Vite or Next.js development setup.

## Usage

1. Start the application in a browser
2. Select Base Sepolia for testing or Base Mainnet for production reads
3. Connect a wallet via the OnchainKit interface
4. Provide an address to query balance data
5. Execute the onchain check and review results

## License

MIT License

## Author

GitHub: https://github.com/grottolegends
Public contact (email): grotto.legends.0u@icloud.com
Public contact (X): https://x.com/greechroma1

## Testnet Deployment (Base Sepolia)
A smart contract has been deployed to the Base Sepolia test network for validation and testing purposes.

Network: Base Sepolia  
chainId (decimal): 84532  
Explorer: https://sepolia.basescan.org  

Deployed contract #1 address:  
0x20a7c838402449f37910ca17c93d839255accfec

Deployed contract #2 address:  
0x11135449aca177008dea9d87734aaf33428a5ed7

Basescan deployment and verification links:

Contract #1 address:  
https://sepolia.basescan.org/address/0x20a7c838402449f37910ca17c93d839255accfec 

Contract #2 address:  
https://sepolia.basescan.org/address/0x11135449aca177008dea9d87734aaf33428a5ed7 

Contract #1 verification (source code):  
https://sepolia.basescan.org/0x20a7c838402449f37910ca17c93d839255accfec /0#code  

Contract #2 verification (source code):  
https://sepolia.basescan.org/0x11135449aca177008dea9d87734aaf33428a5ed7/0#code  

This deployment is used to validate Base-compatible tooling, account abstraction flows, and onchain read operations in a test environment prior to mainnet usage.

