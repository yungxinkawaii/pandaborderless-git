# DeFi Cross Border Payment Platform - PandaBorderless

This is a monorepo containing 1 project as follows:
- backend API

## Deployment
- Backend (using ): 

## Backend

### Set up hyperledger besu
- Download the Besu packaged binaries at this link, https://github.com/hyperledger/besu/releases", choose 22.10.3 version


### Setting up the server locally
- Clone the project
- Install NodeJS **LTS** version from <a href="https://nodejs.org/en/download/">NodeJs Official Page</a>
- Download the product on this page
- Unzip the downloaded file to a folder in your computer
- Download Ganache from https://trufflesuite.com/ganache/
- Open Terminal
- Go to ./cross-border-payment-api folder
- Run in terminal `npm install nodemon -g`
- Run in terminal `npm install truffle -g`
- Run in terminal `npm install`
- In another terminal of same directory, run ```ganache-cli```
- Go back to the previous terminal and run ```truffle compile``` to compile contract
- Then run ```npm run besu```
- Then run ```truffle migrate --network besu``` to create migrations to deploy migrations and wallet on besu network
- Then run ```truffle test --network besu```
- Then run `npm start`
- Navigate to https://localhost:3333