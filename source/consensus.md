# Consensus

## Summary
Double-A Chain adopts the APoS consensus mechanism combining PoA+PoS, jointly governed by verification nodes and voters. As a result, it has the characteristics of democracy, efficiency, low transaction cost, low transaction delay and high transaction concurrency.
To become a validator, you need to stake 10 Million of AAC. After the votes of other token holders, each node candidate must have at least 100 users' votes (i.e. 100 voting addresses) to be eligible to become a candidate node. In addition, the node must be ranked between 22 and 32 to become candidate nodes.

## Glossary
Validators are responsible for packaging out blocks for on-chain transactions. There are a total of 21 of them.
Candidates, Stake at least 10 million of AAC， have at least 100 users' votes and are ranked between 22-32.
Epoch, Time interval in blocks, currently 1epoch = 200block on Double-A Chain. At the end of each epoch, the blockchain interacts with the system contracts to update active validators.

## System Contract
The management of the current validators is all done by the system contracts.
Proposal responsible for managing access to validators and managing validator proposals and votes.
Validators are responsible for ranking management of validators, stake and unstake operations, distribution of block rewards, etc.

## Chain calls for System Contract
The contract is called at the end of each block, and fees are distributed to active validators.
The contract is called to update active validators based on the ranking at the end of each epoch.

## Staking
Any user can stake any number of coins to the validator, and the minimum staking amount for each validator is 10 million AACs.
