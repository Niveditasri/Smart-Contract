# Smart Contract Interaction

This project demonstrates how to interact with a smart contract using a frontend and connect it to a MetaMask wallet for depositing or withdrawing Ether.

## Description

The project consists of three files:
- **deploy.js** (located in the `Scripts` folder)
- **index.js** (located in the `Pages` folder)
- **SmartContract.sol** (located in the `Contracts` folder)

These files work together to enable interactions between the smart contract, frontend, and MetaMask wallet.

## Getting Started

### Installing

You can get started by using Gitpod. Click the link below to open the project in Gitpod:
[Gitpod Link](https://metacrafterc-scmstarter-endrfexphsa.ws-us114.gitpod.io/)

Make sure to copy and paste the following files from the repository into your Gitpod environment:
- `index.js` (frontend code)
- `SmartContract.sol`
- `deploy.js`

### Modifications
No modifications are required to run the program. 

### Executing the Program

1. **Setting up the environment:**
   - Open three terminals in your Gitpod workspace.
   
2. **Deploying the smart contract:**
   - In the second terminal, run the following command to start the Hardhat node:
     ```bash
     npx hardhat node
     ```
   - In the third terminal, deploy the contract:
     ```bash
     npx hardhat run --network localhost scripts/deploy.js
     ```

3. **Launching the frontend:**
   - In the first terminal, start the frontend server:
     ```bash
     npm run dev
     ```
   - The project will be accessible at `http://localhost:3000`.

### Wallet Setup

To interact with the smart contract, you must set up a network in your MetaMask wallet.

1. Open MetaMask and navigate to the settings.
2. Click "Add a Network," then "Add a Network Manually."
3. Enter the following details:
   - **Network name:** (choose any name)
   - **New RPC URL:** `https://8545-metacrafterc-scmstarter-kodhc8ve1v6.ws-us114.gitpod.io`
   - **Chain ID:** `31337`
   - **Currency symbol:** (optional)
4. Import an account using a private key from the second terminal where `npx hardhat node` was executed. Choose any account and copy its private key to import it into MetaMask.

Now, you can interact with the smart contract through MetaMask.

### Transferring Ether

Visit `http://localhost:3000/` again. You can now interact with the frontend, MetaMask wallet, and transfer Ether or tokens as per the smart contract's functionality.

## Help

If you encounter any issues:
- Ensure that your Hardhat node is running (`npx hardhat node`).
- Check the MetaMask network configuration and private key import.

Common command to check for errors:
```bash
npx hardhat help
```

## Authors

- **Nivedita Srivastava** - [GitHub Profile](https://github.com/NiveditaSri)

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
