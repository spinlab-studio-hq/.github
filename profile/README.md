# Spinlab Studio

Developer home of **Spinlab Studio** — https://spinlab.studio — a modular white-label platform for online casino operators.

This org is where we'll publish the things developers who integrate with casino back offices keep asking us for: example clients, schemas and small tools. Nothing here is player-facing.

## What developers usually integrate with

| Area | What it is used for |
|---|---|
| Game data API | Real-time round and wager data for **streamer leaderboards**, tournaments and community dashboards |
| CRM / export hooks | Pushing player events (registration, first deposit, bonus claim) into CRM and email tools |
| Wallet events | Deposit / withdrawal status changes across fiat and crypto (BTC, ETH, USDT, USDC, SOL, TRX) |
| Affiliate data | Click, registration and revenue-share attribution for affiliate dashboards |

## Planned repositories

- `leaderboard-example` — a minimal leaderboard service that polls the game data API, aggregates wagers per streamer code and caches results
- `webhook-verifier` — signature verification snippets for incoming wallet and KYC events (Node, Python, Go)
- `reconciliation-sql` — queries for matching game-provider invoices against round-level GGR

## Principles

- **Operator-side only.** Everything here helps operators, affiliates and streamers build tooling; nothing here is gambling content.
- **Compliance first.** Examples assume KYC/AML status is checked before any payout logic runs.
- **Boring is good.** Idempotent webhooks, explicit retries, no hidden magic.

Questions or integration requests: open an issue in the relevant repo.
