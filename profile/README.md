# Stackbilt

Edge-native product studio. We build, operate, and ship production AI systems and developer tools — and open-source the infrastructure worth sharing.

---

## What we do

Stackbilt is a solo-founder software studio building production systems on Cloudflare's edge platform. TypeScript end to end, serverless everywhere, AI-native by default. No pitch decks, no vaporware — everything listed here is deployed and running.

## Platform

All products run on a shared platform backbone:

- **[stackbilt-auth](https://auth.stackbilt.dev)** — Consolidated auth service. Multi-tenant, Stripe billing (4 tiers), GitHub/Google SSO, unified credit pools, 16 RPCs. Every product authenticates through a single Service Binding.
- **[MCP Gateway](https://mcp.stackbilt.dev)** — OAuth 2.1 (PKCE) protected remote MCP server gateway. Third-party MCP client access to Stackbilt services.
- **Observability Pipeline** — Event-driven usage tracking, cost reporting, tool analytics, and generation metrics via Cloudflare Queues.

## Products

| Product | What it does | Status |
|---|---|---|
| **[AEGIS](https://aegis.stackbilt.dev)** | Persistent autonomous AI agent — hybrid vector memory, 8-tier cost model, full SDLC pipeline (GitHub issue → merged PR), cross-repo intelligence, MCP server (20 tools) | **Live** |
| **[Stackbilder](https://stackbilt.dev)** | AI architecture engine for full-stack edge applications | **Live** |
| **[img-forge](https://imgforge.stackbilt.dev)** | Multi-model image generation API (FLUX.2, Stable Diffusion, Gemini) with OAuth 2.1 MCP server | **Live** |
| **[FoodFiles](https://foodfiles.stackbilt.dev)** | Structured food data API | Active |
| **TarotScript** | Symbolic computation language for deterministic tarot analysis | Active |

## Open Source

### [Charter](https://github.com/Stackbilt-dev/charter)

AI Developer Framework (ADF) for agent context management. Gives teams a structured way to define decision boundaries, context rules, and behavioral constraints for AI agents — provider-agnostic.

- Apache-2.0 licensed
- ADF context compiler (format, bundle, patch, evidence, migrate)
- CLI: `@stackbilt/cli`

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

- Web: [stackbilt.dev](https://stackbilt.dev)
- GitHub: [@Stackbilt-dev](https://github.com/Stackbilt-dev)
