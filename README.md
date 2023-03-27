# staking-contract

Staking and reward contracts are popular mechanisms for incentivizing participation in the activities of a blockchain network. Users can use these contracts to lock up their tokens as collateral in order to participate in network validation and earn rewards. In this article, we will look at how to use the Solidity programming language to create a staking and reward contract.


# Demo

1. Clone repo

```bash
git clone https://github.com/iamoracle/staking-contract.git
```

2. Install Dependencies

```bash
npm install
```


3. Set environment variables

Copy [./.env_sample](.env_sample) file and rename to `.env` and substitute the environment variables with real values.


4. Compile Contract

```bash
npx hardhat compile
```

5. Deploy Contract

```bash
npx hardhat run ./scripts/deploy.ts
```

6. Run test

```bash
npx hardhat test
```


## Known Issues


* Contract not fit for production.
* You need to transfer the reward to the deployed contract else, users will not be able to claim reward.
* You might not be able to unstake, if other users have unstaked e.g used your funds as a reward while the reward pool is empty.
* No start and stop mechanism.