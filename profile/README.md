# Stackbilt

API-first product studio. We build, operate, and ship vertical software products — and open-source the infrastructure worth sharing.

---

## What we do

Stackbilt is a solo-founder software studio focused on production systems that actually run. No pitch decks, no vaporware. Products ship on edge-first architecture (Cloudflare Workers, D1, KV, R2) with TypeScript end to end.

Current focus areas: AI developer tooling, structured data APIs, and governance tooling for AI-assisted development.

## Open Source

### [Charter](https://github.com/Stackbilt-dev/charter)

Local-first governance toolkit for LLM-assisted development. Charter gives teams a structured way to define decision boundaries, context rules, and behavioral constraints for AI agents — without locking into any single provider.

- Apache-2.0 licensed
- ADF context compiler (format, bundle, patch, evidence, migrate)
- CLI: `@stackbilt/cli`
- Works with any LLM provider

Charter is the public expression of how we think about AI governance: practical constraints that ship with your codebase, not policy documents that collect dust.

## Products

We operate several products under the **"Product by Stackbilt"** model. Most are currently private repos in active development.

| Product | What it does | Status |
|---|---|---|
| **EdgeStack** | AI-powered developer platform | Active (private) |
| **img-forge** | MCP-native text-to-image API | Pre-launch (private) |
| **FoodFiles** | Structured food data API | Active (private) |
| **TarotAPI** | Tarot reading API | Active (private) |

## Stack

We default to edge-first unless there's a good reason not to:

- **Runtime:** Cloudflare Workers
- **Language:** TypeScript everywhere
- **APIs:** Hono
- **Storage:** D1, KV, R2
- **AI:** Multi-provider with failover (never single-vendor lock-in)

## Contributing

Charter is our primary open-source project and welcomes contributions under the [DCO](https://developercertificate.org/) (sign-off your commits). See the [Charter contributing guide](https://github.com/Stackbilt-dev/charter/blob/main/CONTRIBUTING.md) for details.

For everything else, we're a small operation. If you're interested in what we're building, the best way to follow along is to watch this org or star the repos that interest you.

## Contact

- GitHub: [@Stackbilt-dev](https://github.com/Stackbilt-dev)
- Web: [stackbilt.dev](https://stackbilt.dev)
