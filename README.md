# Replica

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

Replica is a San Francisco-based data platform for the built environment, spun out of Alphabet's Sidewalk Labs in 2019, that operates a nationwide activity-based travel model. Its analytical engine combines public data (US Census/ACS, GTFS transit feeds, OpenStreetMap road networks, land-use records, state traffic counts) with licensed private data (de-identified aggregate mobile location, credit transaction and driving-behavior data) to synthesize a privacy-preserving simulated population and a complete trip table for the United States. Products include Places (seasonal, high-fidelity activity-based travel model), Trends (weekly near-real-time mobility and land-use data), Safety Hub, Safe Streets Planner, and a suite of workflow applications used by state DOTs, MPOs, transit agencies, cities and counties. Data is consumed through the Replica Studio web platform, CSV export and direct database access; Replica publishes documented dataset schemas at documentation.replicahq.com but no public developer REST API, SDK or developer portal.

**Areas:** Company · Data · Mobility · Transportation · Geospatial · Urban Planning · Travel Demand Modeling · Government · Analytics · Data Platform

## Replica on APIs.io

Everything profiled for Replica is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/replica/](https://apis.io/providers/replica/)** — or go straight to one of the APIs or properties below.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [replica](https://apis.io/servers/replica/replica/)

#### JSON Schema (19)

The data models the API reads and writes.

- [Active Transportation Trips](https://apis.io/schemas/replica/replica-active-transportation/)
- [Annual Average Daily Traffic (AADT)](https://apis.io/schemas/replica/replica-annual-average-daily-traffic-aadt/)
- [Auto and TNC Trips](https://apis.io/schemas/replica/replica-auto-tnc-trips/)
- [Commercial Freight Trips](https://apis.io/schemas/replica/replica-commercial-freight/)
- [[Discontinued] Spend County-to-County Flows](https://apis.io/schemas/replica/replica-consumer-spending-by-county-to-county-flows/)
- [[Discontinued] Weekly Spend (by home location)](https://apis.io/schemas/replica/replica-consumer-spending-by-home-merchant-location/)
- [Crash Data](https://apis.io/schemas/replica/replica-crash-data/)
- [Daily Network Link Volumes](https://apis.io/schemas/replica/replica-daily-network-link-volumes/)
- [Daily O-D Pairs](https://apis.io/schemas/replica/replica-daily-o-d-data/)
- [Daily VMT](https://apis.io/schemas/replica/replica-daily-vmt/)
- [Demographics and Employment](https://apis.io/schemas/replica/replica-demographics-employment/)
- [Seasonal Trip Table](https://apis.io/schemas/replica/replica-disaggregate-trip-tables/)
- [Annual Speeds per Network Link](https://apis.io/schemas/replica/replica-free-flow-speed-per-network-link/)
- [Hourly Auto Volume Profile](https://apis.io/schemas/replica/replica-hourly-auto-volume-profile/)
- [Network Links](https://apis.io/schemas/replica/replica-network-links/)
- [Annual Quarter-Hourly Speed Profiles](https://apis.io/schemas/replica/replica-quarter-hourly-speed-profile-per-network-link-annual/)
- [Transit Trips](https://apis.io/schemas/replica/replica-transit/)
- [Turning Movement Counts](https://apis.io/schemas/replica/replica-turning-movement-counts-tmcs/)
- [[Discontinued] Weekly Spend (by merchant location)](https://apis.io/schemas/replica/replica-weekly-spend-by-merchant-location/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Replica Domain Security](https://apis.io/security/replica/replica-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.replicahq.com/)
- [Documentation](https://documentation.replicahq.com/)
- [Getting started](https://help.replicahq.com/en/collections/1232529-introduction-to-replica)
- [Support](https://help.replicahq.com/en/)
- [Changelog](https://help.replicahq.com/en/articles/4374395-replica-product-release-notes)
- [Blog](https://www.replicahq.com/blog)
- [Terms of service](https://www.replicahq.com/terms-of-use)
- [Privacy policy](https://www.replicahq.com/privacy-policy)
- [GitHub](https://github.com/replicahq)

## API Evangelist rating

**Kin Score 17.4** — emerging · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 58.3 |
| Contract quality | 0.0 |
| Contract governance | 33.3 |
| Operational transparency | 18.4 |
| Developer ergonomics | 21.4 |
| Access clarity | 6.6 |

**Agent readiness 12.2** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 10.8** — Government & Public Sector

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/replica/](https://apis.io/providers/replica/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Replica: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/replica/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
