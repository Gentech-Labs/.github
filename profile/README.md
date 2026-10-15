# GenTech Labs

**Agent infrastructure that holds up under money.** Payments, identity, custody and verification for autonomous agents.

One install gives any agent payment rails, DeFi intelligence, agent identity, a self-evolution harness and an MCP server:

```bash
uvx --from git+https://github.com/Gentech-Labs/genTech-agent-kit.git gentech-kit
```

---

## What's here

| Repo | What it is |
|------|------------|
| **[genTech-agent-kit](https://github.com/Gentech-Labs/genTech-agent-kit)** | One install, full stack — payment rails (x402 / Q402), DeFi intelligence, agent identity (ERC-8004), self-evolution harness, MCP server |
| **[genTech-agent-skills](https://github.com/Gentech-Labs/genTech-agent-skills)** | 175 agent skills — payments, DeFi, context management, handoff mesh, self-evolution. Installable into any profile |
| **[programmable-money-x402](https://github.com/Gentech-Labs/programmable-money-x402)** | x402 payment gateway on Arc — pay-per-call APIs with spend policies and on-chain settlement |
| **[solana-agent-security](https://github.com/Gentech-Labs/solana-agent-security)** | Drain detection and transaction risk analysis for agents that hold keys |
| **[mantle-turing-test](https://github.com/Gentech-Labs/mantle-turing-test)** | Agentic wallet economy — autonomous agents that hold, size and settle capital on-chain |
| **[midnight-confidential-agent-payments](https://github.com/Gentech-Labs/midnight-confidential-agent-payments)** | Confidential payments for agents — what a payment rail looks like when the amount is private |

---

## The part most agent stacks skip

Most agent tooling stops at *connect an app and call a tool*. GenTech builds the layer underneath — the one that decides whether a payment was authorised, whether the trade actually happened, and what happens when a key is lost.

**Custody is a design problem, not a config value.**
Two-of-three threshold authority, bounded and expiring session keys, key material under 3-2-1-0, never a passphrase beside its ciphertext, and no funded wallet without a tested recovery path. Every one of those rules exists because we measured what happens without them.

**Verification is the product, not a test stage.**
A green that cannot go red is not a signal. We treat a monitor that never fires, a guard that can't be provoked, and a value printed as `0` because the read failed as the same class of bug — a confident wrong answer.

**Back up the ability to act.**
A backup that restores files but not the ability to *use* them fails the only day it matters. Disaster recovery here includes the credentials, the runbook and the tested restore drill.

---

## How we work

- **Measure before it publishes.** Size, secrets and structure are checked before a repo gets a remote.
- **Fix the class, not the instance.** A patch that has to be re-applied is evidence, not progress.
- **The audit is the deliverable.** "I found X, fixed it as Y, verified by Z" — and if it can't be verified, it's labelled unaudited.

---

## Start here

1. Install the kit: `uvx --from git+https://github.com/Gentech-Labs/genTech-agent-kit.git gentech-kit`
2. Read what's included: [genTech-agent-kit](https://github.com/Gentech-Labs/genTech-agent-kit)
3. See the security posture: [solana-agent-security](https://github.com/Gentech-Labs/solana-agent-security)

Built by [Jordan Jones](https://github.com/Gentech-Labs) · GenTech Labs
