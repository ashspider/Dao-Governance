# Dao-Governance

Decentralized protocols are in constant evolution from the moment they are publicly released. Often, the initial team retains control of this evolution in the first stages, but eventually delegates it to a community of stakeholders. The process by which this community makes decisions is called on-chain governance, and it has become a central component of decentralized protocols, fueling varied decisions such as parameter tweaking, smart contract upgrades, integrations with other protocols, treasury management, grants, etc.

# About the Project

### Token

The voting power of each account in our governance setup will be determined by an ERC20 token. The token has to implement the ERC20Votes extension. This extension will keep track of historical balances so that voting power is retrieved from past snapshots rather than current balance, which is an important protection that prevents double voting.

### Governor

Initially, we will build a Governor without a timelock. The core logic is given by the Governor contract, but we still need to choose:

1) how voting power is determined
2) how many votes are needed for quorum
3) what options people have when casting a vote and how those votes are counted
4) what type of token should be used to vote

# Technology Stack & Tools

- Solidity (Writing Smart Contract)
- Javascript (React & Testing)
- [Web3](https://web3js.readthedocs.io/en/v1.5.2/) (Blockchain Interaction)
- [Truffle](https://www.trufflesuite.com/docs/truffle/overview) (Development Framework)
- [Ganache](https://www.trufflesuite.com/ganache) (For Local Blockchain)

# Requirements For Initial Setup

- Install [NodeJS](https://nodejs.org/en/), should work with any node version below 16.5.0
- Install [Truffle](https://www.trufflesuite.com/docs/truffle/overview),
- Install truffle run `npm i -g truffle`.
- Install [Ganache](https://www.trufflesuite.com/ganache).

# Setting Up

1. Install Dependencies:
`$ npm install`

2. Start Ganache [Run Ganache-cli]

3. Migrate Smart Contracts
`$ truffle migrate --reset`

4. Run 1st script
`$ truffle exec .\scripts\1_create_proposal.js`

# Graphical Representation

![dao_process](https://user-images.githubusercontent.com/39323954/177732367-a30fb29b-9628-4ad8-a179-168d53cfb72b.jpg)



