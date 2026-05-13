# Changelog

All notable changes to the Hooked Bears documentation will be recorded in this file.

The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and the version numbers refer to **documentation revisions**, not smart-contract versions. Contract changes are versioned separately on-chain (the docs note when a section reflects v3 vs earlier designs).

## [Unreleased]

### Added
- Standard GitHub repository scaffolding (CONTRIBUTING, SECURITY, CODE_OF_CONDUCT, issue templates, PR template, CI workflow, gitignore)

### Notes
- This changelog starts with the public release of the docs repository.
  Earlier internal revisions of the docs are not retroactively cataloged here.

## [1.0.0] — Initial public release

### Added

- `README.md` — project overview and table of contents
- `SUMMARY.md` — GitBook-style navigation

- **Getting Started**
  - `what-are-hooked-bears.md` — the four-mechanic overview, rarity distribution, archetype summary
  - `how-to-trap.md` — step-by-step mint guide
  - `wallet-setup.md` — wallet recommendations and security rules

- **Mechanics**
  - `trap.md` — mint mechanics, Tracking phase, the Sighting
  - `pack.md` — bond mechanics, merge-level math, strategic considerations
  - `roar.md` — release formula, preconditions (level + trading gate), Merkle-proof check
  - `rarity-and-sighting.md` — tier distribution and Merkle-proof verification
  - `strategy.md` — seven archetype play patterns with example math

- **$HOOK Token**
  - `tokenomics.md` — hard cap, premint distribution, supply flow
  - `trading-gate.md` — anti-rug gating mechanism, launch sequence
  - `no-taxes.md` — what was removed from v3 and why

- **Smart Contracts**
  - `architecture.md` — four-contract design (Trap / Hook / Pack / Roar), role plumbing
  - `trust-signals.md` — verifiable read functions per contract
  - `addresses.md` — placeholder addresses (to be filled at launch)

- **FAQ**
  - `index.md` — general, minting, mechanics, token, technical, community
  - `troubleshooting.md` — wallet, revert reasons, indexing, scam-awareness reminders
  - `glossary.md` — terms used across the docs

[Unreleased]: ../../compare/v1.0.0...HEAD
[1.0.0]: ../../releases/tag/v1.0.0
