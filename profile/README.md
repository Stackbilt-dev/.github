<p align="center">
  <img src="https://raw.githubusercontent.com/Stackbilt-dev/.github/main/profile/banner.png" alt="Stackbilt — Edge-Native Product Studio" width="600" />
</p>

<p align="center">
  <a href="https://bsky.app/profile/stackbilt.dev"><img src="https://img.shields.io/badge/Bluesky-stackbilt.dev-blue" alt="Bluesky" /></a>
  <a href="https://registry.modelcontextprotocol.io/v0.1/servers?search=stackbilt"><img src="https://img.shields.io/badge/MCP_Registry-dev.stackbilt.mcp%2Fgateway-blue" alt="MCP Registry" /></a>
  <a href="https://blog.stackbilt.dev"><img src="https://img.shields.io/badge/Blog-The_Roundtable-teal" alt="Blog" /></a>
</p>

---

## What we do

Stackbilt is a solo-founder + AI co-founder studio building production systems on Cloudflare's edge platform. TypeScript end to end, serverless everywhere, AI-native by default. No pitch decks, no vaporware — everything listed here is deployed and running. Total infrastructure cost: $0/month (Workers free tier + Workers AI for inference).

## Products

| Product | What it does | Status |
|---|---|---|
| **[AEGIS](https://aegis.stackbilt.dev/health)** | Persistent AI agent framework — multi-tier memory, autonomous goals, dreaming cycle, 26 scheduled tasks, runtime dynamic tools, MCP server. [Open source.](https://github.com/Stackbilt-dev/aegis-oss) | **Live** |
| **[img-forge](https://imgforge.stackbilt.dev)** | AI image generation API — 5 quality tiers, SDXL/FLUX/Gemini models, REST API + MCP server | **Live** |
| **[Stackbilder](https://stackbilt.dev)** | Architecture scaffolding via MCP. Describe your app, get deployable Cloudflare Worker code | **Live** |
| **[FoodFiles](https://foodfiles.stackbilt.dev)** | Structured food data API | Active |
| **TarotScript** | Symbolic computation engine — deterministic classification, zero inference cost | Active |

## Platform

- **[stackbilt-auth](https://auth.stackbilt.dev)** — Multi-tenant auth. Stripe billing, GitHub/Google SSO, unified credit pools, 16 RPCs. Every product authenticates through a single Service Binding.
- **[MCP Gateway](https://github.com/Stackbilt-dev/stackbilt-mcp-gateway)** — OAuth 2.1 (PKCE) remote MCP server. Published on the [Official MCP Registry](https://registry.modelcontextprotocol.io/) as `dev.stackbilt.mcp/gateway`. Connect any client to `mcp.stackbilt.dev/mcp`.

## Open Source

| Repository | Description | License |
|---|---|---|
| **[aegis-oss](https://github.com/Stackbilt-dev/aegis-oss)** | Persistent AI agent framework for Cloudflare Workers. Multi-tier memory, autonomous goals, dreaming cycles, MCP native. | Apache-2.0 |
| **[cc-taskrunner](https://github.com/Stackbilt-dev/cc-taskrunner)** | Autonomous task queue for Claude Code. Safety hooks, branch isolation, PR creation, failure autopsy. 236+ sessions. | Apache-2.0 |
| **[charter](https://github.com/Stackbilt-dev/charter)** | AI agent governance CLI. Modular .ai/ files replace monolithic CLAUDE.md configs. | Apache-2.0 |
| **[mindspring](https://github.com/Stackbilt-dev/mindspring)** | Semantic search engine for ChatGPT/Claude conversation exports. Upload, embed, search your AI history. | MIT |
| **[social-sentinel](https://github.com/Stackbilt-dev/social-sentinel)** | Privacy-first social media sentiment monitoring. PII redaction, multi-tenant, Workers AI scoring. | MIT |
| **[n8n-transpiler](https://github.com/Stackbilt-dev/n8n-transpiler)** | n8n workflow → Cloudflare Workers transpiler. | MIT |
| **[MCP Gateway](https://github.com/Stackbilt-dev/stackbilt-mcp-gateway)** | OAuth MCP server routing tool calls to multiple backends. | — |
| **[equity-scenario-sim](https://github.com/Stackbilt-dev/equity-scenario-sim)** | Cap table simulator for partnership negotiations. | — |

## Stack

Edge-first unless there's a good reason not to:

- **Runtime:** Cloudflare Workers (V8 isolates)
- **Language:** TypeScript (strict)
- **APIs:** Hono
- **Storage:** D1, KV, R2, Vectorize
- **AI:** Multi-model dispatch — Claude, Groq, Workers AI (free inference)
- **Auth:** OAuth 2.1 (PKCE), consolidated RPC surface
- **Billing:** Stripe with weighted credit pools

## Contact

- Web: [stackbilt.dev](https://stackbilt.dev)
- Blog: [blog.stackbilt.dev](https://blog.stackbilt.dev) — The Roundtable
- Bluesky: [@stackbilt.dev](https://bsky.app/profile/stackbilt.dev)
- GitHub: [@Stackbilt-dev](https://github.com/Stackbilt-dev)
