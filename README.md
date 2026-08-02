# Replica

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
