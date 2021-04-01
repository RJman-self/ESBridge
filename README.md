# Platdot

English | [简体中文](./docs/README_CN.md)

​![build](https://img.shields.io/badge/build-passing-{})    ![test](https://img.shields.io/badge/test-passing-{})   ![release](https://img.shields.io/badge/release-v1.0.0-E6007A)

![Platdot-overview](https://cdn.jsdelivr.net/gh/rjman-self/resources/assets/20210401155745.png)

## A cross-chain Bridge

`Platdot` is based on [ChainBridge](https://github.com/ChainSafe/ChainBridge) a cross-chain project developed by ),
it provides `Polkadot` cross-chain bridge for `Platon` to achieve the functions of PDOT **issuance**, **redemption** and **transfer**. Currently, Platdot supports cross-chain transfer of assets between EVM and substrate chains that support multiSign-pallet, such as polkadot / kusama. EVM's smart contract, as one end of the bridge, allows custom processing behavior when the transaction is received. For example, locking DOT assets on the polkadot network and executing contracts on EVM can mint and issue PDOT assets, similarly, executing contracts on EVM can destroy PDOT assets and redeem DOT assets from Polkadot's multi-signature address. Platodt currently operates under a trusted federation model, and users can complete mortgage issuance and redemption operations at a very low handling fee.

## Installation

### Dependencies

+ Make sure the Golang environment is installed

+ [Platdot-contract v1.0.0](https://github.com/ChainSafe/chainbridge-solidity): Deploy and configure smart contract in Alaya.

### Building

`git clone https://github.com/RJman-self/Platdot.git`

`make build`: Builds `platdot` in `./build`.

**or**

`make install`: Uses `go install` to add `platdot` to your `GOBIN`.

## Getting Start

Documentations are now moved to `GitHub Wiki`.

### RunningLocally

[Deploy Smart Contracts](https://github.com/RJman-self/Platdot/wiki/Deploy-smart-contracts-to-the-alaya-network)

[Start A Relayer](https://github.com/RJman-self/Platdot/wiki/Start-A-Relayer)

## License

The project is released under the terms of the `GPLv3`.
