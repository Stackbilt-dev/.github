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

Stackbilt is a solo-founder + AI co-founder studio building production systems on Cloudflare's edge platform. TypeScript end to end, serverless everywhere, AI-native by default. No pitch decks, no vaporware — everything listed here is deployed and running. Total infrastructure cost: $~25/month (Workers free tier + Workers AI for inference).

## Products

| Product | What it does | Status |
|---|---|---|
| **[AEGIS](https://aegis.stackbilt.dev/health)** | Persistent AI agent framework (`@stackbilt/aegis-core`) — multi-tier memory, autonomous goals, dreaming cycle, 26 scheduled tasks, MCP server. Deploy standalone or extend as a dependency. [Open source.](https://github.com/Stackbilt-dev/aegis-oss) | **Live** |
| **[img-forge](https://imgforge.stackbilt.dev)** | AI image generation API — 5 quality tiers, SDXL/FLUX/Gemini models, REST API + MCP server | **Live** |
| **[Stackbilder](https://stackbilder.com)** | Architecture scaffolding via MCP. Describe your app, get deployable Cloudflare Worker code | **Live** |
| **TarotScript** | Symbolic computation engine — deterministic classification, zero inference cost | Active |

## Platform

- **[edge-auth](https://auth.stackbilt.dev)** — Multi-property auth + billing. Stripe, GitHub/Google SSO, unified credit pools, API key management. Every product authenticates through a single Service Binding.
- **[MCP Gateway](https://github.com/Stackbilt-dev/stackbilt-mcp-gateway)** — OAuth 2.1 (PKCE) remote MCP server. Published on the [Official MCP Registry](https://registry.modelcontextprotocol.io/) as `dev.stackbilt.mcp/gateway`. Connect any client to `mcp.stackbilt.dev/mcp`.

## Open Source

| Repository | Description | License |
|---|---|---|
| **[aegis-oss](https://github.com/Stackbilt-dev/aegis-oss)** | Persistent AI agent framework (`@stackbilt/aegis-core`). Multi-tier memory, autonomous goals, dreaming cycles, MCP native. Use standalone or as a dependency. | Apache-2.0 |
| **[cc-taskrunner](https://github.com/Stackbilt-dev/cc-taskrunner)** | Autonomous task queue for Claude Code. Safety hooks, branch isolation, PR creation, failure autopsy. | Apache-2.0 |
| **[charter](https://github.com/Stackbilt-dev/charter)** | AI agent governance CLI + project scaffolder. Modular .ai/ files replace monolithic CLAUDE.md configs. | Apache-2.0 |
| **[llm-providers](https://github.com/Stackbilt-dev/llm-providers)** | Multi-LLM failover with circuit breakers, cost tracking, and intelligent retry. | Apache-2.0 |
| **[mindspring](https://github.com/Stackbilt-dev/mindspring)** | Semantic search engine for ChatGPT/Claude conversation exports. Upload, embed, search your AI history. | MIT |
| **[social-sentinel](https://github.com/Stackbilt-dev/social-sentinel)** | Privacy-first social media sentiment monitoring. PII redaction, multi-tenant, Workers AI scoring. | MIT |
| **[audit-chain](https://github.com/Stackbilt-dev/audit-chain)** | Tamper-evident hash-chained audit trail for Cloudflare Workers. | Apache-2.0 |
| **[worker-observability](https://github.com/Stackbilt-dev/worker-observability)** | Edge-native observability — structured logging, health checks, SLI monitoring. | Apache-2.0 |
| **[ai-playbook](https://github.com/Stackbilt-dev/ai-playbook)** | Battle-tested AI interaction frameworks, philosophical archetypes, and context engineering patterns. | MIT |
| **[n8n-transpiler](https://github.com/Stackbilt-dev/n8n-transpiler)** | n8n workflow → Cloudflare Workers transpiler. | MIT |
| **[feature-flags](https://github.com/Stackbilt-dev/feature-flags)** | Edge-native feature flags for Cloudflare Workers. KV-backed, per-tenant, canary rollouts. | Apache-2.0 |
| **[equity-scenario-sim](https://github.com/Stackbilt-dev/equity-scenario-sim)** | Cap table simulator for partnership negotiations. Model deal structures and exit scenarios. | — |
| **[MCP Gateway](https://github.com/Stackbilt-dev/stackbilt-mcp-gateway)** | OAuth MCP server routing tool calls to multiple backends. | — |

## Stack

Edge-first unless there's a good reason not to:

- **Runtime:** Cloudflare Workers (V8 isolates)
- **Language:** TypeScript (strict)
- **APIs:** Hono
- **Storage:** D1, KV, R2, Vectorize
- **AI:** Multi-model dispatch — Claude, Groq, Cerebras, Workers AI (free inference)
- **Auth:** OAuth 2.1 (PKCE), edge-auth consolidated RPC surface
- **Billing:** Stripe with weighted credit pools

## Contact

- Web: [stackbilder.com](https://stackbilder.com)
- Blog: [blog.stackbilt.dev](https://blog.stackbilt.dev) — The Roundtable
- Bluesky: [@stackbilt.dev](https://bsky.app/profile/stackbilt.dev)
- GitHub: [@Stackbilt-dev](https://github.com/Stackbilt-dev)
