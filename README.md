# Designing a Smart Contract Platform

There are many interesting and difficult problems to solve in designing a blockchain-based smart contract platform. Most of the available documentation about how these platforms work focusses on the specifics of a particular platform e.g. Ethereum / NEO / Stratis. This repository aims to accumulate important writings about smart contract platforms generally, to better inform developers should they want to learn more or even start working on a new approach themselves.

The information here is mostly low-level and technical, and where possible blockchain-agnostic. It is as much as possible detached from the best practices and development of particular smart contracts or smart contract languages themselves.

Everything here is written as if the reader has a rudimentary understanding of how blockchains work, especially with regards to hashing and merkle roots.

# Contract State

By their nature smart contracts store information on-chain. This includes contract code and data saved during execution, as well as possibly balances, UTXO sets etc. depending on the implementation. With the execution of contracts every block, the global state of the network will hence be updated and nodes all need to be able to agree that they have reached the same state following execution of the same block. Furthermore, nodes may need to rollback to a previous global state during a block reorganisation if a longer chain is discovered.

A particular data structure, the Patricia Trie, has some really valuable properties to help achieve this. It can roughly be thought of as a means of retrieving a Merkle Root for contract state.

https://github.com/ethereum/wiki/wiki/Patricia-Tree

# Contract Execution and Determinism

# Contract Fees and 'Gas'

# External Data and Oracles

https://blog.ethereum.org/2014/07/22/ethereum-and-oracles/

# Origin of Smart Contracts
