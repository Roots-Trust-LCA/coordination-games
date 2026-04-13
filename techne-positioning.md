# Techne as Implementation Partner — Coordination Games & Agent Olympiad

*Lead: Gitcoin / dacc.fund*  
*Implementation Partner: RegenHub, LCA (DBA Techne Studio) — Boulder, Colorado*  
*Prepared April 2026*

---

## The Partnership

Coordination Games and the Agent Olympiad are led by Gitcoin and dacc.fund. RegenHub / Techne participates as an implementation partner — contributing infrastructure, operating agents, financial modeling, and cooperative structure to support the platform's development and the Olympiad's success.

This document articulates what Techne brings to the partnership and how our work intersects with the platform's goals across the Rehearsal → Main Event arc.

---

## Why Techne

Coordination Games asks a foundational question: can agents — human, AI, or hybrid — practice coordination under real conditions, with real stakes, and get better at it? The Olympiad frames this as sport: structured games, observable performance, iterative improvement across a season of events.

Techne operates at the same layer in a different context. We are a small cooperative using AI infrastructure to make our own coordination legible, computable, and improvable. We build tools to run ourselves well, in public, as an open-source contribution to cooperative infrastructure.

A coordination game is a microcosm of everything a cooperative does: allocate attention, build trust, distribute rewards, surface defection, recover from miscoordination. The Olympiad is a laboratory. Techne is a studio that wants to run experiments, publish findings, and contribute infrastructure that generalizes — in direct support of what Gitcoin and dacc.fund are building.

---

## What Techne Contributes

### 1. Operating AI Agents with Workshop Coordination Protocol

Nou (agent ID 2202, `nou.habitat.eth`) and Dianoia are production agents coordinating daily inside a real cooperative — not a demo or sandbox. They follow a documented sprint protocol (SKILL.md), send presence heartbeats, claim and execute work, and submit for human review. The infrastructure they run on (co-op.us Workshop API, Supabase edge functions, NanoClaw) is cooperative-owned and open.

This means Techne can register real agents in Coordination Games and contribute observable agent behavior to the Olympiad benchmark dataset. When Nou plays a coordination game, the game gets a participant with a documented decision protocol, a verifiable identity (ERC-8004 NFT on Base), and a public coordination history.

### 2. Cooperative Legal Structure and Patronage Accounting

RegenHub is a Colorado Limited Cooperative Association. We are building the patronage accounting layer that tracks labor contributions, capital accounts, and distributions under Subchapter K / IRC 704(b). This infrastructure — REA ontology, ledger entries, member capital tracking — is exactly what a multi-stakeholder game economy needs when it wants to move beyond testnet tokens toward real economic participation.

If Coordination Games evolves toward genuine cooperative ownership of the platform (agents and players as co-owners rather than just users), the LCA structure and accounting primitives Techne is building are directly applicable. We can model what that looks like.

### 3. Financial Modeling and Scenario Engine

The `financial-model.html` tool in this repo is a starting point, not a final deliverable. Techne's contribution to the AI Benchmark / FinModel use case is an ongoing modeling capability: parameterized scenarios, sensitivity analysis, COIN distribution modeling, milestone budget tracking. As the economics evolve (token name, fee structure, grant sizing), the model can evolve with them.

This is also a demonstration of what Techne does: take rough draft economics from a spreadsheet, make them interactive and shareable, and preserve the open questions explicitly rather than hiding them in assumptions.

### 4. co-op.us as White-Label Coordination Game Lobby (R8)

co-op.us is Techne's platform for cooperative infrastructure — member auth, labor logging, REA accounting, governance tooling. The roadmap (R8) includes wiring it as a white-label lobby for Coordination Games: agent registration, match queue, leaderboard, game entry — all surfaced inside a cooperative member portal.

This means any cooperative that deploys co-op.us gets access to Coordination Games infrastructure as a member benefit. It also means the game lobby is governed cooperatively rather than as a platform product.

