<p align="center">
  <img src="https://raw.githubusercontent.com/Stackbilt-dev/.github/main/profile/banner.png" alt="Stackbilt — Edge-Native Product Studio" width="600" />
</p>

<p align="center">
  <a href="https://registry.modelcontextprotocol.io/v0.1/servers?search=stackbilt"><img src="https://img.shields.io/badge/MCP_Registry-dev.stackbilt.mcp%2Fgateway-blue" alt="MCP Registry" /></a>
  <a href="https://blog.stackbilt.dev"><img src="https://img.shields.io/badge/Blog-The_Roundtable-teal" alt="Blog" /></a>
</p>

---

## What we do

Stackbilt is a solo-founder software studio building production systems on Cloudflare's edge platform. TypeScript end to end, serverless everywhere, AI-native by default. No pitch decks, no vaporware — everything listed here is deployed and running.

## Platform

All products run on a shared platform backbone:

- **[stackbilt-auth](https://auth.stackbilt.dev)** — Consolidated auth service. Multi-tenant, Stripe billing (4 tiers), GitHub/Google SSO, unified credit pools, 16 RPCs. Every product authenticates through a single Service Binding.
- **[MCP Gateway](https://github.com/Stackbilt-dev/stackbilt-mcp-gateway)** — OAuth 2.1 (PKCE) protected remote MCP server. Published on the [Official MCP Registry](https://registry.modelcontextprotocol.io/) as `dev.stackbilt.mcp/gateway`. Connect any MCP client to `mcp.stackbilt.dev/mcp`.
- **Observability Pipeline** — Event-driven usage tracking, cost reporting, tool analytics, and generation metrics via Cloudflare Queues.

## Products

| Product | What it does | Status |
|---|---|---|
| **[AEGIS](https://aegis.stackbilt.dev?utm_source=github&utm_medium=org-profile&utm_campaign=launch)** | Persistent autonomous AI agent — hybrid vector memory, 8-tier cost model, full SDLC pipeline (GitHub issue → merged PR), cross-repo intelligence, MCP server (20 tools) | **Live** |
| **[Stackbilder](https://stackbilt.dev?utm_source=github&utm_medium=org-profile&utm_campaign=launch)** | AI architecture engine for full-stack edge applications | **Live** |
| **[img-forge](https://imgforge.stackbilt.dev?utm_source=github&utm_medium=org-profile&utm_campaign=launch)** | Multi-model image generation API (FLUX.2, Stable Diffusion, Gemini) with OAuth 2.1 MCP server | **Live** |
| **[FoodFiles](https://foodfiles.stackbilt.dev)** | Structured food data API | Active |
| **TarotScript** | Symbolic computation language for deterministic tarot analysis | Active |

## Open Source

### [Charter](https://github.com/Stackbilt-dev/charter) — AI Developer Framework

ADF context management for AI agents. Define decision boundaries, context rules, and behavioral constraints — provider-agnostic.

- Apache-2.0 licensed
- ADF context compiler (format, bundle, patch, evidence, migrate)
- CLI: `@stackbilt/cli`

### [MCP Gateway](https://github.com/Stackbilt-dev/stackbilt-mcp-gateway) — OAuth MCP Server

Production MCP gateway routing tool calls to multiple backend services through a single OAuth-authenticated endpoint. 10 tools across 2 products.

### [cc-taskrunner](https://github.com/Stackbilt-dev/cc-taskrunner) — Autonomous Claude Code Task Runner

Queue-driven task execution for Claude Code. Safety hooks, governance tiers, auto-PR creation. Powers AEGIS's issue→PR pipeline.

## Stack

Edge-first unless there's a good reason not to:

- **Runtime:** Cloudflare Workers (V8 isolates)
- **Language:** TypeScript
- **APIs:** Hono
- **Storage:** D1, KV, R2, Vectorize
- **AI:** Multi-model orchestration across 8 cost tiers (Claude, Groq, Workers AI, OpenAI-compatible)
- **Auth:** OAuth 2.1 (PKCE), consolidated RPC surface
- **Billing:** Stripe with weighted credit pools

## Contributing

Charter is our primary open-source project and welcomes contributions under the [DCO](https://developercertificate.org/). See the [Charter contributing guide](https://github.com/Stackbilt-dev/charter/blob/main/CONTRIBUTING.md).

## Contact

- Web: [stackbilt.dev](https://stackbilt.dev?utm_source=github&utm_medium=org-profile&utm_campaign=launch)
- Blog: [blog.stackbilt.dev](https://blog.stackbilt.dev?utm_source=github&utm_medium=org-profile&utm_campaign=launch) — The Roundtable
- GitHub: [@Stackbilt-dev](https://github.com/Stackbilt-dev)
