# Security Policy

We take security seriously across every layer of the Hooked Bears project — smart contracts, the dashboard, and the documentation that explains them.

## 🔭 Scope

This security policy covers:

| Surface | What we care about |
|---|---|
| **Smart contracts** (Trap, HookToken, Pack, Roar) on Ethereum mainnet | Logic bugs, reentrancy, access-control issues, fund loss, denial of service, Merkle-proof bypasses |
| **Dashboard** at hookedbears.xyz | XSS, transaction substitution, wallet-connect issues, RPC injection, leaked secrets |
| **This documentation repository** | Misleading claims that could endanger users (e.g., wrong contract address, false trust signal) |

Out of scope (we appreciate the report but cannot reward or prioritize):

- Issues in third-party wallets (Rabby, MetaMask, etc.)
- Issues in Uniswap V2 itself
- Generic dependency CVEs without a demonstrated impact on Hooked Bears
- Social-engineering attempts against the team (we'll just block & report)
- Browser-extension conflicts (`Cannot redefine property: ethereum` — see [troubleshooting](faq/troubleshooting.md))

## 🛡️ Reporting a vulnerability

**Please do not open a public GitHub issue, public tweet, or Discord post about a security bug before we've had a chance to respond.**

Two ways to reach us privately:

1. **GitHub private vulnerability report** — preferred. Use the **"Report a vulnerability"** button on the [Security tab](../../security/advisories/new) of this repository. This is the most reliable path; only repository maintainers see the report.
2. **DM on X** — [@hookedbears](https://x.com/hookedbears). DMs are open. Lead with **"security disclosure"** so we know not to discuss in public replies. Do not include the technical details in the first message — we'll move to a more private channel.

What to include in the disclosure:

- A clear description of the issue and its impact
- Steps to reproduce (transaction hashes, code snippets, repro URLs)
- Your suggested severity and reasoning
- Whether the issue is already public anywhere
- How you'd like to be credited if/when the fix ships (or "anonymous")

## ⏱️ What happens next

- **Within 72 hours** — we acknowledge receipt and start triage
- **Within 7 days** — we confirm whether we've reproduced the issue and share our preliminary severity
- **Fix window** — varies. Smart-contract bugs that risk user funds get top priority; documentation issues get fixed in the next routine update
- **Disclosure** — we coordinate publication with you. Where possible, we publish a post-mortem within 30 days of the patch

## 🚫 No bug bounty (yet)

We are a solo, pseudonymous, unfunded project. We do **not** have a paid bug bounty at this time. We can offer:

- Public credit (or anonymity, your choice)
- A shout-out from the official X account
- Eternal gratitude

If we do introduce a paid program later, prior-reported issues will be reviewed for retroactive consideration.

We mention this up front so there are no surprises. We'd rather under-promise than over-promise.

## ⚖️ Safe-harbor commitment

If you make a **good-faith effort** to follow this policy, we commit to:

- Not pursuing legal action against you for the research
- Not asking law enforcement to investigate you
- Working with you on coordinated disclosure timing

"Good faith" specifically means:

- ✅ Test against your own bears, on testnet, or with funds you'd be comfortable losing
- ✅ Stop and report as soon as you've proven the issue exists
- ❌ **Do not** drain user funds, manipulate the trading gate, or perform any action that harms other holders, even "for science"
- ❌ **Do not** publicly disclose or use the vulnerability before we've patched it
- ❌ **Do not** attempt social engineering against the team or any third-party services

If a vulnerability **could** drain user funds and you exploit it for more than the minimum needed to prove the issue, you're outside the safe harbor.

## 🎭 Phishing & impersonation

A non-technical but important security category: **scams targeting our users.**

If you spot:

- A fake "Hooked Bears" Twitter account
- A phishing site with a similar URL (e.g., `hook3dbears.xyz`)
- Discord servers pretending to be official support
- "Free $HOOK claim" sites collecting wallet signatures
- Anyone DMing users for "support" pretending to be the team

…please **report it** by replying or DMing [@hookedbears](https://x.com/hookedbears) with screenshots. We can't shut these down, but we can warn the community.

## 📜 Documentation security

The docs themselves can be a security surface. If you find:

- A wrong contract address that could send users to a fake contract
- Instructions that would cause a user to leak their seed phrase or sign a dangerous message
- A code snippet with an obvious vulnerability that someone might copy into production

…treat it as a security disclosure and follow the reporting steps above, not a normal issue.

## 🧭 On-chain truth wins

The verified source code on Etherscan is the **single source of truth** about what the contracts do. The docs are our best-effort explanation of that code. If they disagree, the code wins — please tell us so we can fix the docs.

You can always verify trust signals yourself: see [contracts/trust-signals.md](contracts/trust-signals.md) for the full list of read-only checks anyone can run.

---

Thanks for helping keep Hooked Bears safe. 🐻🪝
