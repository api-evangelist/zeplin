# Zeplin (zeplin)

Zeplin is a design-to-development handoff platform that bridges the gap between designers and developers by providing a structured workspace for accessing design specs, assets, style guides, components, and annotations. The Zeplin REST API enables programmatic access to all resources within Zeplin including projects, screens, components, layers, assets, and notes exported from Figma, Sketch, and Adobe XD. Developers can build custom integrations using read and write operations on design data, receive real-time updates via webhooks, and automate design-to-code workflows. The API uses OAuth 2.0 with PKCE support and personal access tokens for authentication, with an official JavaScript SDK and OpenAPI specification available.

- **APIs.json:** https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/apis.yml
- **Naftiko:** https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=zeplin-api-evangelist&utm_content=repo

## Tags

- Design
- Design Handoff
- Developer Tools
- Figma
- Sketch
- Adobe XD
- Style Guides
- Components
- Assets
- Webhooks

## APIs

### Zeplin API

The Zeplin REST API provides programmatic access to design collaboration data including projects, screens, components, layers, assets, style guides, annotations, and design tokens. Supports both read and write operations for select resources, real-time webhook notifications, and design token management including variable collections and modes.

- **Documentation:** https://docs.zeplin.dev/docs/welcome
- **API Reference:** https://docs.zeplin.dev/reference/introduction
- **OpenAPI Spec:** https://github.com/zeplin/openapi
- **Authentication:** https://docs.zeplin.dev/reference/authentication
- **Rate Limits:** https://docs.zeplin.dev/reference/rate-limiting
- **Webhooks:** https://docs.zeplin.dev/reference/webhook-events-overview
- **JavaScript SDK:** https://github.com/zeplin/javascript-sdk
- **MCP Server:** https://github.com/zeplin/mcp-server
- **CLI:** https://github.com/zeplin/cli

## Plans, Rate Limits, and FinOps

- **Plans and Pricing:** [plans/zeplin-plans-pricing.yml](plans/zeplin-plans-pricing.yml)
- **Rate Limits:** [rate-limits/zeplin-rate-limits.yml](rate-limits/zeplin-rate-limits.yml)
- **FinOps:** [finops/zeplin-finops.yml](finops/zeplin-finops.yml)

Zeplin offers four plans: Free ($0, 1 project, 100 screens), Basic ($13.75+/month per project bundle), Advanced ($12/seat/month), and Enterprise (custom). The API enforces 200 requests per minute per user with rate limit headers (Zeplin-RateLimit-Limit, Zeplin-RateLimit-Remaining, Zeplin-RateLimit-Reset). All API access is included in the platform subscription with no per-call charges.

## Timestamps

- **Created:** 2026-06-12
- **Modified:** 2026-06-12

## Common

| Type | URL |
|------|-----|
| Website | https://zeplin.io |
| Documentation | https://docs.zeplin.dev |
| GitHub Org | https://github.com/zeplin |
| LinkedIn | https://www.linkedin.com/company/zeplin-io |
| Blog | https://blog.zeplin.io |
| Pricing | https://zeplin.io/pricing/ |
| Status Page | https://status.zeplin.io |
| X (Twitter) | https://twitter.com/zeplinproject |

## Maintainers

- **Kin Lane** - kin@apievangelist.com
