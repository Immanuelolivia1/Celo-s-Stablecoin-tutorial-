# The Celo Stablecoin Tutorial
This article dives into the Celo Dollar (cUSD), a stablecoin built on the Celo blockchain. It explains how cUSD works, its stability mechanism, and its advantages in promoting financial accessibility, and lastly, it explains how to write a smart contract using Hardhat and Solidity to build a stablecoin and deploy it on the Celo blockchain.

## Table of Contents
- [The Celo Stablecoin Tutorial](#the-celo-stablecoin-tutorial)
  - [Table of Contents](#table-of-contents)
  - [Abstract](#abstract)
  - [Introduction](#introduction)
  - [Pre-requisites](#pre-requisites)
  - [Requirements](#requirements)
  - [Understanding the Celo Dollar (cUSD)](#understanding-the-celo-dollar-cusd)
  - [How cUSD Works: Exploring the Stability Mechanism](#how-cusd-works-exploring-the-stability-mechanism)
  - [Advantages of the Celo Dollar](#advantages-of-the-celo-dollar)
  - [Building a Stablecoin on the Celo Blockchain](#building-a-stablecoin-on-the-celo-blockchain)
  - [Writing a Smart Contract with Hardhat and Solidity](#writing-a-smart-contract-with-hardhat-and-solidity)
    - [Setting Up Your Development Environment](#setting-up-your-development-environment)
    - [Defining the Stablecoin Contract](#defining-the-stablecoin-contract)
    - [Implementing the Stability Mechanism](#implementing-the-stability-mechanism)
    - [Testing Your Contract](#testing-your-contract)
    - [Deploying to the Celo Blockchain](#deploying-to-the-celo-blockchain)
    - [Interacting with Your Stablecoin](#interacting-with-your-stablecoin)
  - [Conclusion](#conclusion)

## Abstract

This article delves into the world of the Celo Dollar (cUSD), a stablecoin built on the Celo blockchain. By providing a comprehensive overview, aiming to equip readers with a deep understanding of cUSD's functionality, stability mechanism, and the advantages it offers in promoting financial accessibility. Additionally, exploring the process of writing a smart contract using Hardhat and Solidity to build a stablecoin and deploy it on the Celo blockchain. Join me on this journey as I uncover the intricacies of cUSD and its significance in the evolving landscape of digital currencies.

## Introduction

Cryptocurrencies have skyrocketed in popularity in recent years, completely altering how we see and use established financial institutions. Stablecoins are a dependable way to deal with the volatility that many cryptocurrencies face among the wide range of digital currencies. The Celo Dollar (cUSD), a stablecoin that runs on the Celo blockchain, is one example.

The reader will gain a thorough grasp of the Celo Dollar (cUSD) stablecoin after reading this article. We'll delve into its stability mechanism, examine its basic principles, and highlight its benefits for fostering financial accessibility. Additionally, I will walk you through creating a stablecoin and deploying it on the Celo blockchain using a smart contract written in Hardhat and Solidity.


## Pre-requisites

To be able to follow this tutorial, you'll need to have a basic understanding of:

- Solidity
- JavaScript
- [Basis points](https://www.investopedia.com/terms/b/basispoint.asp)
- The [ERC-20](https://ethereum.org/en/developers/docs/standards/tokens/erc-20/) token standard
- [The Chainlink data feeds](https://docs.chain.link/data-feeds#:~:text=Chainlink%20Data%20Feeds%20are%20the,prices%2C%20and%20L2%20sequencer%20health.)
- Finance concepts such as [Collateralization](https://www.investopedia.com/terms/c/collateralization.asp)
- Blockchain concepts such as [Algorithmic stablecoins](https://cointelegraph.com/learn/stablecoins-101-what-are-crypto-stablecoins-and-how-do-they-work)

## Requirements

- [Node.js](https://nodejs.org/en) and npm installed
- A code editor
- The Remix IDE
- A funded account with CELO tokens

## Understanding the Celo Dollar (cUSD)

Understanding the underlying idea of this stablecoin is essential before going into its technical details. A digital version of fiat money (like the US Dollar) with a steady value is called the Celo Dollar (cUSD). Contrary to volatile cryptocurrencies, the cUSD tries to offer stability by utilizing a number of methods to guarantee that its value stays largely consistent.

## How cUSD Works: Exploring the Stability Mechanism

The stability of cUSD is achieved through a mechanism known as a [stability protocol](https://blog.celo.org/diving-into-the-celo-price-stability-protocol-d7afd210609e). This protocol relies on various elements, including collateralization, algorithmic adjustments, and governance mechanisms. By understanding the intricacies of these components, we can gain insight into how cUSD maintains its stable value in the face of market fluctuations.

Collateralization is a key aspect of the stability mechanism. In the case of cUSD, collateral is provided in the form of other digital assets. These assets are held in reserve and serve as a safeguard against potential fluctuations in the value of cUSD. In the event of market volatility, the collateral acts as a buffer, ensuring that the value of cUSD remains pegged to the designated fiat currency.

Algorithmic adjustments play a vital role in maintaining the stability of cUSD. These adjustments are implemented based on the supply and demand dynamics of the stablecoin. When there is an increased demand for cUSD, the algorithm may employ mechanisms to expand the supply, ensuring that there is sufficient liquidity in the market. Conversely, if there is a surplus supply, the algorithm may adjust accordingly to contract the circulating cUSD and maintain stability.

Governance mechanisms are another crucial element in the stability protocol of cUSD. The Celo community actively participates in governing the stablecoin, making decisions related to collateralization ratios, algorithmic adjustments, and other factors that impact stability. This decentralized governance model ensures that the stablecoin remains adaptable and responsive to the evolving needs of the community, further enhancing its stability.

## Advantages of the Celo Dollar

The Celo Dollar has a number of benefits that help it gain popularity and adoption:

- Accessibility: The capacity of the cUSD to encourage financial accessibility is one of its key benefits. People without access to banking services or those who experience economic volatility are frequently left out of traditional financial institutions. This gap is filled by the Celo Dollar (cUSD), which offers a reliable and easily accessible medium of exchange. Users may transact seamlessly and securely thanks to its digital nature, regardless of their location or financial situation. By utilizing the infrastructure of the Celo blockchain, cUSD enables anyone to take part in international economic operations, promoting financial inclusiveness and empowerment.

Moreover, cUSD opens up opportunities for individuals in regions with volatile or underperforming national currencies. By utilizing cUSD, they can mitigate the risks associated with currency fluctuations and maintain a stable store of value. This stability creates a conducive environment for commerce, savings, and investments, enabling economic growth and prosperity.

- Security and transparency: Built on a blockchain, cUSD transactions profit from the security and transparency that come standard with distributed ledger technology. Users benefit from the ease of a reliable medium of exchange while maintaining confidence in the integrity of their transactions.

- Low Transaction Fees: The Celo network boasts low transaction fees, making cUSD an attractive option for microtransactions and everyday purchases. Whether you're sending money to a friend or making a purchase, the cost-efficiency of cUSD makes it a practical choice.

## Building a Stablecoin on the Celo Blockchain
For those interested in creating their stablecoin on the Celo blockchain, understanding the process of writing a smart contract is crucial. Hardhat and Solidity are powerful tools that facilitate the development of smart contracts and their deployment on the Celo blockchain.
<br/>

To begin, you will need to set up your development environment with Hardhat. Hardhat is a popular development framework that simplifies the process of writing, testing, and deploying smart contracts. It provides a comprehensive suite of tools and utilities that aid in the smooth development process.
<br/>

Next, you will write your smart contract using Solidity, a high-level programming language specifically designed for creating smart contracts. Solidity enables you to define the rules and functionalities of your stablecoin, including its stability mechanisms, token supply, and governance structure. By leveraging Solidity's capabilities, you can customize your stablecoin to meet your specific requirements.
<br/>

Once your smart contract is written, you can use Hardhat to compile and deploy it onto the Celo blockchain. Hardhat streamlines the deployment process by providing easy-to-use commands and integration with Celo's infrastructure. Through this process, your stablecoin will become a part of the Celo ecosystem, ready to empower users with stability and financial accessibility.
<br/>

By following these steps and leveraging the capabilities of Hardhat and Solidity, you can build a powerful and reliable stablecoin on the Celo blockchain. Remember to conduct thorough testing, ensure proper security measures, and seek external audits if necessary to provide confidence in your stablecoin's integrity.

## Writing a Smart Contract with Hardhat and Solidity

You will need to build a smart contract utilizing the well-known development framework Hardhat and the programming language Solidity to start creating your stablecoin on the Celo network. The essential steps are as follows:

### Setting Up Your Development Environment 
Start by installing Hardhat, a powerful tool for Ethereum and Celo development. Once installed, create a new directory for your project and initialize it with Hardhat.

1. Install Hardhat globally:

    ```bash
    npm install --save-dev hardhat
    ```


2. Create a new directory for your project:

    ```bash
    mkdir my-stablecoin-project
    ```
3. Change directory to the project's folder:
    ```bash
    cd my-stablecoin-project
    ```

4. Initialize the project with Hardhat:

    ```bash
    npx hardhat init
    ```

The above code snippet assumes you have Node.js and npm (Node Package Manager) installed on your machine. By following these steps, you will have Hardhat installed globally and a new directory created for your stablecoin project. The **`npx hardhat init`** command initializes the project with the necessary configuration files and folder structure provided by Hardhat, allowing you to start developing and deploying your smart contracts on the Celo blockchain.
<br/>

Please note that you may need to customize the project configuration and install additional dependencies based on your specific requirements. Make sure to refer to the [Hardhat documentation](https://hardhat.org/hardhat-runner/docs/config) for further guidance on configuring and extending your project.

### Defining the Stablecoin Contract
Within your project directory, create a new Solidity file for your stablecoin contract. Define the necessary variables and functions to handle the token's supply, transfers, and stability mechanisms. Consider incorporating the Celo Stability Protocol into your contract design.

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract MyStablecoin is ERC20 {
    address private governance;
    uint256 private reserveRatio;

    constructor() ERC20("My Stablecoin", "MYS") {
        governance = msg.sender;
        reserveRatio = 2000; // Example reserve ratio, adjust as needed
    }

    modifier onlyGovernance() {
        require(msg.sender == governance, "Only governance can call this function");
        _;
    }

    modifier checkAmount(uint256 amount){
        require(amount > 0, "Invalid amount");
        _;
    }

     /** @dev Creates `amount` tokens and assigns them to `recipient`, increasing
     * the total supply.
     *
     * Requirements:
     *
     * - `recipient` cannot be the zero address.
     * - `amount` cannot be zero.
     */
    function mint(address recipient, uint256 amount) external onlyGovernance checkAmount(amount) {    
        _mint(recipient, amount);
    }

    /**
     * @dev Destroys `amount` tokens from `msg.sender`, reducing the
     * total supply.
     *
     * Requirements:
     *
     * - `msg.sender` cannot be the zero address.
     * - `msg.sender` must have at least `amount` tokens.
     * - `amount` cannot be zero.
     */
    function burn(uint256 amount) external checkAmount(amount) {
        _burn(msg.sender, amount);
    }

    /**
     * @dev Moves `amount` of tokens from `msg.sender` to `recipient`.
     *
     * Requirements:
     *
     * - `msg.sender` cannot be the zero address.
     * - `recipient` cannot be the zero address.
     * - `msg.sender` must have a balance of at least `amount`.
     */
    function transfer(address recipient, uint256 amount) public override returns (bool) {
        require(amount <= _calculateStability(amount), "Transfer amount exceeds stability limit");
        return super.transfer(recipient, amount);
    }


    /**
     * @dev  Moves `amount` of tokens from `sender` to `recipient`
     *
     * Requirements:
     *
     * - `sender` and `to` cannot be the zero address.
     * - `sender` must have a balance of at least `amount`.
     * - the caller must have allowance for ``sender``'s tokens of at least
     * `amount`.
     * - `amount` needs to be lower than the required fractional reserve the smart contract has to maintain
     */
    function transferFrom(
        address sender,
        address recipient,
        uint256 amount
    ) public override returns (bool) {
        require(amount <= _calculateStability(amount), "Transfer amount exceeds stability limit");
        return super.transferFrom(sender, recipient, amount);
    }

    /**
     * @dev  Returns the maximum allowed amount to trade
     */
    function _calculateStability(uint256 amount) private view returns (uint256) {
        uint256 totalSupply = totalSupply();
        uint256 reserve = (totalSupply * reserveRatio) / 10000; // adjust to decimal percentage
        return totalSupply - reserve - amount;
    }
}
```

In the above code snippet, we define a **`MyStablecoin`** contract that extends the **`ERC20`** contract from the OpenZeppelin library. The contract initializes with a governance address and a reserve ratio, which represents the portion of the total supply reserved to maintain stability.

The **`mint`** function allows the governance address to mint new stablecoins and allocate them to a recipient. The **`burn`** function enables users to burn their stablecoins and reduce the token supply.

The **`transfer`** and **`transferFrom`** functions override the corresponding functions in the ERC20 contract. Before executing the transfer, these functions verify that the transfer amount does not exceed the stability limit, calculated based on the reserve ratio.

The **`_calculateStability`** internal function calculates the maximum transferable amount by subtracting the reserve and the desired transfer amount from the total supply.

Make sure to customize the contract name, token symbol, reserve ratio, and other aspects based on your specific requirements.


### Implementing the Stability Mechanism
Utilize the functionality provided by the Celo blockchain to implement the stability mechanism of your stablecoin. This may involve interacting with Celo's Oracle system to fetch real-time price information and adjusting the supply of your stablecoin accordingly.
<br/>

Here are some code samples that show how you can use the capabilities of the Celo blockchain to implement the stability mechanism in your stablecoin contract. These examples include connecting with Celo's Oracle system and modifying the token supply based on current pricing information.

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";
import { AggregatorV3Interface } from "./AggregatorV3Interface.sol";

contract MyStablecoin is ERC20 {
    address private governance;
    uint256 private reserveRatio;
    AggregatorV3Interface private priceFeed;

    constructor(address _priceFeedAddress) ERC20("My Stablecoin", "MYS") {
        governance = msg.sender;
        reserveRatio = 2000; // Example reserve ratio, adjust as needed. Currently represents 2000(20%) basis points
        priceFeed = AggregatorV3Interface(_priceFeedAddress);
    }

    modifier onlyGovernance() {
        require(msg.sender == governance, "Only governance can call this function");
        _;
    }

    modifier checkAmount(uint256 amount){
        require(amount > 0, "Invalid amount");
        _;
    }


     /** @dev Creates `amount` tokens and assigns them to `recipient`, increasing
     * the total supply.
     *
     * Requirements:
     *
     * - `recipient` cannot be the zero address.
     * - `amount` cannot be zero.
     */
    function mint(address recipient, uint256 amount) external onlyGovernance checkAmount(amount) {    
        _mint(recipient, amount);
    }

    /**
     * @dev Destroys `amount` tokens from `msg.sender`, reducing the
     * total supply.
     *
     * Requirements:
     *
     * - `msg.sender` cannot be the zero address.
     * - `msg.sender` must have at least `amount` tokens.
     * - `amount` cannot be zero.
     */
    function burn(uint256 amount) external checkAmount(amount) {
        _burn(msg.sender, amount);
    }

    /**
     * @dev Moves `amount` of tokens from `msg.sender` to `recipient`.
     *
     * Requirements:
     *
     * - `msg.sender` cannot be the zero address.
     * - `recipient` cannot be the zero address.
     * - `msg.sender` must have a balance of at least `amount`.
     */
    function transfer(address recipient, uint256 amount) public override returns (bool) {
        require(amount <= _calculateStability(amount), "Transfer amount exceeds stability limit");
        return super.transfer(recipient, amount);
    }


    /**
     * @dev  Moves `amount` of tokens from `sender` to `recipient`
     *
     * Requirements:
     *
     * - `sender` and `to` cannot be the zero address.
     * - `sender` must have a balance of at least `amount`.
     * - the caller must have allowance for ``sender``'s tokens of at least
     * `amount`.
     * - `amount` needs to be lower than the required fractional reserve the smart contract has to maintain
     */
    function transferFrom(
        address sender,
        address recipient,
        uint256 amount
    ) public override returns (bool) {
        require(amount <= _calculateStability(amount), "Transfer amount exceeds stability limit");
        return super.transferFrom(sender, recipient, amount);
    }

    /**
     * @dev  Returns the maximum allowed amount to trade
     */
    function _calculateStability(uint256 amount) private view returns (uint256) {
        uint256 totalSupply = totalSupply();
        uint256 reserve = (totalSupply * reserveRatio) / 10000; // adjust to decimal percentage
        return totalSupply - reserve - amount;
    }

    /**
     * @dev  Updates the address of the `updatePriceFeedAddress` to `_priceFeedAddress`
     *
     * Requirements:
     *
     * - `_priceFeedAddress` cannot be the zero address.
     * - `sender` must be the `governance`.
     */
    function updatePriceFeedAddress(address _priceFeedAddress) external onlyGovernance {
        require(_priceFeedAddress != address(0), "Invalid price feed address");
        priceFeed = AggregatorV3Interface(_priceFeedAddress);
    }

    /**
     * @dev  Returns the latest price of MYS tokens
     *
     */
    function getLatestPrice() public view returns (uint256) {
        (, int256 price, , , ) = priceFeed.latestRoundData();
        require(price > 0, "Invalid price"); // Ensure the price is positive
        return uint256(price);
    }

    /**
     * @dev  Updates the address of the `updatePriceFeedAddress` to `_priceFeedAddress`
     *
     * Requirements:
     *
     * - `sender` must be the `governance`.
     */
    function adjustSupply() external onlyGovernance {
        uint256 currentPrice = getLatestPrice();
        uint256 totalSupply = totalSupply();
        uint256 reserve = (totalSupply * reserveRatio) / 10000;
        uint256 targetSupply = reserve / currentPrice;
        if (totalSupply > targetSupply) {
            uint256 amountToBurn = totalSupply - targetSupply;
            _burn(governance, amountToBurn);
        } else if (totalSupply < targetSupply) {
            uint256 amountToMint = targetSupply - totalSupply;
            _mint(governance, amountToMint);
        }
    }
}
```

In the above code snippet, we have made several updates to the previous stablecoin contract:

- We import the **`AggregatorV3Interface`** from the **`AggregatorV3Interface.sol`** file, which provides an interface for interacting with Celo's Oracle system.

- The constructor now takes an address parameter **`_priceFeedAddress`**, which represents the address of the Celo Oracle price feed.

- The **`updatePriceFeedAddress`** function allows the governance address to update the price feed address if needed.

- The **`getLatestPrice`** function retrieves the latest price from the Oracle system using the **`latestRoundData`** function provided by the **`AggregatorV3Interface`**. It ensures that the price is positive before returning it.

- The **`adjustSupply`*** function is called by the governance address to adjust the stablecoin's supply based on the target reserve ratio. It fetches the current price from the Oracle system, calculates the target supply based on the reserve and the current price, and adjusts the supply accordingly. If the total supply is greater than the target supply, it burns the excess tokens. If the total supply is less than the target supply, it mints additional tokens.

>**_Note_**: You can find the code for the AggregatorV3Interface by going to https://github.com/smartcontractkit/chainlink/blob/develop/contracts/src/v0.8/interfaces/AggregatorV3Interface.sol

### Testing Your Contract
To ensure the security and operation of your smart contract, it is essential to run a thorough test of it. You can create thorough test cases to verify your stablecoin's functionality in various scenarios using the strong testing framework offered by Hardhat.

### Deploying to the Celo Blockchain
Once your contract passes all tests, it's time to deploy it to the Celo blockchain. Hardhat provides deployment scripts that make it straightforward to deploy your contract to the Celo network. Ensure you have the necessary Celo account and network configurations in place.

To deploy to the Celo Alfajores testnet, you'll need to configure your `hardhat.config.js` as follows:

```js

require("@nomiclabs/hardhat-waffle");

// Export the Hardhat configuration object
module.exports = {
  // Specify the networks to be used
  networks: {
    // Local development network
    hardhat: {},
    // Celo Alfajores testnet
    alfajores: {
      url: "https://alfajores-forno.celo-testnet.org",
      // Replace <your-private-key> with your own private key
      accounts: ["<your-private-key>"],
      chainId: 44787,
    }
  },
  // Specify the version of Solidity to be used
  solidity: {
    version: "0.8.0",
    // Specify settings for the Solidity compiler
    settings: {
      // Enable the optimizer
      optimizer: {
        enabled: true,
        // Specify the number of optimization runs
        runs: 200
      }
    }
  }
};

```

Here is an example of code that shows how to use Hardhat's deployment tools to publish your stablecoin contract to the Celo blockchain:

```javascript
// deploy.js
async function main() {
  // Set up your Celo account and network configurations
  const [deployer] = await ethers.getSigners();

  console.log("Deploying contracts with the account:", deployer.address);

  // Set up your contract deployment parameters
  const stablecoinName = "My Stablecoin";
  const stablecoinSymbol = "MYS";
  const priceFeedAddress = "0x1234567890123456789012345678901234567890"; // Replace with actual Oracle price feed address

  // Deploy your stablecoin contract
  const Stablecoin = await ethers.getContractFactory("MyStablecoin");
  const stablecoin = await Stablecoin.deploy(priceFeedAddress);

  await stablecoin.deployed();

  console.log("Stablecoin deployed to:", stablecoin.address);
}

main()
  .then(() => process.exit(0))
  .catch((error) => {
    console.error(error);
    process.exit(1);
  });
  ```
  
  
The JavaScript deployment script in the code snippet above makes use of Hardhat to upload the stablecoin contract to the Celo network. The script is broken down as follows:

- First, we set up the necessary configurations and obtain the deployer's Celo account using **`ethers.getSigners()`**.

- Next, we define the parameters for the stablecoin contract deployment, including the name, symbol, and address of the Oracle price feed.

- We then use **`ethers.getContractFactory()`** to obtain the contract factory for the stablecoin contract.

- After that, we deploy the stablecoin contract using **`stablecoin.deploy(priceFeedAddress)`**. This deploys the contract with the provided price feed address as a constructor parameter.

- Finally, we log the deployed contract's address to the console.

To deploy the contract, you can run this script using Hardhat's deployment command, such as **`npx hardhat run deploy.js --network celo`**. Ensure that you have the necessary network configurations in the Hardhat configuration file, such as the RPC URL and the private key of the deployer account.

Please note that the code snippet assumes you have a valid Oracle price feed address and that you've replaced the placeholder address **(`0x1234567890123456789012345678901234567890`)** with the actual address of the Oracle price feed.

### Interacting with Your Stablecoin
Using a variety of wallets and programs that are compatible with Celo, you can now interact with your stablecoin after it has been deployed. To guarantee seamless use, test transactions, transfers, and other features.

You may create a strong and dependable stablecoin on the Celo blockchain by following these instructions and utilizing the abilities of Hardhat and Solidity. To give people confidence in the integrity of your stablecoin, don't forget to do extensive testing, establish appropriate security measures, and request external audits if necessary.


## Conclusion
In conclusion, the Celo Dollar (cUSD) stands as an impressive stablecoin built on the Celo blockchain, promoting financial accessibility and stability. Understanding its stability mechanism and advantages helps shed light on its potential impact on the world of decentralized finance. Furthermore, with the guidance provided on writing a smart contract using Hardhat and Solidity, you now have the tools to embark on your own stablecoin creation journey on the Celo blockchain.

Harness the power of cUSD and explore the possibilities of stablecoin innovation on the Celo network. By adhering to best practices, conducting thorough testing, and building on the robust infrastructure provided by Celo and Hardhat, you can contribute to the exciting and rapidly evolving world of decentralized finance.

































