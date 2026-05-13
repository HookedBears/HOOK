# Contributing to Hooked Bears Docs

Thanks for considering a contribution! This repo is the public documentation for the Hooked Bears project, and improvements from the community are what keep it accurate, clear, and useful.

This is a small, pseudonymous-solo-dev project. Please be patient with response times, and please be kind in your tone — we read every issue and PR personally.

## 🟢 What we welcome

- **Typo and grammar fixes** — open a PR directly, no issue needed
- **Clarity improvements** — confusing paragraphs, ambiguous tables, missing diagrams
- **New examples** — code snippets, command examples, walk-throughs
- **Translations** — open a discussion first so we can coordinate the folder structure
- **Better diagrams** — ASCII art or Mermaid is preferred over external images
- **Factual corrections** — if the docs disagree with what's on-chain, the on-chain truth wins. Open an issue with the discrepancy.
- **FAQ additions** — saw a question come up in the wild more than once? Submit it with an answer.
- **Glossary expansions** — terms you had to look up are terms others will need too.

## 🔴 What we won't merge

- **Promotional content** for unrelated projects, exchanges, or shilled tokens
- **Price predictions, "alpha," or financial advice** — the docs stay mechanical and factual
- **Speculation about future features** — if it isn't shipped, it doesn't belong in the docs
- **Anything attributing words to the deployer that they didn't say** on the official channels
- **Edits that change contract addresses** — those come from the team, never from a PR
- **AI-generated bulk PRs** — we welcome AI-assisted edits, but every PR must be read and understood by a human contributor before submitting

## 📝 How to contribute

### Small change (typo, single sentence)

1. Click the pencil icon on any file in GitHub
2. Make the edit
3. Submit a PR with a descriptive title (e.g., `fix: typo in roar.md formula table`)
4. We'll merge promptly if it's clearly correct

### Larger change (new section, restructure)

1. **Open an issue first** describing what you'd like to change and why
2. Wait for a thumbs-up before investing significant time
3. Fork the repo
4. Make your changes on a feature branch (`docs/your-topic`)
5. Submit a PR referencing the issue (`Closes #123`)

### Translation

We'd love translated docs. The plan is a `translations/<lang-code>/` directory mirroring the English structure (e.g. `translations/es/`, `translations/zh/`). If you want to volunteer, open a discussion and we'll set up the folder.

## ✍️ Style guide

The docs aim for a specific voice: **technical, honest, slightly playful, never hype-y**. A few concrete rules:

- **Prefer plain language** over jargon when both work. If you must use jargon, define it on first use or link to the glossary.
- **Show, don't promise.** "The contract reverts if X" is better than "The team has ensured Y."
- **Use tables** for parameter lists, comparisons, and "what can / cannot happen" sections.
- **Use code blocks** for Solidity, JavaScript, and shell snippets. Specify the language for syntax highlighting.
- **Wrap lines around 100 characters** in prose — don't hard-wrap at 80, and don't write 400-character paragraphs either.
- **Headings use sentence case** (`## Why we removed taxes`), not Title Case.
- **Emoji are fine, sparingly.** They're part of the project's voice. Don't overdo it.
- **Link relatively** to other docs: `[Trading gate](../token/trading-gate.md)`, not absolute URLs.
- **Don't invent numbers.** If you don't have a source, leave it out or mark it as an estimate.

## 🧪 Local preview

The docs are plain Markdown — most editors will render them. If you want a GitBook-style preview locally, any of these work:

```bash
# Option 1: VS Code's built-in preview (Ctrl+Shift+V on any .md file)

# Option 2: serve as a static site
npx serve .

# Option 3: GitBook CLI (matches the production rendering)
npm install -g gitbook-cli
gitbook serve
```

The `SUMMARY.md` file is the table of contents that GitBook reads — if you add a new doc, link it there.

## ✅ PR checklist

Before submitting, please confirm:

- [ ] My change is documentation only (no contract changes, no deployer keys, no production secrets)
- [ ] I've read the file I'm editing end-to-end (not just the section I changed)
- [ ] Internal links still resolve (`./foo.md`, `../section/bar.md`)
- [ ] If I added a new doc, I added it to `SUMMARY.md`
- [ ] My commit messages are descriptive (`docs: clarify pack multiplier table`, not `update`)
- [ ] I'm not promoting an unrelated project
- [ ] If I'm changing factual claims about contracts, I've cross-referenced Etherscan

## 🔒 Security issues

**Do not** open a public issue for security vulnerabilities — in the docs, in the contracts, or in the dashboard. Follow [SECURITY.md](SECURITY.md) for responsible disclosure.

## 💬 Need help?

- General questions → open an [issue](../../issues/new/choose) with the "Question" template
- Real-time discussion → reply to [@hookedbears](https://x.com/hookedbears) on X
- Bug in the live dashboard → [troubleshooting guide](faq/troubleshooting.md) first, then issue

Thanks for making the docs better. 🐻🪝
