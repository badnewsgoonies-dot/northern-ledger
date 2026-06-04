# The Northern Ledger

An interactive explorer for the financials of the **S&P/TSX Composite** and ~240 TSX-connected filers — where **every figure is traced to the regulatory filing it came from and cryptographically signed**, so the numbers are checkable rather than "trust us."

**Live:** https://badnewsgoonies-dot.github.io/northern-ledger/

## What it does
- Headline financials and interactive multi-year charts for each company
- **Trace any figure** to its source filing, on-chain position, content hash, and ed25519 signature
- **Compare** up to four companies; **rank** the whole market by any metric (FX-normalized to CAD)
- **Restatements** surfaced as signed `current_validity` verdicts (superseded → current)
- A built-in **field guide**: what each metric means, what actually matters, and how the right metrics change by sector (a bank isn't read like a tech company) — plus automatic per-company sector notes and an earnings-quality (cash-vs-profit) flag

## How it's built
A single self-contained HTML file — data, charts, and fonts all inline, no external requests, works offline. It's a read-only projection of a signed, append-only evidence chain (GCOS / Briefcase).

Sources: SEC EDGAR XBRL (interlisted filers), issuer results releases (SEDAR-only names), iShares XIC roster, Bank of Canada FX. **Not investment advice.**
