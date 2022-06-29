# BSC Hello World Tutorial

## Overview

## Prerequisites
  - node --version
    - v16.13.0
  - npm --version 
    - 8.1.0
  - truffle version
    - Truffle v5.5.19 (core: 5.5.19)
    - Ganache v7.2.0
    - Solidity - ^0.8.0 (solc-js)
    - Web3.js v1.5.3
  - MetaMask Wallet
    - 10.16.1

## Setup

1. **Clone the repository**
```git clone https://github.com/RumeelHussain/BSC-Hello-World-Tutorial```
2. **Change the current directory**
```cd BSC-Hello-World-Tutorial```
3. **Install all the dependencies (node modules)**
```npm install```
4. **Compile Smart Contracts**
```truffle compile```
5. **Migrate Smart Contracts**
```truffle migrate --reset --network bscTestnet```
6. **Create build**
```npm run build```
7. **Run the application**
```npm run dev```

## Available Scripts
```
  $ truffle compile
  $ truffle migrate
  $ truffle test
  $ npm run build
  $ npm run test
  $ npm run dev
```

## Structure
```sh
HelloWorld.
|   .env
|   .gitattributes
|   LICENSE
|   package-lock.json
|   package.json
|   README.md
|   truffle-config.js
|   webpack.config.js
|   yarn.lock
| 
+---build
|   \---contracts
|           HelloWorld.json
|           Migrations.json
|           
+---client
|   |   app.js
|   |   chain-smart-bsc-l.png
|   |   index.css
|   |   index.html
|   |   
|           
+---contracts
|       HelloWorld.sol
|       Migrations.sol
|       
+---migrations
|       1_initial_migration.js
|       2_hello_world.js
|                 
+---server
|       main.js
|       
+---test
|       .gitkeep
|       hello_world.js       
|       
```

## How it Works
### Checklist
- Make sure you have MetaMask installed and logged in on your browser.
- Create a file named ```.secret```, save your MetaMask Secret Phrase in this file.
- Run the command ```truffle compile``` to compile the smart contracts.
- Run the command ```truffle migrate --reset --network bscTestnet``` to deploy the contract on the BSC Testnet.
- Run the command ```npm run build``` to build the application.
- Run the command ```npm run dev``` to start the application.

### How to Use
1. Open browser and navigate to ```http://localhost:3000/```
2. Select your desired account of MetaMask that has BNB Test tokens to perform transactions.
3. To get test tokens use the [BNB Smart Chain Faucet](https://testnet.binance.org/faucet-smart).
4. Click on Greet Button to display message, by default its Hello World.
5. Enter a name in the input field, Click save button to save the name.
6. Confirm the transaction when MetaMask notification pops up.
7. Click on Greet Button to display message along with the last name saved with the current account.

## Unit Test Coverage
```sh
  Contract: HelloWorld
    √ Default message should be hello, world (264ms)
    √ Should save name (796ms)
    √ Should be default message for other accounts (412ms)
    √ Should throw error on empty name (3306ms)


  4 passing (5s)
```
## Contact
For more inquiries and conversations, feel free to contact me at rumeelhussain@live.com | rumeelhussain123@gmail.com