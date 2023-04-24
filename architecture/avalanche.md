# Avalanche

[Avalanche](https://docs.avax.network/overview/getting-started/avalanche-platform) is a heterogeneous network of blockchains. Unlike homogeneous networks, where all applications reside in the same chain, heterogeneous networks allow separate chains to be created for different applications.

DRT runs on a public C-Chain. A P-Chain version is on the roadmap.

The Primary Network is a special [Subnet](https://docs.avax.network/subnets) containing all validators (including any custom Subnets). A node can become a validator for the Primary Network by staking at least 2,000 AVAX.

![Primary network](https://docs.avax.network/assets/images/primary-network-71c0c060a5ad7654635f8ff8110e272e.png)

All validators as members of the Primary Network are required to validate and secure the following three blockchains: the [**Exchange Chain (X-Chain)**](https://docs.avax.network/overview/getting-started/avalanche-platform#exchange-chain-x-chain), the [**Platform Chain (P-Chain)**](https://docs.avax.network/overview/getting-started/avalanche-platform#platform-chain-p-chain), and the [**Contract Chain (C-Chain**)](https://docs.avax.network/overview/getting-started/avalanche-platform#contract-chain-c-chain).

### Contract Chain (C-Chain)[​](https://docs.avax.network/overview/getting-started/avalanche-platform#contract-chain-c-chain) <a href="#contract-chain-c-chain" id="contract-chain-c-chain"></a>

The **C-Chain** is an implementation of the Ethereum Virtual Machine (EVM). The [C-Chain’s API](https://docs.avax.network/apis/avalanchego/apis/c-chain) supports Geth's API and the creation and execution of smart contracts in Solidity.

The C-Chain is an instance of the Coreth Virtual Machine.

### Platform Chain (P-Chain)[​](https://docs.avax.network/overview/getting-started/avalanche-platform#platform-chain-p-chain) <a href="#platform-chain-p-chain" id="platform-chain-p-chain"></a>

The **P-Chain** is responsible for all validator and Subnet-level operations. The [P-Chain API](https://docs.avax.network/apis/avalanchego/apis/p-chain) supports the creation of new blockchains and Subnets, adding validators to Subnets, staking operations, and other platform-level operations.

The P-Chain is an instance of the Platform Virtual Machine.

### Exchange Chain (X-Chain)[​](https://docs.avax.network/overview/getting-started/avalanche-platform#exchange-chain-x-chain) <a href="#exchange-chain-x-chain" id="exchange-chain-x-chain"></a>

The **X-Chain** is responsible for operations on digital smart assets, Avalanche **Native Tokens**. A smart asset represents a real-world resource (for example, equity or a bond) with rules that govern its behaviour, like "can’t be traded until tomorrow." The [X-Chain API](https://docs.avax.network/apis/avalanchego/apis/x-chain) supports the creation and trade of Avalanche Native Tokens.

One asset traded on the X-Chain is AVAX. When you issue a transaction to a blockchain on Avalanche, you pay a fee denominated in AVAX.

The X-Chain is an instance of the Avalanche Virtual Machine (AVM).
