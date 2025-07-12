# NFT Staking Platform with ERC20 Rewards

This project implements a fully on-chain NFT staking contract where users can stake their ERC721 NFTs and earn ERC20 tokens as rewards over time.

---

## 📋 Features

- ERC721 NFT contract (`MyNFT`) to mint NFTs
- ERC20 token contract (`MyToken`) to distribute as staking rewards
- Staking contract (`Staker`) where users can:
  - Stake NFTs
  - Unstake NFTs
  - Accumulate ERC20 rewards over time
- Reward calculation based on staking duration

---

## 🛠️ Tech Stack

- Solidity
- OpenZeppelin ERC721 & ERC20 libraries
- Remix IDE / Hardhat compatible

---

## 📄 Contracts

| Contract       | Description                            |
|----------------|----------------------------------------|
| `MyNFT.sol`    | ERC721 NFT contract for minting tokens |
| `MyToken.sol`  | ERC20 token used as staking rewards    |
| `Staker.sol`   | Staking contract to stake NFTs & earn rewards |

---

## 🚀 Getting Started

### Deploy & Test with Remix

1️⃣ Open [Remix IDE](https://remix.ethereum.org/)

2️⃣ Clone or download this repository, and upload the `contracts/` folder to Remix.

3️⃣ Compile the contracts:
- In Remix, go to the **Solidity Compiler** tab.
- Select the appropriate Solidity version (check `pragma` in the contracts).
- Click **Compile MyNFT.sol**, `MyToken.sol`, and `Staker.sol`.

4️⃣ Deploy the contracts:
- Deploy `MyToken.sol` and `MyNFT.sol` first.
- Then deploy `Staker.sol`, passing the addresses of `MyToken` and `MyNFT` as constructor arguments.

5️⃣ Interact with the contracts:
- Mint NFTs using `MyNFT`.
- Stake NFTs in the `Staker` contract.
- Earn and claim ERC20 rewards over time.
- Unstake NFTs when desired.

---

## 📜 License

MIT
