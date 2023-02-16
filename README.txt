    The Ethereum blockchain has great decentralization & security properties. These properties come at a price: transaction throughput is low, and transactions can be expensive (search term: blockchain trilemma). This makes many traditional web applications infeasible on a blockchain... or does it?

    🍰 A number of approaches to scaling have been developed, collectively referred to as layer-2s (L2s). Among them is the concept of payment channels, state channels, and state channel networks. This tutorial walks through the creation of a simple state channel application, where users seeking a service lock collateral on-chain with a single transaction, interact with their service provider entirely off-chain, and finalize the interaction with a second on-chain transaction.

    🧑‍🤝‍🧑 State channels really excel as a scaling solution in cases where a fixed set of participants want to exchange value-for-service at high frequency. The canonical example is in file sharing or media streaming: the server exchanges chunks of a file in exchange for micropayments.

Build a Streamer.sol contract that collects ETH from numerous client addresses using a payable fundChannel() function and keeps track of balances.
💵 Exchange paid services off-chain between the Streamer.sol contract owner (the Guru) and rube clients with funded channels. The Guru provides the service in exchange for signed vouchers which can later be redeemed on-chain.

