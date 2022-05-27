# ETHEREUM-TODO LIST

A blockchain based ToDoList that runs on Ethereum Networks. Every
task added or completed triggers a smart contract and is counted as
a transaction on the blockchain. A new block is mined for every
transaction. The Wallet balance before and after every transaction
also reflects on Metamask Wallet (or any Ethereum Wallet).

<hr>

## Project Structure

    ├── LICENSE.md           ->    License file.
    |
    ├── README.md            ->    The top-level README for developers/collaborators using this project.
    |
    ├── build                ->    Compiled Smart Contracts (JSON).
    |
    ├── contracts            ->    Contains two contracts: Migration.sol (to migrate the contract onto blockchain) and ToDoList.sol (the contract responsible for ToDoList transactions).
    |
    ├── Migrations           ->    Pushes the desired files to the blockchain.
    │   
    ├── source               ->    Source code for frontend and JavaScript file linked with the contracts.
        │
        └── images           ->    Images used in frontend part.      
    │
    ├── test                 ->    Test set for testing the DAPP's working.
    │
    ├── package.json         ->    Information regarding name of package and versions of modules used.
    │ 
    └── truffle-config.js    ->    Port Configuration for Truffle.     

## Project Setup 

Open the Command line or Terminal

- Clone the repository

```
git clone https://github.com/pavvann/ToDoList-on-Ethereum
```

- Move to the folder

```
cd DAPP
```

- Download Truffle

```
npm install -g truffle@5.0.2
```

- Download Ganache - https://trufflesuite.com/ganache/

- Compile the contracts

```
truffle compile
```

- Migrate the contracts (Ganache must be running)

```
truffle migrate --reset
```

- Connect your Metamask to the Local Network and add the Ganache Private Account

- Deploy the package

```
npm run dev
```

**_NOTE:_** Metamask and other wallets keep on changing the protocols to work with the blockchain to ensure safety. "Deprecated" error might appear in future. Check official Metamask documentation for updates.