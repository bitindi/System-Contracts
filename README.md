# System contracts

## Overview

The management of the current validators are all done by the system contracts.

- Proposal Responsible for managing access to validators and managing validator proposals and votes.
- Validators Responsible for ranking management of validators, staking and unstaking operations, distribution of block rewards, etc.
- Punish Responsible for punishing operations against active validators who are not working properly.

## Blockchain call system contracts：
At the end of each block, the Validators contract is called and the fees for all transactions in the block are distributed to active validators.
The Punish contract is called to punish the validator when the validator is not working properly.
At the end of each epoch, the Validators contract is called to update active validators, based on the ranking.
