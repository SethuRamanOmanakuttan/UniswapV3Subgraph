# Uniswap V3 Subgraph

This repository contains a subgraph for Uniswap V3, designed to index data from the Ethereum blockchain, specifically from the Uniswap smart contracts, and make it easily queryable using GraphQL.

## Overview

Uniswap is a decentralized exchange (DEX) on the Ethereum network that handles a vast number of transactions daily. These transactions carry valuable data that can provide insights into token popularity, distribution, price, and the overall market state. The Graph protocol offers a solution to efficiently index and query this data.

## Features

- **The Graph**: An open-source decentralized protocol for querying and indexing data from Ethereum and other decentralized networks using GraphQL.
- **Subgraphs**: These are mappings of blockchain data into an easily understandable format, allowing developers to access and understand the data stored on the blockchain.
- **Chainstack Subgraphs**: An enterprise-grade solution for deploying and managing subgraphs.

## Getting Started

1. **Prerequisites**:
   - Node.js (^v16)
   - A code editor (e.g., VS Code)
   - Install the graph-cli package:
     ```bash
     npm install -g @graphprotocol/graph-cli
     ```

2. **Setting Up**:
   - Initialize a new subgraph project:
     ```bash
     graph init
     ```
   - Follow the prompts to set up the subgraph based on the UniswapV3Factory contract.
   - Modify the `schema.graphql` file to define the data schema.
   - Update the `subgraph.yaml` manifest file.
   - Generate the necessary code:
     ```bash
     graph codegen && graph build
     ```

3. **Deployment**:
   - Deploy the subgraph to a project on The Graph using:
     ```bash
     graph deploy
     ```
   

## Querying

You can query the subgraph using the GraphQL UI or via curl commands. Example queries are provided in the blog to fetch details of liquidity pools and tokens.

## Conclusion

Subgraphs offer a powerful tool for Web3 developers to access blockchain data efficiently. This repository provides a subgraph for Uniswap V3, enabling seamless access to valuable blockchain data and insights.
