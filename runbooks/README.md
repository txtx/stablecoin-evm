# Circle's Stablecoin EVM Runbooks

[![Txtx](https://img.shields.io/badge/Operated%20with-Txtx-gree?labelColor=gray)](https://txtx.sh)

## Available Runbooks

`txtx` Runbooks are the perfect companion to Foundry + Hardhat when creating
Solidity smart contracts. Foundry + Hardhat shine in making the development
process a breeze; `txtx` makes deploying and operating on your contracts secure,
simple, and reproducible.

The following Runbooks are available for this project.

### Deploy Fiat Token V2_2 Contract

This Runbook deploys the `FiatToken_V2_2` and or the `FiatTokenCelloV2_2`
contract, depending on the selected environment.

The following table summarizes the possible environments and their impact:

| Env            | Impact                                                                                                                                                         |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `fiat-devnet`  | Deploys & initializes the `FiatTokenV2_2` contract on a local devnet.                                                                                          |
| `fiat-mainnet` | Initializes the `FiatTokenV2_2` contract on mainnet Expects the contract to already be deployed, and for the env variables to supply the contract address.     |
| `celo-devnet`  | Deploys & initializes the `FiatTokenCeloV2_2` contract on a local devnet.                                                                                      |
| `celo-mainnet` | Initializes the `FiatTokenCeloV2_2` contract on mainnet Expects the contract to already be deployed, and for the env variables to supply the contract address. |

To execute, run:

```console
txtx run deploy -u --env <env>
```

## Getting Started

This repository is using [txtx](https://txtx.sh) for handling its on-chain
operations.

`txtx` takes its inspiration from a battle tested devops best practice named
`infrastructure as code`, that have transformed cloud architectures.

### Installation

#### macOS

```console
brew tap txtx/txtx
brew install txtx
```

#### Linux

```console
sudo snap install txtx
```

### List runbooks available in this repository

```console
$ txtx ls
ID                                      Name                                    Description
deploy                                  deploy                                  Deploys the Fiat Token or Fiat Token Celo contracts. Use environment CLI args to specify the network + contracts to deploy.
```

### Scaffold a new runbook

```console
$ txtx new
```

Access tutorials and documentation at [docs.txtx.sh](https://docs.txtx.sh) to
understand the syntax and discover the powerful features of txtx.

Additionally, the
[Visual Studio Code extension](https://marketplace.visualstudio.com/items?itemName=txtx.txtx)
will make writing runbooks easier.

### Execute an existing runbook

```console
$ txtx run <runbook-id>
```
