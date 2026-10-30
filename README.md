# Nagios

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

Nagios is a family of open-source and commercial IT infrastructure monitoring tools, including Nagios Core (the original open-source monitoring engine), Nagios XI (the commercial enterprise distribution), Nagios Fusion, Nagios Log Server, and Nagios Network Analyzer, used to monitor hosts, services, networks, applications, and metrics with alerting and reporting. Nagios Core itself has no central HTTP API; Nagios XI ships a built-in REST API (typically reached at https://{nagios-xi-host}/nagiosxi/api/v1/) for reading, writing, deleting, and updating monitoring configuration and status. The Nagios XI API is authenticated via a per-user API key passed as a query parameter or header. Passive check results can also be submitted via NRDP (HTTP, JSON/XML) or NSCA (encrypted TCP, port 5667), and the NCPA cross-platform agent exposes a hierarchical REST API on port 5693.

**Areas:** Monitoring · Infrastructure Monitoring · Network Monitoring · Open Source · IT Operations · Alerting · Observability · Nagios XI · Nagios Core · NCPA · NRPE · NSCA

## Nagios on APIs.io

Everything profiled for Nagios is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/nagios/](https://apis.io/providers/nagios/)** — or go straight to one of the APIs or properties below.

### APIs (13)

- [NSCA (Nagios Service Check Acceptor)](https://apis.io/apis/nagios/nsca/) — Encrypted binary TCP daemon (default port 5667) that accepts passive service/host check results from remote machines. Not REST — clients send tab-delimited…
- [NRPE (Nagios Remote Plugin Executor)](https://apis.io/apis/nagios/nrpe/) — Daemon that runs Nagios plugins on a remote Linux/Unix host on TCP port 5666, returning the plugin's exit code and output to the Nagios server. Binary…
- [Nagios Config API](https://apis.io/apis/nagios/nagios-config-api/) — Admin-only endpoints to add, modify, and delete hosts and services.
- [Nagios CPU API](https://apis.io/apis/nagios/nagios-cpu-api/) — System-wide CPU utilization and core counts.
- [Nagios Disk API](https://apis.io/apis/nagios/nagios-disk-api/) — Logical, physical, and mount-point disk metrics.
- [Nagios Interface API](https://apis.io/apis/nagios/nagios-interface-api/) — Network interface byte and packet counters.
- [Nagios Memory API](https://apis.io/apis/nagios/nagios-memory-api/) — Physical memory and swap.
- [Nagios Objects API](https://apis.io/apis/nagios/nagios-objects-api/) — Read-only backend for hosts, services, host groups, contacts, downtime, history, and other monitored objects.
- [Nagios Plugins API](https://apis.io/apis/nagios/nagios-plugins-api/) — User-defined Nagios-style plugins executed by the agent.
- [Nagios Processes API](https://apis.io/apis/nagios/nagios-processes-api/) — Running process inventory and resource use.
- [Nagios Services API](https://apis.io/apis/nagios/nagios-services-api/) — Host service / daemon status.
- [Nagios Submission API](https://apis.io/apis/nagios/nagios-submission-api/) — Submit passive check results and external commands.
- [Nagios System API](https://apis.io/apis/nagios/nagios-system-api/) — Admin-only endpoints to manage Nagios XI subsystems, apply configuration, schedule downtime, and execute commands.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Nagios Agentic Access](https://apis.io/agentic-access/nagios/nagios-agentic-access/)

#### JSON Schema (4)

The data models the API reads and writes.

- [Nagios Check Result](https://apis.io/schemas/nagios/nagios-check-result/)
- [Nagios XI Host](https://apis.io/schemas/nagios/nagios-xi-host/)
- [Nagios XI Service](https://apis.io/schemas/nagios/nagios-xi-service/)
- [NCPA Metric Response](https://apis.io/schemas/nagios/ncpa-metric/)

#### JSON Structure (2)

Data models expressed in JSON Structure.

- [Nagios Check Result Structure](https://apis.io/json-structure/nagios/nagios-check-result-structure/)
- [Nagios Xi Host Structure](https://apis.io/json-structure/nagios/nagios-xi-host-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Nagios Context](https://apis.io/jsonld/nagios/nagios-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Nagios Vocabulary](https://apis.io/vocabularies/nagios/nagios-vocabulary/)

#### Examples (7)

Example requests and responses.

- [Nagios Xi Host Create Example](https://apis.io/examples/nagios/nagios-xi-host-create-example/)
- [Nagios Xi Host Status Example](https://apis.io/examples/nagios/nagios-xi-host-status-example/)
- [Nagios Xi Service Delete Example](https://apis.io/examples/nagios/nagios-xi-service-delete-example/)
- [Nagios Xi System Status Example](https://apis.io/examples/nagios/nagios-xi-system-status-example/)
- [Ncpa Cpu Percent Example](https://apis.io/examples/nagios/ncpa-cpu-percent-example/)
- [Ncpa Memory Virtual Example](https://apis.io/examples/nagios/ncpa-memory-virtual-example/)
- [Nrdp Submit Check Example](https://apis.io/examples/nagios/nrdp-submit-check-example/)

#### Collections (14)

Postman and Open Collection request collections.

- [Nagios XI REST Config API](https://apis.io/collections/nagios/open-nagios-config-api/)
- [Nagios XI REST Config CPU API](https://apis.io/collections/nagios/open-nagios-cpu-api/)
- [Nagios XI REST Config Disk API](https://apis.io/collections/nagios/open-nagios-disk-api/)
- [Nagios XI REST Config Interface API](https://apis.io/collections/nagios/open-nagios-interface-api/)
- [Nagios XI REST Config Memory API](https://apis.io/collections/nagios/open-nagios-memory-api/)
- [Nagios XI REST Config Objects API](https://apis.io/collections/nagios/open-nagios-objects-api/)
- [Nagios XI REST Config Plugins API](https://apis.io/collections/nagios/open-nagios-plugins-api/)
- [Nagios XI REST Config Processes API](https://apis.io/collections/nagios/open-nagios-processes-api/)
- [Nagios XI REST Config Services API](https://apis.io/collections/nagios/open-nagios-services-api/)
- [Nagios XI REST Config Submission API](https://apis.io/collections/nagios/open-nagios-submission-api/)
- [Nagios XI REST Config System API](https://apis.io/collections/nagios/open-nagios-system-api/)
- [Nagios XI REST API](https://apis.io/collections/nagios/open-nagios-xi/)
- [NCPA (Nagios Cross-Platform Agent) API](https://apis.io/collections/nagios/open-ncpa/)
- [NRDP (Nagios Remote Data Processor) API](https://apis.io/collections/nagios/open-nrdp/)

#### Governance rules (3)

Spectral rulesets for the provider's contracts.

- [Nagios — jsonschema rules](https://apis.io/rules/nagios/nagios-jsonschema-spectral-rules/)
- [Nagios — xi rules](https://apis.io/rules/nagios/nagios-xi-rules/)
- [Nagios — ncpa rules](https://apis.io/rules/nagios/ncpa-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Nagios Authentication](https://apis.io/security/nagios/nagios-authentication/)
- [Nagios Domain Security](https://apis.io/security/nagios/nagios-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Nagios Plans Pricing](https://apis.io/plans/nagios/nagios-plans-pricing/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.nagios.org)
- [Documentation](https://www.nagios.org/documentation/)
- [Pricing](https://www.nagios.com/products/pricing/)
- [Blog](https://www.nagios.com/feed/)
- [GitHub](https://github.com/NagiosEnterprises)

## API Evangelist rating

**Kin Score 35.7** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 53.1 |
| Contract governance | 27.3 |
| Operational transparency | 2.6 |
| Developer ergonomics | 31.0 |
| Access clarity | 18.4 |

**Agent readiness 17.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
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
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 16.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/nagios/](https://apis.io/providers/nagios/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Nagios: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/nagios/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
