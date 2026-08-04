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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Replica is a San Francisco-based data platform for the built environment, spun out of Alphabet's
Sidewalk Labs in 2019, that operates a nationwide activity-based travel model. Its engine combines
public data (US Census/ACS, GTFS, OpenStreetMap, land-use records, state traffic counts) with
licensed private data (de-identified aggregate mobile location, credit transaction and
driving-behavior data) to synthesize a privacy-preserving simulated population and a complete trip
table for the United States.

- Website: https://www.replicahq.com/
- Documentation: https://documentation.replicahq.com/
- Help center: https://help.replicahq.com/en/
- Platform (login): https://studio.replicahq.com/
- GitHub: https://github.com/replicahq

## API surface

**Replica publishes no public developer API.** Contract discovery probed `replicahq.com`,
`documentation.replicahq.com`, `studio.replicahq.com` and `api.studio.replicahq.com` for OpenAPI,
Swagger, GraphQL, MCP `tools/list`, A2A agent cards and every `/.well-known/*` discovery document —
all missed. The documentation site is ReadMe.io-hosted but its API-reference section is not enabled.
The Studio application is backed by a private `api.studio.replicahq.com/api/v1/*` service that
answers `401 Unauthorized` behind an Express session cookie; it is undocumented and is not offered
as a developer API. Beware the marketing site's SPA catch-all, which answers HTTP 200 with an HTML
shell for `/openapi.json`, `/llms.txt` and every `/.well-known/*` path.

What Replica *does* publish machine-readably is its **dataset schemas** — field name, content type,
sample value and description for each data product. Those are captured here.

## Artifacts

| Path | What |
|---|---|
| `vocabulary/replica-data-dictionary.yml` | Data dictionary: 19 datasets, 338 documented fields, harvested from the documentation schema tables |
| `json-schema/` | One JSON Schema (2020-12) per dataset, derived from the data dictionary, plus `_index.yml` |
| `data-model/replica-data-model.yml` | Entity-relationship graph (person / household / trip / network_link / transit_route / geography / intersection) derived from the documented join keys |
| `llms/replica-llms.txt` | Verbatim `llms.txt` from documentation.replicahq.com |
| `changelog/replica-changelog.yml` | Structured recent release notes (seasonal data, annual traffic, platform, product launches) |
| `lifecycle/replica-lifecycle.yml` | Data-vintage versioning cadence, dated dataset discontinuations, absent SLA/status page |
| `conformance/replica-conformance.yml` | Reference-standard conformance (OSM, GTFS, FIPS, ACS/PUMS/CTPP/LEHD, NAICS, HPMS, NHTSA FARS, WGS 84, H3, WKT/GeoJSON, published privacy principles) plus the negative API-protocol rows |
| `packages/replica-packages.yml` | First-party open-source libraries (no API client SDK exists) |
| `well-known/replica-well-known.yml` | Full `/.well-known/` probe record — zero documents found |
| `security/replica-domain-security.yml` | TLS/HSTS per host; DNSSEC, SPF and DMARC (p=reject) on replicahq.com |

## Disambiguation

**Replica (replicahq.com)** — this repo — is not **Replica Cyber (replicacyber.com)**, **Replicate
(replicate.com)**, **Replicated (replicated.com)**, **Replicant** or **Replika**. Public claims that
"Replica achieved SOC 2 Type II" belong to Replica Cyber and are not attributed here.
