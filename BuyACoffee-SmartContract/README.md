You can see a demo of this repo on Replit : https://replit.com/@farhan756/BuyMeACoffee-Website?v=1


# BuyMeACoffee solidity contract

This repo contains a contract that implements tipping functionality.

Install dependencies with `npm install`.

Set up by creating a `.env` file, and filling out these variables:

```
GOERLI_URL="your Alchemy RPC URL"
GOERLI_API_KEY="your Alchemy API key"
PRIVATE_KEY="your wallet private key"
```



## !!! Be very careful with exporting your private key !!!

Deploy your contract with:

```
npx hardhat run scripts/deploy.js
```

Run an example buy coffee flow locally with:

```
npx hardhat run scripts/buy-coffee.js
```

Once you have a contract deployed to Goerli testnet, grab the contract address and update the `contractAddress` variable in `scripts/withdraw.js`, then:

```
npx hardhat run scripts/withdraw.js
```

will allow you to withdraw any tips stored on the contract.

 