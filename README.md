# Nagios (nagios)

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

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/nagios/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Monitoring
- Infrastructure Monitoring
- Network Monitoring
- Open Source
- IT Operations
- Alerting
- Observability
- Nagios XI
- Nagios Core
- NCPA
- NRPE
- NSCA
- NRDP

## Timestamps

- **Created:** 2026-05-11
- **Modified:** 2026-05-23

## APIs

### Nagios XI REST API

Built-in REST API for Nagios XI. Split into three sections: Objects (read-only backend for hosts, services, host groups, contacts, downtime, history), Config (admin-only writes for hosts and services), and System (admin-only commands such as apply configuration, scheduled downtime, status). Responses are returned as JSON. Authentication uses a per-user Nagios XI API key passed via the `apikey` query parameter (or header). Custom endpoints can be added by creating a Nagios XI Component.

- **Human URL:** [https://support.nagios.com/kb/article/nagios-xi-rest-api-176.html](https://support.nagios.com/kb/article/nagios-xi-rest-api-176.html)
- **Base URL:** `https://{nagios-xi-host}/nagiosxi/api/v1`

#### Tags

- Monitoring
- REST
- Nagios XI
- IT Operations

#### Properties

- [Documentation](https://support.nagios.com/kb/article/nagios-xi-rest-api-176.html)
- [A P I  P D F  Guide](https://assets.nagios.com/downloads/nagiosxi/docs/Accessing-and-Using-the-XI-REST-API.pdf)
- [Backend  A P I](https://assets.nagios.com/downloads/nagiosxi/docs/Accessing_The_XI_Backend_API.pdf)
- [Automated  Host  Management](https://assets.nagios.com/downloads/nagiosxi/docs/Automated_Host_Management.pdf)
- [OpenAPI](openapi/nagios-xi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/nagios-xi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/nagios-xi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/nagios-xi-host-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/nagios-xi-service-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/nagios-xi-host-structure.json)
- [Spectral Rules](rules/nagios-xi-rules.yml)

### NCPA (Nagios Cross-Platform Agent) API

REST API exposed by the Nagios Cross-Platform Agent (NCPA), a cross-platform monitoring agent that runs on Linux, Windows, and macOS. Uses a hierarchical URL structure `/api/{module}/{node1}/{node2}` for CPU, memory, disk, interface, process, service, and plugin metrics. Both active polling and passive Nagios-style check results (`check=1` + thresholds) are supported. Authenticated via a `token` query parameter matching the `community_string` in the agent config. Default TLS port 5693.

- **Human URL:** [https://www.nagios.org/ncpa/help/3.x/api.html](https://www.nagios.org/ncpa/help/3.x/api.html)
- **Base URL:** `https://{ncpa-host}:5693/api`

#### Tags

- Monitoring
- Agent
- REST
- NCPA

#### Properties

- [Documentation](https://www.nagios.org/ncpa/help/3.x/api.html)
- [Git Hub](https://github.com/NagiosEnterprises/ncpa)
- [OpenAPI](openapi/ncpa-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ncpa.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ncpa.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/ncpa-metric-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Spectral Rules](rules/ncpa-rules.yml)

### NRDP (Nagios Remote Data Processor) API

PHP-based HTTP collector that accepts passive check results and external commands. Two commands are supported: `submitcheck` (host/service check results) and `submitcmd` (Nagios external command). Payloads can be sent as XML (`XMLDATA`) or JSON (`JSONDATA`) in a POST form. Authenticated by a token configured in `config.inc.php` with optional per-command deny mappings.

- **Human URL:** [https://github.com/NagiosEnterprises/nrdp](https://github.com/NagiosEnterprises/nrdp)
- **Base URL:** `https://{nrdp-host}/nrdp`

#### Tags

- Monitoring
- Passive Check
- REST
- NRDP

#### Properties

- [Git Hub](https://github.com/NagiosEnterprises/nrdp)
- [OpenAPI](openapi/nrdp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/nrdp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/nrdp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/nagios-check-result-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/nagios-check-result-structure.json)

### NSCA (Nagios Service Check Acceptor)

Encrypted binary TCP daemon (default port 5667) that accepts passive service/host check results from remote machines. Not REST — clients send tab-delimited records over a shared-secret-encrypted socket. Use NRDP for an HTTP/JSON equivalent.

- **Human URL:** [https://github.com/NagiosEnterprises/nsca](https://github.com/NagiosEnterprises/nsca)
- **Base URL:** `tcp://{nsca-host}:5667`

#### Tags

- Monitoring
- Passive Check
- Binary Protocol
- NSCA

#### Properties

- [Git Hub](https://github.com/NagiosEnterprises/nsca)
- [Postman Collection](collections/nagios-xi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/nagios-xi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ncpa.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ncpa.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/nrdp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/nrdp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### NRPE (Nagios Remote Plugin Executor)

Daemon that runs Nagios plugins on a remote Linux/Unix host on TCP port 5666, returning the plugin's exit code and output to the Nagios server. Binary protocol, not REST.

- **Human URL:** [https://github.com/NagiosEnterprises/nrpe](https://github.com/NagiosEnterprises/nrpe)
- **Base URL:** `tcp://{nrpe-host}:5666`

#### Tags

- Monitoring
- Active Check
- Binary Protocol
- NRPE

#### Properties

- [Git Hub](https://github.com/NagiosEnterprises/nrpe)
- [Postman Collection](collections/nagios-xi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/nagios-xi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ncpa.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ncpa.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/nrdp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/nrdp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.nagios.org)
- [Nagios  X I  Website](https://www.nagios.com/products/nagios-xi/)
- [Documentation](https://www.nagios.org/documentation/)
- [Nagios Library](https://library.nagios.com/docs/)
- [Support  Knowledgebase](https://support.nagios.com/kb/)
- [Pricing](https://www.nagios.com/products/pricing/)
- [Downloads](https://www.nagios.org/downloads/)
- [Nagios Exchange](https://exchange.nagios.org/)
- [GitHub Organization](https://github.com/NagiosEnterprises)
- [Source Repo](https://github.com/NagiosEnterprises/nagioscore)
- [Source Repo](https://github.com/NagiosEnterprises/ncpa)
- [Source Repo](https://github.com/NagiosEnterprises/nrpe)
- [Source Repo](https://github.com/NagiosEnterprises/nsca)
- [Source Repo](https://github.com/NagiosEnterprises/nrdp)
- [Source Repo](https://github.com/NagiosEnterprises/ndoutils)
- [Source Repo](https://github.com/NagiosEnterprises/nagios-mod-gearman)
- [Python S D K](https://github.com/NagiosEnterprises/napiv2)
- [SDK](https://github.com/NagiosEnterprises/automation)
- [Prometheus Exporter](https://github.com/NagiosEnterprises/nagprom)
- [Service Now Integration](https://github.com/NagiosEnterprises/NagiosXI-ServiceNow-EventHandler)
- [Pager Duty Integration](https://github.com/NagiosEnterprises/nagiosxi-pagerduty-handler)
- [V Mware Integration](https://github.com/NagiosEnterprises/NSXMon)
- [LinkedIn](https://www.linkedin.com/company/nagios-enterprises-llc)
- [License](https://github.com/NagiosEnterprises/nagioscore/blob/master/LICENSE)
- [Plans](plans/nagios-plans-pricing.yml)
- [Vocabulary](vocabulary/nagios-vocabulary.yml)
- [JSON-LD](json-ld/nagios-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
