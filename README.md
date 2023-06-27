<img src="https://filecoin.io/images/filecoin-logo.svg" width="100">

A curated list of useful resources for Filecoin

## Contents
- [Documentation](#-documentation)
- [Nodes](#-nodes)
- [Libraries and tools](#-libraries-and-tools)
- [Filecoin explorers](#-filecoin-explorers)
- [Wallets](#-wallets)
- [Filecoin Virtual Machine](#-filecoin-virtual-machine)
  * [Tutorials](#-fvm-tutorials)
  * [Libraries and tools](#-fvm-libraries-and-tools)
  * [Documentation](#-fvm-documentation)
  * [Other resources](#-fvm-other-resources)
- [Resources](#resources)
  * [Articles](#-articles)
  * [Videos](#-videos)
  * [Other resources](#-other-resources)


### 📄 Documentation
- [Filecoin website](https://filecoin.io/) - Official Filecoin website
- [What is Filecoin](https://docs.filecoin.io/intro/intro-to-filecoin/what-is-filecoin/) - Official Filecoin intro
- [Filecoin Spec](https://spec.filecoin.io/) - Filecoin specification
- [FIPs](https://github.com/filecoin-project/FIPs) - Filecoin Improvement Proposals
- [Networks](https://docs.filecoin.io/networks/overview/) - Available Filecoin networks
- [Network Upgrades](https://github.com/filecoin-project/core-devs/tree/master/Network%20Upgrades) - Network upgrades (FIPs included, bugfixes, improvements)

### 🌐 Nodes

- [🪷 Lotus](https://github.com/filecoin-project/lotus) - Reference implementation of the Filecoin protocol, written in Go
  - [Lotus docs](https://lotus.filecoin.io/) - Lotus node website, tutorials, knowledge base

- [🌲Forest](https://github.com/ChainSafe/forest) - Implementation of the Filecoin protocol, written in Rust
- [🪐 Venus](https://github.com/filecoin-project/venus) - Implementation of the Filecoin protocol, written in Go

### 🧰 Libraries and Tools
- [Filecoin status](https://status.filecoin.io/) - Filecoin (mainnet, calibnet, butterfly-snapnet) status page
- [built-in actors](https://github.com/filecoin-project/builtin-actors) - On-chain built-in actors code
- [FilSnap](https://github.com/ChainSafe/filsnap) - MetaMask snap for interacting with Filecoin dapps
- [Lily](https://github.com/filecoin-project/lily/) - A wrapped Lotus node designed specifically for indexing the Filecoin blockchain.
- [Lotus Docker images](https://github.com/glifio/filecoin-docker)

### 🧭 Filecoin explorers
- [Filfox](https://filfox.info/)
- [Beryx Explorer](https://beryx.zondax.ch/)
- [Starboard FVM explorer](https://fvm.starboard.ventures/)
- [Filscan](https://filscan.io/)
- [dev.storage explorer](https://dev.storage/)
- [Glif Explorer](https://explorer.glif.io/)

### 👛 Wallets
- [Brave Wallet](https://brave.com/wallet/)
- [GLIF Wallet](https://wallet.glif.io/)

## FVM(Filecoin Virtual Machine)

📢 **[FVM cheatsheet](./fvm.md)** - everything you need to know about FVM.

### 📄 Introduction

- [FVM Docs](https://docs.filecoin.io/fvm) - where to get start learning about FVM.
- [What is FEVM](https://docs.filecoin.io/smart-contracts/fundamentals/filecoin-evm-runtime/) - welcome EVM hacker, here's what allows you to build on Filecoin.
- [Quickstart with Remix](https://docs.filecoin.io/developers/smart-contracts/quickstart/) - Tutorial on deploying your first FEVM actor.

### 🏫 FVM starter kits

- [FEVM Hardhat Kit](https://github.com/filecoin-project/FEVM-Hardhat-Kit) - A starter hardhat project for developing, deploying, and testing Solidity actors on the FEVM.
- [FEVM Foundry Kit](https://github.com/filecoin-project/fevm-foundry-kit) - A starter foundry project for developing, deploying, and testing Solidity smart contracts on the FEVM.
- [FVM Deal Making starter kit](https://github.com/filecoin-project/fvm-starter-kit-deal-making) - use the client contract here to make a deal proposal directly with the Storage Provider for data >4GB.
- [DataDao starter kit](https://github.com/filecoin-project/fevm-data-dao-kit) - quickly spin up a DataDAO using client contract & OpenZepplin's  Dao contracts.

### 🧰 FVM Libraries and Tools

- [Filecoin.solidity](https://docs.zondax.ch/fevm/filecoin-solidity/) - Solidity library for FEVM development to call methods on system/built-in actors on Filecoin.
- [ref-fvm](https://github.com/filecoin-project/ref-fvm) - Reference Filecoin VM implementation
- [fvm-rs-sdk](https://github.com/polyphene/fvm-rs-sdk) - FVM Rust SDK for building actors
- [FVM AssemblyScript SDK](https://github.com/Zondax/fvm-as-sdk)
- [FVM Go SDK](https://github.com/ipfs-force-community/go-fvm-sdk)

### 🦝 FVM Other resources

- [FVM Conceptual Overview](https://hackernoon.com/the-filecoin-virtual-machine-everything-you-need-to-know)
- [FVM resources list from Protocol Labs](https://www.notion.so/Filecoin-Virtual-Machine-FVM-Developer-Resources-94cabfd650184f4b9664bd4974e4d329)
- [EVM to FVM Address Management (F4 Addressing)](https://drive.google.com/file/d/17ngqxflu9B-gBqVl--5KqVhXsTLhkWtJ/view)
- [FEVM Technical Overview presentation](https://www.youtube.com/watch?v=ybR9sYlKkOs)

## Resources

### 📰 Articles
- [How storage and retrieval deals work on Filecoin](https://filecoin.io/blog/posts/how-storage-and-retrieval-deals-work-on-filecoin/)

### 📹 Videos
- [Filecoin Foundation YouTube channel](https://www.youtube.com/@filecoinfoundation) - Talks from Filecoin conferences/events
- [Filecoin Project YouTube channel](https://www.youtube.com/@filecoinfoundation) - Talks/recordings from the Filecoin ecosystem
- [How Filecoin Actors Work](https://www.youtube.com/watch?v=9JbwbTPonv0) - Deep dive into the actors by [zenground0](https://github.com/ZenGround0)
- [The EVM-compatibility of FVM aka FEVM](https://www.youtube.com/watch?v=lgUMVhM3FIM)

### 🦝 Other resources
- [Launchpad Curriculum](https://curriculum.pl-launchpad.io/) - PL Launchpad bootcamp resources

