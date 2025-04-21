# Cairo Smart Contract: Counter

This project demonstrates a simple Cairo smart contract deployed on StarkNet. The contract implements a counter with functionalities to get, set, and increment the counter value.

## Project Structure

- **src/**
  - `lib.cairo`: Entry point for the Cairo modules.
  - `counter.cairo`: Contains the implementation of the counter contract.
- **scripts/**
  - `deploy.ts`: Script to deploy the counter contract on StarkNet.
  - `utils.ts`: Utility functions for reading compiled contract files.
- **Scarb.toml**: Configuration file for the Scarb package manager.
- **package.json**: Node.js project configuration file.

## Prerequisites

- Node.js (v16 or higher)
- Scarb (Cairo package manager)
- StarkNet CLI
- Cairo language support

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd cairo-contract
   ```

2. Install Node.js dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   Create a `.env` file in the root directory with the following variables:
   ```
   RPC_ENDPOINT=<StarkNet RPC endpoint>
   DEPLOYER_ADDRESS=<Deployer account address>
   DEPLOYER_PRIVATE_KEY=<Deployer private key>
   ```

## Usage

### Compile the Contract

Use Scarb to compile the contract:
```bash
scarb build
```

### Deploy the Contract

Run the deployment script:
```bash
npm run deploy
```

### Contract Functionalities

The contract provides the following functionalities:
- **Get Counter**: Retrieve the current counter value.
- **Set Counter**: Set the counter to a specific value.
- **Increase Counter**: Increment the counter by 1.

## Project Dependencies

- [StarkNet.js](https://www.npmjs.com/package/starknet): JavaScript library for interacting with StarkNet.
- [dotenv](https://www.npmjs.com/package/dotenv): For managing environment variables.
- [ts-node](https://www.npmjs.com/package/ts-node): TypeScript execution environment.

## License

This project is licensed under the MIT License.