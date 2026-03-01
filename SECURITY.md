# Security Policy

This is the default security policy for all repositories under the Stackbilt-dev organization. Individual repositories may have their own SECURITY.md with product-specific guidance — check the repository root first.

## Reporting a Vulnerability

**Do not open a public GitHub issue for security vulnerabilities.**

Email: **security@stackbilt.dev**

Include:
- Vulnerability description
- Affected product and version (if known)
- Reproduction steps
- Potential impact
- Suggested mitigation (if available)

### Response Targets

| Severity | Acknowledgement | Fix Target |
|---|---|---|
| Critical (active exploitation, data exposure) | 24 hours | 7 days |
| High (exploitable with effort) | 48 hours | 14 days |
| Medium / Low | 5 business days | Next release cycle |

These are targets, not SLAs. Stackbilt is a solo-founder operation — response times reflect that reality honestly. Critical issues affecting user data will always be prioritized above everything else.

## Scope

This policy covers all software published under the Stackbilt-dev GitHub organization, including but not limited to:

| Product | Type | Notes |
|---|---|---|
| **Charter** | OSS governance toolkit | Has its own [SECURITY.md](https://github.com/Stackbilt-dev/charter/blob/main/SECURITY.md) |
| **EdgeStack** | AI developer platform (SaaS) | Private repo — report via email |
| **img-forge** | MCP text-to-image API | Private repo — report via email |
| **FoodFiles** | Structured food data API | Private repo — report via email |
| **GameHub** | Family gaming platform | See additional guidance below |

### GameHub — Additional Guidance

GameHub is designed for families and children. Vulnerabilities that could expose child user data, bypass parental controls, or enable contact between users are treated as **Critical** regardless of technical severity. If you discover any issue in this category, email security@stackbilt.dev immediately.

## Out of Scope

The following are appreciated but not treated as security vulnerabilities:

- Denial of service against free-tier services (we run on Cloudflare — they handle DDoS)
- Rate limiting bypass on non-authenticated endpoints (unless it enables data access)
- Missing security headers on non-production deployments (localhost, preview URLs)
- Social engineering of the sole founder (nice try)
- Vulnerabilities in third-party dependencies where we are not the upstream maintainer (report those upstream; let us know if we should pin or patch)

## Disclosure Policy

- We practice **coordinated disclosure**. We ask that you give us a reasonable window (minimum 90 days for non-critical, 30 days for critical) to address the issue before public disclosure.
- We will credit reporters in release notes and changelogs unless you prefer to remain anonymous.
- We do not pursue legal action against good-faith security researchers acting within this policy.

## Security Contact

- **Primary:** security@stackbilt.dev
- **Fallback:** admin@stackbilt.dev
- **PGP:** Not currently available. If you need encrypted communication, request it and we will set up a secure channel.

## General Security Posture

Across all Stackbilt products:

- **Edge-first architecture.** Production services run on Cloudflare Workers. No traditional servers to patch, no SSH access to compromise, no persistent processes to hijack.
- **No secrets in code.** Secrets are managed via Cloudflare Wrangler secrets or environment-specific `.dev.vars` files (never committed). If you find a committed secret, report it.
- **Minimal dependencies.** We actively minimize the dependency tree. Fewer dependencies = smaller attack surface.
- **TLS everywhere.** All production traffic is HTTPS via Cloudflare. No exceptions.
- **No tracking.** No analytics SDKs, no advertising networks, no third-party tracking scripts across any product. Fewer third parties = fewer vectors.

---

*This policy is maintained by Stackbilt LLC. Last updated: 2026-03-01.*
