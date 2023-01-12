# Sample Hardhat Project

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a script that deploys that contract.

first insatll hardhat by
```
npm init -y

npm install --save-dev hardhat @nomicfoundation/hardhat-toolbox

npx install hardhat    
```

or
```

nvm install hardhat //before using this you have to do       “nvm use 18  then nvm install 18”
```

Try running some of the following tasks:

shell
```
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat run scripts/deploy.js
```

# Write NFT Contract Code

Simple you can import from "Openzeppelin" and use the function

install openzeppelin contracts on your system
```
npm install @openzeppelin/contracts
```

In the contracts folder, create a new Solidity file called NFTee.sol and write code there...

# Compile the contract

```
npx hardhat compile
```
If there are no errors, you are good to go :)

# Env file
must create env file in the main folder of your project

add HTTP test net url and your metamask private key there like:

HTTP_URL="add-http-provider-url-here"

PRIVATE_KEY="add-the-private-key-here"

now install dotenv for using env file
```
npm install dotenv
```

Now write code to add your testnet in hardhat.config.js file

For deploy to your test net by 
```
npx hardhat run scripts/deploy.js --network goerli
```

After deploy save your smart contract address for using in web3.js for integration

using the following command for build front end by next.js, firstly

```
npx create-next-app@latest
```

the below command for run localhost for design your front end website
```
npm run dev
```

Now go to http://localhost:3000, your app should be running 

mpw lets start Web3Modal Library by 

```
npm install web3modal
```

Web3Modal is an easy to use library to help developers easily allow their users to connect to your dApps with all sorts of different wallets. By default Web3Modal Library supports injected providers like (Metamask, Dapper, Gnosis Safe, Frame, Web3 Browsers, etc) and WalletConnect, You can also easily configure the library to support Portis, Fortmatic, Squarelink, Torus, Authereum, D'CENT Wallet and Arkane. (Here's a live example on Codesandbox.io)

In the same terminal install ether.js by 

```
npm install ethers
```

You must have to create a new folder under the my-app folder and name it constants. In the constants folder create a file, index.js 
make sure after deploy you must paste your smart contract address and abi into constant folder -> index.js file
To get the ABI for your contract, go to your hardhat-tutorial/artifacts/contracts/Whitelist.sol folder and from your Whitelist.json file get the array marked under the "abi" key (it will be a huge array of about 100 lines or more) and put the abi into abi const...

open terminal in my-app folder, execute 

```
npm run dev
```

Your whitelist dapp should now work without errors 🚀

Thanks me later :)