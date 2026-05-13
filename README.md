# 🐻🪝 Hooked Bears — Documentation

[![Docs](https://img.shields.io/badge/docs-hookedbears.xyz-orange)](https://hookedbears.xyz)
[![Twitter](https://img.shields.io/badge/X-@hookedbears-black?logo=x)](https://x.com/hookedbears)
[![OpenSea](https://img.shields.io/badge/OpenSea-collection-2081E2?logo=opensea)](https://opensea.io/collection/hookedbears)
[![Chain](https://img.shields.io/badge/chain-Ethereum%20Mainnet-627EEA?logo=ethereum)](https://etherscan.io)
[![License](https://img.shields.io/badge/docs%20license-CC--BY--4.0-blue)](LICENSE)

> **The slop is the art.**

Official documentation for **Hooked Bears** — an experimental on-chain economy of 3,333 pixel-art bears on Ethereum mainnet, plus an ERC-20 token called **$HOOK** and the mechanics that connect them.

You catch bears. You bond two together. You release them into the wild for $HOOK tokens.

Every action is permanent. Every action shapes the population. Every $HOOK in circulation represents a bear that lived, bonded, and was set free.

---

## 📚 What's in this repo

This repository hosts the **public documentation** for the Hooked Bears project. The docs are written in plain Markdown and organized into six sections:

| Section | What's inside |
|---|---|
| **Getting Started** | Wallet setup, how to mint your first bear |
| **Mechanics** | Trap, Pack, Roar, rarity, and a strategy guide |
| **$HOOK Token** | Tokenomics, the trading gate, no-tax design |
| **Smart Contracts** | Architecture, trust signals, contract addresses |
| **FAQ** | Common questions, troubleshooting, glossary |

Browse the rendered version at **[hookedbears.xyz/docs](https://hookedbears.xyz)** or read the Markdown directly here on GitHub.

---

## 🚀 Quick start for readers

**New here?** Start with [What are Hooked Bears?](getting-started/what-are-hooked-bears.md).

**Want to mint?** Read [How to Trap your first bear](getting-started/how-to-trap.md).

**Curious about the mechanics?** Jump to [Trap](mechanics/trap.md) → [Pack](mechanics/pack.md) → [Roar](mechanics/roar.md).

**Tokenomics-focused?** Go to [$HOOK Tokenomics](token/tokenomics.md).

**Developer or researcher?** See [Smart Contract Architecture](contracts/architecture.md) and [Trust Signals](contracts/trust-signals.md).

---

## 🎯 What makes the project different

- **No transfer tax** on $HOOK — the entire tax system was removed from the contract
- **No treasury fee** on Roars — you receive 100% of every payout
- **Trading gate** — $HOOK cannot be minted before legitimate liquidity exists, blocking fake-pool frontrun attacks
- **Forced gameplay loop** — bears must be Packed at least once before they can Roar
- **Tighter rarity** — only 17 Legendary bears in the entire collection (0.5%)

The contracts are deployed on Ethereum mainnet and verified on Etherscan. See [Contract Addresses](contracts/addresses.md) for canonical addresses (published after launch).

---

## 🧭 The four mechanics

```
🪤 TRAP   →   👀 SIGHT   →   🤝 PACK   →   🦁 ROAR
```

1. **TRAP** — Mint a bear for 0.001 ETH (max 10 per wallet)
2. **SIGHT** — At sellout, every bear reveals its species, traits, and rarity score simultaneously
3. **PACK** — Combine two bears: one survives at +1 level, the other is permanently burned (max level 5)
4. **ROAR** — Release a bear (level 1+) into the wild for $HOOK tokens. The bear is destroyed.

NFTs go down. Tokens go up. The supply tells a story.

---

## 🔗 Quick links

| | |
|---|---|
| 🌐 Site | [hookedbears.xyz](https://hookedbears.xyz) |
| 🐻 OpenSea | [opensea.io/collection/hookedbears](https://opensea.io/collection/hookedbears) |
| 🐦 Twitter / X | [@hookedbears](https://x.com/hookedbears) |
| 📜 Etherscan | All four contracts verified — see [addresses](contracts/addresses.md) |

---

## 🛠️ Repository layout

```
.
├── README.md                          ← you are here
├── SUMMARY.md                         ← table of contents (GitBook-style)
├── getting-started/
│   ├── what-are-hooked-bears.md
│   ├── how-to-trap.md
│   └── wallet-setup.md
├── mechanics/
│   ├── trap.md
│   ├── pack.md
│   ├── roar.md
│   ├── rarity-and-sighting.md
│   └── strategy.md
├── token/
│   ├── tokenomics.md
│   ├── trading-gate.md
│   └── no-taxes.md
├── contracts/
│   ├── architecture.md
│   ├── trust-signals.md
│   └── addresses.md
└── faq/
    ├── index.md
    ├── troubleshooting.md
    └── glossary.md
```

---

## 🤝 Contributing

Documentation contributions are warmly welcomed — typo fixes, clarity improvements, translations, new examples, better diagrams.

Read **[CONTRIBUTING.md](CONTRIBUTING.md)** before opening a pull request.

Found a bug, security concern, or factual error? See:

- **General issues** → [open an issue](../../issues/new/choose)
- **Security disclosures** → [SECURITY.md](SECURITY.md) (please do **not** open a public issue for security bugs)

By participating you agree to abide by our **[Code of Conduct](CODE_OF_CONDUCT.md)**.

---

## ⚠️ Important notice

This repository contains **documentation only**. It does not contain:

- Private keys or seed phrases (these never leave a user's wallet)
- Deployer credentials or admin keys
- API keys, RPC keys, or infrastructure secrets
- The Merkle tree (`tree.json`) used to generate rarity proofs at runtime

Smart-contract source is published and verified directly on **Etherscan** — that is the canonical source of truth, not this repository. Always cross-reference contract addresses against the official site, [hookedbears.xyz](https://hookedbears.xyz).

If you see Hooked Bears content published anywhere else with different contract addresses, **it is a scam**. See [Troubleshooting](faq/troubleshooting.md#still-stuck) for how real support behaves (hint: it never DMs first and never asks for your seed phrase).

---

## 📄 License

The documentation in this repository is released under [**CC-BY-4.0**](LICENSE) — you may share and adapt it freely, including commercially, provided you give appropriate credit.

The smart-contract source code is governed by separate license headers in the verified Etherscan source — refer to those for contract licensing.

---

> Made with bait, hooks, and questionable financial decisions. 🐻🪝
