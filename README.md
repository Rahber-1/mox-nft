# 🐶 Puppy NFT & 😄 Mood NFT

A collection of NFT smart contracts written in **Vyper**, utilizing the [Snekmate](https://github.com/Boa-Network/snekmate) modular framework. The project includes:

- 🐶 **Puppy NFT**: A simple ERC721 contract that mints NFTs with IPFS-based URIs.
- 😄 **Mood NFT**: A dynamic on-chain NFT that changes its mood (Happy/Sad) and stores SVGs directly on-chain.

---

## 📦 Features

### 🐶 Puppy NFT
- ERC721 compliant
- Mint NFTs with IPFS URIs
- Basic contract structure using Snekmate modules

### 😄 Mood NFT
- On-chain SVG storage (Happy & Sad moods)
- Dynamic `tokenURI()` generation using base64-encoded metadata
- `flip_mood()` function allows owner to toggle mood of the NFT
- Fully on-chain metadata and images (no IPFS needed)

---

# 📁 Folder Structure
```
├── contracts/
│ ├── puppy_nft.vy
│ └── mood_nft.vy
├── scripts/
│ ├── deploy_basic_nft.py
│ └── deploy_mood_nft.py
├── images/
│ └── dynamic/
│ ├── happy.svg
│ └── sad.svg
├── README.md
├──moccasin.toml
├──pyproject.toml
```


---

## 🚀 Deploy & Mint (using Python + Moccasin)

1. Install dependencies:
   ```bash
   pip install moccasin
python scripts/deploy_basic_nft.py
python scripts/deploy_mood_nft.py

🛠️ Technologies Used
Vyper — Smart contract language

Snekmate — Modular Vyper components

Boa — Python-based Vyper development toolchain

Moccasin — Dev environment for Vyper

IPFS — For Puppy NFT metadata

Base64 — For encoding on-chain metadata

👨‍💻 Author
Rahbar Ahmed
License: MIT
