<img src="https://bafybeiesyiylnbxe5lrim35mwcwckoipn6eg32kpn6nibfdgb4vkmvzsta.ipfs.w3s.link/FVM%20logo.png" style="zoom:33%;" >

Hi there builders! Not sure where to begin? Too many docs to navigate? 

**Here’s a cheat sheet to get you from zero to hero**. This cheat sheet provides a guide to the following, in order:

💡 Filecoin & FVM concepts
📍 Navigate what you need to use for your hackathon project
🚀 Resources to get you building

## Filecoin Virtual Machine
- [Filecoin 101](https://docs.filecoin.io/about/basics/introduction/) - you know nothing BUT that's okay, this will help!
- [The EVM-compatible FVM](https://docs.filecoin.io/smart-contracts/fundamentals/filecoin-evm-runtime/) - welcome EVM hacker, here's what allows you to build on Filecoin.

#### FVM Developer Basics

- [FVM Docs](https://docs.filecoin.io/smart-contracts/fundamentals/the-filecoin-virtual-machine/): Quickstarts & concepts.
- [EVM vs EVM-compatible FVM (FEVM)](https://docs.filecoin.io/smart-contracts/filecoin-evm-runtime/differences-with-ethereum/): Differences to note.
- [Filecoin address types](https://docs.filecoin.io/basics/the-blockchain/addresses/) - To learn 4 different Filecoin address types, especially EVM-compatible type - **f410**xxx.
- [ERC20 quickstart with Remix](https://docs.filecoin.io/smart-contracts/fundamentals/erc-20-quickstart/) Tutorial FROM SCRATCH: Deploy your first FEVM actor (smart contract equivalent). 
- [Filecoin.solidity](https://docs.zondax.ch/fevm/filecoin-solidity/): Solidity library for FEVM development to call methods on system/built-in actors on Filecoin. 
  - Please ensure you’re using the latest [release](https://github.com/Zondax/filecoin-solidity/releases/tag/v4.0.1) v4.0.1. 
  - To learn how to use Filecoin.sol check out the FEVM Hardhat Starter Kit's Filecoin API contract examples [here](https://github.com/filecoin-project/fevm-hardhat-kit/blob/main/contracts/filecoin-api-examples/FilecoinMarketConsumer.sol). 
  - If you’re curious about the methods of built-in actors and what they can do, you can see [here](https://docs.filecoin.io/reference/json-rpc/introduction/).

####  FVM Project Ideas & Blueprints

- [Data + FVM](https://pl-strflt.notion.site/Data-FVM-234b7f4c17624cd8b972f92806732ca9?pvs=4) See how we are thinking about new concepts on Programmable Storage Markets, including dataDAOs and decentralized data aggregators
- [Request for Startups](https://rfs.fvm.dev/) L2 solution ideas built on top of FVM & FVM tooling ideas. These are some ideas that Filecoin finds valuable to the ecosystem, but is not a finite list.

#### FVM starter kits

- [FEVM Hardhat Kit](https://github.com/filecoin-project/FEVM-Hardhat-Kit) - A starter hardhat project for developing, deploying, and testing Solidity actors on the FEVM.
- [FEVM Foundry Kit](https://github.com/filecoin-project/fevm-foundry-kit) - A starter foundry project for developing, deploying, and testing Solidity smart contracts on the FEVM.
- [FVM Deal Making starter kit](https://github.com/filecoin-project/fvm-starter-kit-deal-making) - use the client contract here to make a deal proposal directly with the Storage Provider for data >4GB.
- [DataDao starter kit](https://github.com/filecoin-project/fevm-data-dao-kit) - quickly spin up a DataDAO using client contract & OpenZepplin's  Dao contracts.

#### How-to

- [Transfer FIL between different address types](https://docs.filecoin.io/basics/assets/transfer-fil/) - learn how to send FIL to ETH compatible address.
- [Convert different Filecoin addresses](https://github.com/filecoin-project/community/discussions/650) - how to convert from f410 to 0x, or ID address to 0x.
- [Send FIL to my Filecoin ID address using MetaMask](https://github.com/filecoin-project/community/discussions/649)
- [Verify your smart contracts](https://docs.filecoin.io/smart-contracts/developing-contracts/verify-contracts/)

#### Navigate to what you need

Filecoin? FVM? IPFS? What should I use to store data for my projects.? 

We got you. Follow the decision-making guide below, to see which resource is recommended for your use case: 
<img width="1296" alt="7" src="https://github.com/filecoin-project/community/assets/113331491/61f74083-396a-447c-977c-266b2da110d4">

**Recommended resources from guide above**

1. **Deal aggregation:** this allows you to store smaller pieces of data (<4GB) to Filecoin that aggregators can pick up and form a larger deal (data sizes <4GB are too small for Storage Providers to pick up directly and you might not get your deal made)
   - with Filecoin Data Tools (FDT), use this [daemon contract](https://github.com/hammertoe/fdt-deal-monitor/blob/main/fdt-deal-monitor-ethers.js) to trigger a deal aggregation workflow with [Filecoin Data Tools' Edge-UR tool](https://github.com/application-research/edge-ur/blob/car-gen/docs/aggregation.md). 
   - with [Lighthouse.storage](https://www.lighthouse.storage/documentation) 
2. **[Deal Making Starter Kit](https://github.com/filecoin-project/fvm-starter-kit-deal-making) (Direct deal making with Storage Providers with):** use the Client Contract here to make a deal proposal, directly with the Storage Provider, for data >4GB.
3. **[HackFS 2023 FVM Starter Ideas](https://ecosystem-wg.notion.site/7d70e8503de64050b765b1fde8dca4d8?v=ad0e8b62ef51486598750abd1195a49b)**: detailed description for solutions and tools to build with and/or to support programmatic storage.
4. **[DataDAO Starter Kit](https://github.com/filecoin-project/fevm-data-dao-kit):** uses Client Contract for storage and Open Zepplin's Governor contract to quickly spin up a dataDAO. Keep building from there!
5. **[Storage Onramps](https://docs.filecoin.io/basics/how-storage-works/storage-onramps/):** easy API integration for non-programmatic storage in your dApp.

#### More FVM-compatible tools

- **Blockchain explorer support FVM**
  
  Check smart contracts, invocation txs & logs, and verify contracts, etc.
  
  - [Filfox](https://filfox.info/)
  - [Beryx Explorer](https://beryx.zondax.ch/)
  - [Starboard FVM explorer](https://fvm.starboard.ventures/)
  
- **Network analytics APIs**
  
  - [Zondax Beryx API](https://docs.zondax.ch/Beryx): Open API for indexing Filecoin. There is a Beryx client for JS
  - [Spacescope API](https://spacescope.io/): Protocol-generated APIs for indexing Filecoin
  - [Storage Provider FilRep reputation system API](https://filrep.io/api): query storage provider reputations. FilRep is not FEVM-compatible yet but is a useful resource to reference for reputation systems
  
- **Decentralized compute**
  - [Bacalhau with FVM](https://github.com/bacalhau-project/lilypad)
  - [Shale Protocol](https://docs.shaleprotocol.com/) Shale-Serve API is a production-ready inference API for open-source LLMs (large language models). It currently supports [Vicuna-13b](https://lmsys.org/blog/2023-03-30-vicuna/). It can be used as a drop-in replacement for the OpenAI API (specifically GPT3.5-turbo) in any language, including Python, cURL, and HTTP requests.
  
- **Access control**
  
  - [Medusa access control APIs](https://documentation-medusa.vercel.app/): Simple programmatic access control without keys
  - [Lighthouse Kavach access control SDK](https://github.com/lighthouse-web3/encryption-sdk): Access control encryption SDK to build trustless applications using distributed key shards with threshold cryptography
  
- **DeFi**
  
  - [wFIL](https://github.com/glifio/wfil) - wrapped FIL for DeFi scenarios like bridging assets, AMM, token swap, etc.
  - [Magmo Nitro State Channels for payment](http://docs.statechannels.org/): ultra-low cost, near-zero-latency conditional transfer of cryptoassets via a "layer 2" network that sits above the blockchain
  - [BANYAN interface for SushiSwap](https://github.com/banyancomputer/figswap-interface): DEX template, need to configure to point to hyperspace instead of wallaby
  
- **Oracles**
  - [Tellor oracle](https://gist.github.com/trruckerfling/b304f1de5901c16867822cd2b9c086da): list of testnet contract addresses
  
- **FVM smart contract templates**
  - [Cookbook.dev](https://www.cookbook.dev/filecoin)
  
- **Naming Service**
  - [Spheron's Filecoin Naming Service SDK](https://www.npmjs.com/package/@spheron/fnslib)
  - [FNS.Space](https://fns.space/) 
  
- **Gaming**
  - [LYNC](https://lync.gitbook.io/lync/fevm-support) Integrate FVM into any game and enable features such as dynamic NFTs and more

## FAQs

**How can I use FVM to store data to Filecoin? / How can I store data with FVM?** 

The intent of FEVM/FVM is to compute over state data (the metadata of your stored data). Storage Providers are the ones that are able to store your data and upload the deal to the Filecoin network. You can check out the [deal flow here,](https://docs.filecoin.io/get-started/store-and-retrieve/store-data/) where various steps can benefit from integrating FEVM! Data retrieval happens via Retrieval Providers, accepting the client's ask to retrieve and working with Storage Providers to decrypt the data to deliver to the client. FEVM/FVM is able to build logic around these 2 processes and automate, add verification and proofs, time-lock retrievals etc.

- **Awesome! But what specifically can I do today to automate filecoin storage deals on FVM?** 

  As of today, we allow you to create deal bounties to incentivize the storage of data through FEVM. [Read more here](https://github.com/lotus-web3/deal-bounty-contract) (this repo is specifically tracks the creation of deal bounties to build a DataDAO; the same pattern applies for any other dapps that need to incentivize the creation of data deals). This means that you need to incentivize the storage of the deal off-chain, and then a user of your dapp can claim the rewards on-chain. We recommend this approach for the hackathon. In the future, we aim to allow you to do this in a few different ways, which will make an exciting landscape to incentivize the storage of deals.

**When a storage deal is made, is the data only stored by a single storage provider? What would happen if the storage provider (for some reason) removed all the data, would it be recoverable or is it lost completely?** 

When a SP stores your data and the deal is active, over time, the SP has to provide Proof of Replication (porep) of the stored data. They also have to provide Proofs of Spacetime (PoST), where randomly selected SPs have to provide PoReps for randomly selected storage sectors they maintain. So your data is replicated and not easily lost. and SPs get slashed if they are unable to provide the proofs so they are not incentivized to delete your data. However, let's say a miner does delete your data for some reason, then to prevent against that, the individual client can choose to store with various SPs. Or you can upload your data via storage helpers like web3storage and estuary, who do the replication across various SPs for you. more reading https://filecoin.io/blog/posts/filecoin-features-verifiable-storage/ https://docs.filecoin.io/developers/storage-helpers/overview/

**How do I close a storage deal on Filecoin and stop Storage Providers from storing my data on-chain?** 

How can I manipulate storage deals? It’s not impossible but SPs are incentivized not to close the storage deal as they are slashed for not providing [Proof of Spacetime (PoST)](https://spec.filecoin.io/algorithms/pos/). Someone has to pay for the broken promise a miner makes to the chain and you need a custom market actor for it most likely to make the deal. You need to make deals for a certain amount of time - right now the boundaries are 6-18 months. You cannot ask a storage provider to take down your data without contacting them off-chain.

**What’s the benefit of deploying EVM to FVM/Filecoin instead of Ethereum network? Or write a dApp that way?** 

What are the unique features of Filecoin as compared to Ethereum? Need narrative/article on why Eth devs should care about FVM, covering gas expectations, performance, dApp benefits. Our current answer is around using FVM for storage-heavy parts of the dApp (at exabibyte level) which might not be priority for most devs.

**Do I have to install Lotus to work with FVM? How do I install it? How do I install it on Hyperspace?** 

Here is a public lotus node you can use https://api.hyperspace.node.glif.io/rpc/v0 

**How do I check SP’s balance with their FEVM address?** 

You can query balance of any address[ https://docs.zondax.ch/openapi#get-/account/balance/-address-](https://docs.zondax.ch/openapi#get-/account/balance/-address-) 

**Who is the beneficiary role, in the deal flow process?** 

The beneficiary role takes on the financial control from the Storage Provider, who then focuses on node control. The node owner, who is the SP, has overarching control over both roles. See more [here](https://github.com/filecoin-project/FIPs/blob/master/FIPS/fip-0029.md).

**How do I control access or encrypt data before storing on Filecoin?** 

You can check out lighthouse.storage. They are an FVM Early Builder who has built an access control SDK https://github.com/lighthouse-web3/encryption-sdk   

**For the frontend, what's a recommended framework(s) to use?**

Most frontend that works for EVM works for FEVM too including Flutter, Dart, Ethers.js, web.js, ReactJs. These can also query events on the frontend.

**How is the Filecoin network accessed through Solidity?** 

We have a feature-complete Ethereum JSON-RPC API that enables EVM tooling to deploy seamlessly to Filecoin. This is a good talk to learn more about the various architectural considerations and features https://youtu.be/TD-LsOpFeMU?t=6665 

**Could someone tell me the characteristics of fvm robust addresses and f4 addresses?** 

https://docs.filecoin.io/developers/smart-contracts/concepts/accounts-and-assets/ 

**Can someone explain what the t0 and t1 addresses are?** 

- 0 - ID Address
- 1 - SECP256K1 Public Key Address
- 2 - Actor Address
- 3 - BLS Public Key Address
- 4 - F4 translated address from foreign runtime to Filecoin

**I am still trying to understand the built-in actors.**

https://docs.filecoin.io/developers/smart-contracts/concepts/actors-and-contracts/ 

**Where can I see other projects built on FEVM?**

- [Filecoin Ecosystem Dashboard (with FVM filter)](https://ecosystem.filecoin.io/?filters=enabled&tags=FVM) - these showcase our early builders and is still being updated through next week
- [ETHGlobal HackFEVM Finalists](https://ethglobal.com/talks/hack-fevm-winners-announced-ads0q) - we ran a FEVM-focused smaller hackathon in Nov 2022, before the latest release of FEVM.