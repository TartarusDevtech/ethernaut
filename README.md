# Ethernaut MMO Naut

Ethernaut MMO Naut is a Web3/Solidity-based wargame, designed to be played in the Ethereum Virtual Machine. Each level is a smart contract that needs to be 'hacked'—challenging players to solve security puzzles and exploit vulnerabilities, all while learning about Ethereum and smart contract development.

The game acts both as an educational tool for those interested in learning Ethereum/Solidity security and as a living catalogue of historical hacks, modeled as levels. There can be an infinite number of levels, and the game does not require them to be played in any particular order.

## Features

- **Interactive Smart Contract Levels:** Solve security puzzles by hacking smart contracts.
- **Educational Content:** Each level focuses on real-world vulnerabilities and concepts such as storage, parameter parsing, delegatecall, proxies, and more.
- **Open-ended Progression:** Play and solve levels in any order.
- **Community Contributions:** The game is open to new levels and improvements from the community.
- **Multi-language Support:** Play the game in several languages.

## Deployed Version

You can play the current, official version at: [ethernaut.openzeppelin.com](https://ethernaut.openzeppelin.com)

## Getting Started

### Prerequisites

- Node.js (use `nvm use` at the root to select a compatible version)
- Yarn package manager

### Installation

1. Clone the repository and install dependencies:
    ```bash
    git clone git@github.com:TartarusDevtech/ether-mmo-naut.git
    yarn install
    ```

2. Start a local test Ethereum network (e.g., using Ganache, Hardhat, or Geth).

    ```bash
    yarn network
    ```

3. Deploy contracts to your local network:

    ```bash
    yarn deploy:contracts
    ```

4. Run the client/frontend (React app):

    ```bash
    yarn start
    ```

The app will be available on [localhost:3000](http://localhost:3000).

### Deploying to Goerli Testnet

- Set the `ACTIVE_NETWORK` variable in `constants.js`.
- Edit `deploy.goerli.json` to manage contract and level instances.
- Deploy with:
    ```bash
    yarn deploy:contracts
    ```

## Contributing

Contributions are welcome! Please check the [issues](https://github.com/TartarusDevtech/ether-mmo-naut/issues) and feel free to submit pull requests for new levels, bug fixes, documentation, or features.

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Acknowledgements

- Inspired by [OverTheWire](https://overthewire.org) and [OpenZeppelin Ethernaut](https://ethernaut.openzeppelin.com)
- Built with [React](https://reactjs.org/), [Solidity](https://soliditylang.org/), and [EVM](https://ethereum.org/en/developers/docs/evm/)
