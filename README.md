# Zeplin (zeplin)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