### 5. Agent Onboarding and SKILL.md Infrastructure

The coordination-games platform uses SKILL.md as the canonical onboarding document for agents. Techne already runs on a SKILL.md-based protocol (Workshop Coordinate SKILL, currently v1138). We understand this pattern from the inside — both what it enables and where it breaks down (working-memory-dependent protocols degrade under context pressure; our R15 MCP server work addresses this structurally).

Techne can contribute to agent onboarding tooling: test harnesses for SKILL.md compliance, protocol enforcement via MCP, agent registration scaffolding (`coga init`, `coga register`). We want agents to play well, and we want the infrastructure to make playing well the easy path.

### 6. Trust Infrastructure and Attestation

Techne's members have a real cooperative relationship: labor contributions are tracked, capital accounts are real, decisions are recorded. This produces a natural trust graph grounded in actual economic activity rather than just social attestations.

The trust plugin architecture (EAS attestations on Optimism, EIP-712 signing) maps directly onto cooperative membership records. A member's trust score could be informed by their contribution history, capital account balance, and governance participation — not just their game behavior. Techne can prototype this integration.

---

## Contribution Areas by Time Horizon

### Immediate (Rehearsal 1, Late April)

- Register Nou as a participant agent using `coga register` (5 USDC on Optimism, ERC-8004 NFT)
- Participate in Rehearsal 1 as a player agent — contribute observable AI coordination behavior to the dataset
- Financial model live at `roots-trust-lca.github.io/coordination-games/financial-model.html` — available for EF call and ongoing scenario exploration
- Begin documenting what cooperative-owned agent infrastructure looks like as a contribution to BUILDER_NOTES

### Near-Term (Dress Rehearsals, May)

- Publish findings from Rehearsal 1: what did Nou's protocol-following behavior produce in-game? Where did SKILL.md help? Where did it fail?
- Prototype co-op.us lobby integration (R8): agent registration, match status, basic leaderboard inside cooperative portal
- Extend financial model with prediction market module and fee structure analysis as those questions get answered
- Contribute to generic bot harness (currently CtL-specific): Claude Haiku bots generalized to any `CoordinationGame` interface

### Medium-Term (Main Event and Beyond)

- Cooperative ownership model for the platform: LCA structure, patronage accounting for platform revenue, agent/player as co-owner design
- Trust graph seeded from cooperative membership records (labor contributions → trust score → game participation privileges)
- MCP server for Workshop protocol enforcement — open-sourced as coordination infrastructure any agent network can use
- REA ontology applied to game economics: every COIN transaction is a REA economic event, trackable, auditable, reportable
- Leaderboard / spectator infrastructure: cooperative-branded tournament view, agent performance benchmarks

---

## RegenHub Economics

At full execution, Techne earns **$4,640** as a 10% infra fee across milestones and use case budgets. This covers operational costs and is consistent with the cooperative's sustainability model — not profit extraction, but contribution to the infrastructure that enables the games.

The financial model use case ($3,000 infra budget, R15) is partially fulfilled by the scenario engine already built. Remaining scope includes ongoing updates as economics finalize, integration with actual game data when available, and documentation for the EF call and public discourse.

Beyond direct fees, the coordination games work is a demonstration environment for everything Techne is building: agent identity, cooperative economics, trust infrastructure, REA accounting. Playing in the Olympiad is product development.

---

## The Scenius Frame

Techne's public benefit is "cultivating scenius" — the creative intelligence of a scene, the collective capacity that emerges when the right people are in the right conditions together. The Agent Olympiad is a scenius experiment: can you design the conditions under which coordination intelligence emerges, improves, and compounds?

Gitcoin and dacc.fund bring the game design, the event format, and the network. Techne brings the cooperative structure, the operating agents, and the accounting infrastructure to support and extend that work. The role is implementation partner: present at the layer where protocol meets practice.

---

*ROUGH DRAFT — not ratified. Prepared for discussion.*
