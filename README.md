# T-REX Clone

## Overview

The T-REX (Token for Regulated EXchanges) protocol is a comprehensive suite of Solidity smart contracts,
implementing the [ERC-3643 standard](https://eips.ethereum.org/EIPS/eip-3643) and designed to enable the issuance, management, and transfer of security
tokens in
compliance with regulations. It ensures secure and compliant transactions for all parties involved in the token exchange.

## Key Components

The T-REX protocol consists of several key components:

- **[ONCHAINID](https://github.com/onchain-id/solidity)**: A smart contract deployed by a user to interact with the security token or any other application
  where an on-chain identity may be relevant. It stores keys and claims related to a specific identity.

- **Trusted Issuers Registry**: This contract houses the addresses of all trusted claim issuers associated with a specific token.

- **Claim Topics Registry**: This contract maintains a list of all trusted claim topics related to the security token.

- **Identity Registry**: This contract holds the identity contract addresses of all eligible users authorized to hold the token. It is responsible for claim verification.

- **Compliance Smart Contract**: This contract independently operates to check whether a transfer is in compliance with the established rules for the token.

- **Security Token Contract**: This contract interacts with the Identity Registry to check the eligibility status of investors, enabling token holding and transactions.

## Getting Started

1. Clone the repository: `git clone https://github.com/TokenySolutions/T-REX-Clone.git`
2. Install dependencies: `npm ci`
3. Compile the contracts: `hardhat compile`
4. Run tests: `hardhat test`

## Deployment

1. Replace .env.example with .env and replace
   RPC_URL=<Alchemy/Infura rpc>
   PRIVATE_KEY=<Wallet address private Key>
   BASESCAN_API=<Etherscan or other api key>

2. To deply and mint security token run

```sh
npx hardhat run scripts/deploy.js --netowrk NETWORK
```

Replace NETWORK valide network of your choice (ex: sepolia or base-sepolia)
