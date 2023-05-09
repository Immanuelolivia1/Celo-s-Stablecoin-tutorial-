# Tutorial of Celo Stablecoin:

## Table of Contents:

- [Celo-Stablecoin-tutorial](#Celo-Stablecoin-tutorial)
  - [Abstract](#abstract)
  - [Introduction](#introduction)
  - [Requirements](#requirements)
  - [Understanding the Celo Dollar (cUSD)](#Understanding-the-Celo-Dollar-(cUSD))
  - [How cUSD Works: Exploring the Stability Mechanism](#how-cUSD-works-exploring-the-stability-mechanism)
  - [Advantages of cUSD: Promoting Financial Accessibility](#advantages-of-cUSD-promoting-financial-accessibility)
  - [Building a Stablecoin on the Celo Blockchain](#building-a-stablecoin-on-the-celo-blockchain)
  - [Writing a Smart Contract with Hardhat and Solidity](#writing-a-smart-contract-with-hardhat-and-solidity)
    - [Setting Up Your Development Environment](#setting-up-your-development-environment)
    - [Defining the Stablecoin Contract](#defining-the-stablecoin-contract)
    - [Implementing the Stability Mechanism](#implementing-the-stability-mechanism)
    - [Testing Your Contract](#testing-your-contract)
    - [Deploying to the Celo Blockchain](#deploying-to-the-celo-blockchain)
    - [Interacting with Your Stablecoin](#interacting-with-your-stablecoin)
  - [Conclusion](#conclusion)

## Abstract:

This tutorial delves into the world of Celo Dollar (cUSD) which a stablecoin built on the Celo blockchain. By providing a comprehensive overview to equip readers with a deep understanding of cUSD's functionality, stability mechanism and the advantages it offers in promoting financial accessibility. Additionally, exploring  the process of writing a Smart Contract using [Hardhat](https://hardhat.org/) and [Solidity](https://docs.soliditylang.org/en/v0.8.19/) to build a stablecoin and deploy it on the Celo blockchain. 
Join me on this exciting journey as I uncover the intricacies of cUSD and its significance in the evolving landscape of digital currencies!!

## Introduction:

Cryptocurrencies's popularity has skyrocketed in the recent years, completely altering how we see and use established financial institutions. Stablecoins are a dependable way to deal with the volatility that many cryptocurrencies face among the wide range of digital currencies. The Celo Dollar (cUSD) is a stablecoin that runs on the Celo blockchain, is one such example.

The reader will gain a thorough grasp of the Celo Dollar (cUSD) stablecoin after reading this tutorial. We'll delve into its stability mechanism, examine its basic principles and highlight its benefits for fostering financial accessibility. Additionally, I will walk you through creating a stablecoin and deploying it on the Celo blockchain using a Smart Contract written using [Hardhat](https://hardhat.org/) and [Solidity](https://docs.soliditylang.org/en/v0.8.19/).

## Requirements:

Install the following in your computer:

1. [Remix IDE](https://remix.ethereum.org/#lang=en&optimize=false&runs=200&evmVersion=null&version=soljson-v0.8.18+commit.87f61d96.js)
2. [Celo Extension wallet](https://chrome.google.com/webstore/detail/celoextensionwallet/kkilomkmpmkbdnfelcpgckmpcaemjcdh?hl=en)
3. [Node.js](https://nodejs.org/en/download)
4. [npm](https://www.npmjs.com/package/download) (Node Package Manager)
5. [Hardhat](https://hardhat.org/)

## Understanding the Celo Dollar (cUSD):

Understanding the underlying idea of this stablecoin is essential before going into its technical details. A digital version of fiat money (like the US Dollar) with a steady value is called the Celo Dollar (cUSD). Contrary to volatile cryptocurrencies, the cUSD tries to offer stability by utilizing a number of methods to guarantee that its value stays largely consistent.

## How cUSD Works: Exploring the Stability Mechanism-

The stability of cUSD is achieved through a mechanism called **stability protocol**. This protocol relies on various elements like collateralization, algorithmic adjustments and governance mechanisms. By understanding the intricacies of these components, we can gain insight into how cUSD maintains its stable value in the face of market fluctuations.

Collateralization is a key aspect of the stability mechanism. In the case of cUSD, collateral is provided in the form of other digital assets. These assets are held in reserve and serve as a safeguard or buffer against potential fluctuations, ensuring that the value of cUSD remains pegged to the designated fiat currency.

Algorithmic adjustments play a vital role in maintaining the stability of cUSD. These adjustments are implemented based on the supply and demand dynamics of the stablecoin. When there is an increased demand for cUSD, the algorithm may employ mechanisms to expand the supply, ensuring that there is sufficient liquidity in the market. Conversely if there is a surplus supply, the algorithm may adjust accordingly to contract the circulating cUSD and maintain stability.

Governance mechanisms are another crucial element in the stability protocol of cUSD. The Celo community actively participates in governing the stablecoin, making decisions related to collateralization ratios, algorithmic adjustments and other factors that impact stability. This decentralized governance model ensures that the stablecoin remains adaptable and responsive to the evolving needs of the community which further enhances its stability.

## Advantages of the Celo Dollar:

1. **Accessibility:** People without access to banking services or those who experience economic volatility are frequently left out of traditional financial institutions. This gap is filled by the Celo Dollar (cUSD) which offers a reliable and easily accessible medium of exchange. Users may transact seamlessly and securely due to its digital nature, regardless of their location or financial situation. By utilizing the infrastructure of the Celo blockchain, cUSD enables anyone to take part in international economic operations promoting financial inclusiveness and empowerment.
Moreover, cUSD opens up opportunities for individuals in regions with volatile or underperforming national currencies. By utilizing cUSD, they can mitigate the risks associated with currency fluctuations and maintain a stable store of value. This stability creates a conducive environment for commerce, savings and investments enabling economic growth and prosperity to the vulnerables.

2. **Security & transparency:** come standard with distributed ledger technology. Users benefit from the ease of a reliable medium of exchange while maintaining confidence in the integrity of their transactions.

3. **Low Transaction Fees:** makes cUSD an attractive option for microtransactions and everyday purchases. Whether you're sending money to a friend or making a purchase, the cost-efficiency of cUSD makes it a practical choice.

## Building a Stablecoin on the Celo Blockchain:

For those interested in creating their own stablecoin on the Celo blockchain, understanding the process of writing a Smart Contract is crucial. Hardhat and Solidity are powerful tools that facilitate the development of Smart Contracts and their deployment on the Celo blockchain.
<br/>

To begin, you will need to set up your development environment using Hardhat. **Hardhat** is a popular development framework that simplifies the process of writing, testing and deploying Smart Contracts. It provides a comprehensive suite of tools and utilities that aid in the smooth development process.
<br/>

Next, you will write your Smart Contract using Solidity which is a high-level programming language specifically designed for creating Smart Contracts. Solidity enables you to define the rules & functionalities of your stablecoin like its stability mechanisms, token supply and governance structure. By leveraging Solidity's capabilities, you can customize your stablecoin to meet your favored requirements.
<br/>

Once your Smart Contract is written, you can use Hardhat to compile and deploy it onto the Celo blockchain. Hardhat streamlines the deployment process by providing easy-to-use commands and integration with Celo's infrastructure. Through this process, your stablecoin will become a part of the Celo ecosystem, ready to empower users with stability and financial accessibility.
<br/>

By following these steps and leveraging the capabilities of Hardhat and Solidity, you can build a powerful and reliable stablecoin on the Celo blockchain. Remember to conduct thorough testing, ensure proper security measures and seek external audits (if necessary) in order to provide confidence in your stablecoin's integrity.

## Writing a Smart Contract using Hardhat and Solidity:

You will need to build a Smart Contract utilizing the well-known development framework "Hardhat" and the programming language "Solidity" to start creating your stablecoin on the Celo network. The essential steps are as follows:

### Setting Up Your Development Environment:

Start by installing Hardhat, a powerful tool for Ethereum and Celo development. Once installed, create a new directory for your project and initialize it with Hardhat.

1. Install Hardhat globally:

``npm install -g hardhat``


2. Create a new directory for your project:

```mkdir my-stablecoin-project```

```cd my-stablecoin-project```

3. Initialize the project with Hardhat:

```npx hardhat init```

The above code snippet assumes you have [Node.js](https://nodejs.org/en/download) and [npm](https://www.npmjs.com/package/download) (Node Package Manager) installed on your machine. By following these steps, you will have Hardhat installed globally and a new directory created for your stablecoin project. The **```npx hardhat init```** command initializes the project with the necessary configuration files and folder structure provided by Hardhat, allowing you to start developing and deploying your Smart Contracts on the Celo blockchain.
<br/>

Note: You may need to customize the project configuration and install additional dependencies based on your specific requirements. Make sure to refer to the [Hardhat documentation](https://hardhat.org/docs) for further guidance on configuring and extending your project.

### Defining the Stablecoin Contract:

Within your project directory, create a new Solidity file for your stablecoin contract. Define the necessary variables and functions to handle the token's supply, transfers and stability mechanisms. Consider incorporating the Celo Stability Protocol into your contract design.

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";
import "@openzeppelin/contracts/utils/math/SafeMath.sol";

contract MyStablecoin is ERC20 {
    using SafeMath for uint256;

    address private governance;
    uint256 private reserveRatio;
    mapping(address => uint256) private reserveFunds;

    constructor() ERC20("My Stablecoin", "MYS") {
        governance = msg.sender;
        reserveRatio = 2000; // Example reserve ratio, adjust as needed
    }

    modifier onlyGovernance() {
        require(msg.sender == governance, "Only governance can call this function");
        _;
    }

    function setReserveRatio(uint256 ratio) external onlyGovernance {
        reserveRatio = ratio;
    }

    function mint(address recipient, uint256 amount) external onlyGovernance {
        _mint(recipient, amount);
    }

    function burn(uint256 amount) external {
        _burn(msg.sender, amount);
    }

    function transfer(address recipient, uint256 amount) public override returns (bool) {
        require(amount <= _calculateStability(amount), "Transfer amount exceeds stability limit");
        return super.transfer(recipient, amount);
    }

    function transferFrom(
        address sender,
        address recipient,
        uint256 amount
    ) public override returns (bool) {
        require(amount <= _calculateStability(amount), "Transfer amount exceeds stability limit");
        return super.transferFrom(sender, recipient, amount);
    }

    function withdrawReserve(uint256 amount) external onlyGovernance {
        require(amount <= reserveFunds[msg.sender], "Insufficient reserve funds");
        reserveFunds[msg.sender] = reserveFunds[msg.sender].sub(amount);
        _burn(address(this), amount);
        payable(msg.sender).transfer(amount);
    }

    function _calculateStability(uint256 amount) private view returns (uint256) {
        uint256 totalSupply = totalSupply();
        uint256 reserve = totalSupply.mul(reserveRatio).div(10000); // adjust to decimal percentage
        uint256 totalReserve = balanceOf(address(this));
        uint256 stabilityAmount = totalSupply.sub(reserve).sub(totalReserve).sub(amount);
        return stabilityAmount;
    }

    receive() external payable {
        reserveFunds[msg.sender] = reserveFunds[msg.sender].add(msg.value);
    }
}

```

In the above code snippet:

1. Define a **`MyStablecoin`** contract that extends the **`ERC20`** contract from the OpenZeppelin library. The contract initializes with a governance address and a reserve ratio, which represents the portion of the total supply reserved to maintain stability.

2. **`mint`** function: allows the governance address to `mint` new stablecoins and allocate them to a recipient. 

3. **`burn`** function: enables users to burn their stablecoins and reduce the token supply.

4. **`transfer`** and **`transferFrom`** functions: override the corresponding functions in the ERC20 contract. Before executing the transfer, these functions verify that the transfer amount does not exceed the stability limit, calculated based on the reserve ratio.

5. **`_calculateStability`** internal function: calculates the maximum transferable amount by subtracting the reserve and the desired transfer amount from the total supply.

Make sure to customize the contract name, token symbol, reserve ratio and other aspects based on your specific requirements.

### Implementing the Stability Mechanism:

Utilize the functionality provided by the Celo blockchain to implement the stability mechanism of your stablecoin. This may involve interacting with Celo's Oracle system to fetch real-time price information and adjusting the supply of your stablecoin accordingly.
<br/>

Here are some code samples that show how you can use the capabilities of the Celo blockchain to implement the stability mechanism in your stablecoin contract. These examples include connecting with Celo's Oracle system and modifying the token supply based on current pricing information.

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";
import { AggregatorV3Interface } from "./AggregatorV3Interface.sol";

contract MyStablecoin is ERC20 {
address public governance;
uint256 public reserveRatio;
AggregatorV3Interface public priceFeed;

   constructor(address _priceFeedAddress) ERC20("My Stablecoin", "MYS") {
    governance = msg.sender;
    reserveRatio = 200000000000000000; // 20% represented in wei
    priceFeed = AggregatorV3Interface(_priceFeedAddress);
}

modifier onlyGovernance() {
    require(msg.sender == governance, "Only governance can call this function");
    _;
}

function mint(address recipient, uint256 amount) external onlyGovernance {
    _mint(recipient, amount);
}

function burn(uint256 amount) external {
    _burn(msg.sender, amount);
}

function transfer(address recipient, uint256 amount) public override returns (bool) {
    require(amount <= calculateStability(amount), "Transfer amount exceeds stability limit");
    return super.transfer(recipient, amount);
}

function transferFrom(
    address sender,
    address recipient,
    uint256 amount
) public override returns (bool) {
    require(amount <= calculateStability(amount), "Transfer amount exceeds stability limit");
    return super.transferFrom(sender, recipient, amount);
}

function calculateStability(uint256 amount) public view returns (uint256) {
    uint256 totalSupply = totalSupply();
    uint256 reserve = totalSupply * reserveRatio / 1000000000000000000; // convert back to ether
    return totalSupply - reserve - amount;
}

function updatePriceFeedAddress(address _priceFeedAddress) external onlyGovernance {
    priceFeed = AggregatorV3Interface(_priceFeedAddress);
}

function getLatestPrice() public view returns (uint256) {
    (, int256 price, , , ) = priceFeed.latestRoundData();
    require(price > 0, "Invalid price"); // Ensure the price is positive
    return uint256(price);
}

function adjustSupply() external onlyGovernance {
    uint256 currentPrice = getLatestPrice();
    uint256 totalSupply = totalSupply();
    uint256 reserve = totalSupply * reserveRatio / 1000000000000000000; // convert back to ether
    uint256 targetSupply = reserve * 1000000000000000000 / currentPrice; // convert to wei
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

1. Imported the **`AggregatorV3Interface`** from the **`AggregatorV3Interface.sol`** file, which provides an interface for interacting with Celo's Oracle system.

2, The constructor now takes an address parameter **`_priceFeedAddress`**, which represents the address of the Celo Oracle price feed.

3. The **`updatePriceFeedAddress`** function allows the governance address to update the price feed address if needed.

4. The **`getLatestPrice`** function retrieves the latest price from the Oracle system using the **`latestRoundData`** function provided by the **`AggregatorV3Interface`**. It ensures that the price is positive before returning it.

5. The **`adjustSupply`*** function is called by the governance address to adjust the stablecoin's supply based on the target reserve ratio. It fetches the current price from the Oracle system, calculates the target supply based on the reserve and the current price and adjusts the supply accordingly. If the total supply is greater than the target supply, it burns the excess tokens. If the total supply is less than the target supply, it mints additional tokens.

Note: The code assumes the availability of the AggregatorV3.

### Testing Your Contract:

To ensure the security and operation of your Smart Contract, it is essential to run a thorough test of it. You can create thorough test cases to verify your stablecoin's functionality in various scenarios using the strong testing framework offered by Hardhat.

### Deploying to the Celo Blockchain:

Once your contract passes all tests, it's time to deploy it to the Celo blockchain. Hardhat provides deployment scripts that make it straightforward to deploy your contract to the Celo network. Ensure you have the necessary Celo account and network configurations in place.

Here is an example of code that shows how to use Hardhat's deployment tools to publish your stablecoin contract to the Celo blockchain:

```javascript
/ deploy.js
// This script deploys a stablecoin contract on the Celo network using an Oracle price feed address

async function main() {
// Set up your Celo account and network configurations
const [deployer] = await ethers.getSigners();

console.log("Deploying contracts with the account:", deployer.address);

// Set up your contract deployment parameters
const stablecoinName = "My Stablecoin"; // The name of the stablecoin
const stablecoinSymbol = "MYS"; // The symbol of the stablecoin
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

1. Set up the necessary configurations and obtain the deployer's Celo account using **`ethers.getSigners()`**.

2. Define the parameters for the stablecoin contract deployment, including the name, symbol and the address of the Oracle price feed.

3. Use **`ethers.getContractFactory()`** to obtain the contract factory for the stablecoin contract.

4. Deploy the stablecoin contract using **`stablecoin.deploy(priceFeedAddress)`**. This deploys the contract with the provided price feed address as a constructor parameter.

5. Log the deployed contract's address to the console.

To deploy the contract, you can run this script using Hardhat's deployment command, such as **`npx hardhat run deploy.js --network celo`**. Ensure that you have the necessary network configurations in the Hardhat configuration file like the RPC URL and the private key of the deployer account.

Note: The code snippet assumes you have a valid Oracle price feed address and that you've replaced the placeholder address **(`0x1234567890123456789012345678901234567890`)** with the actual address of the Oracle price feed.

### Interacting with Your Stablecoin:

Using a variety of wallets and programs that are compatible with Celo, you can now interact with your stablecoin after it has been deployed. To guarantee seamless use, test transactions, transfers and other features.

You may create a strong and dependable stablecoin on the Celo blockchain by following these instructions and utilizing the abilities of Hardhat and Solidity. To give people confidence in the integrity of your stablecoin, don't forget to do extensive testing, establish appropriate security measures and request external audits (if necessary).

## Conclusion:

Therefore, the Celo Dollar (cUSD) stands as an impressive stablecoin built on the Celo blockchain promoting financial accessibility and stability. Understanding its stability mechanism and advantages helps to shed light on its potential impact on the world of decentralized finance (De-Fi). Furthermore, with the guidance provided on writing a Smart Contract using Hardhat and Solidity, you now have the tools to embark on your own stablecoin creation journey on the Celo blockchain.

Harness the power of cUSD and explore the possibilities of stablecoin innovation on the Celo network. By adhering to best practices, conducting thorough testing and building on the robust infrastructure provided by Celo and Hardhat, you can now contribute to the exciting and rapidly evolving world of decentralized finance.
