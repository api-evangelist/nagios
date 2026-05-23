# Nagios

[apis.yml](apis.yml) profile for **Nagios**, the family of open-source and
commercial IT infrastructure monitoring tools maintained by Nagios
Enterprises, LLC: Nagios Core, Nagios XI, NCPA, NRPE, NSCA, NRDP, and a
broader ecosystem of plugins, integrations, and Nagios Exchange add-ons.

> "The Industry Standard in Open Source IT Monitoring Tools." — nagios.org

## APIs Indexed

| AID | Name | Surface | Protocol |
|---|---|---|---|
| `nagios:xi-rest-api` | Nagios XI REST API | `/nagiosxi/api/v1` | HTTP / JSON |
| `nagios:ncpa-api` | NCPA (Nagios Cross-Platform Agent) | `https://host:5693/api` | HTTPS / JSON |
| `nagios:nrdp-api` | NRDP (Nagios Remote Data Processor) | `/nrdp` | HTTP / XML or JSON |
| `nagios:nsca` | Nagios Service Check Acceptor | TCP 5667 | Encrypted binary |
| `nagios:nrpe` | Nagios Remote Plugin Executor | TCP 5666 | Binary |

The Nagios XI REST API is split into three sections: **Objects** (read-only
hosts/services/groups/contacts/downtime/history), **Config** (admin writes for
hosts and services), and **System** (apply config, scheduled downtime, status).

## Artifacts

| Folder | Files |
|---|---|
| [`openapi/`](openapi) | `nagios-xi-openapi.yml`, `ncpa-openapi.yml`, `nrdp-openapi.yml` |
| [`json-schema/`](json-schema) | `nagios-xi-host-schema.json`, `nagios-xi-service-schema.json`, `nagios-check-result-schema.json`, `ncpa-metric-schema.json` |
| [`json-structure/`](json-structure) | `nagios-xi-host-structure.json`, `nagios-check-result-structure.json` |
| [`json-ld/`](json-ld) | `nagios-context.jsonld` |
| [`examples/`](examples) | Request/response pairs for host create/delete, host & service status, system status, NCPA CPU & memory, NRDP submit |
| [`capabilities/`](capabilities) | Shared per-API (`nagios-xi`, `ncpa`, `nrdp`) plus workflow compositions (`incident-monitoring`, `host-lifecycle`) |
| [`rules/`](rules) | `nagios-xi-rules.yml`, `ncpa-rules.yml` Spectral rulesets |
| [`vocabulary/`](vocabulary) | `nagios-vocabulary.yml` |
| [`plans/`](plans) | `nagios-plans-pricing.yml` (Nagios XI Free / Standard / Enterprise / Sitewide) |

## Pricing (Nagios XI)

- **Free** — 7 nodes or 100 services, whichever is reached first.
- **Standard** — from $2,595 (100 nodes) up to $14,995 (1,000 nodes); 2,000+ nodes Contact Sales.
- **Enterprise** add-on — from $4,690 (100 nodes) up to $17,090 (1,000 nodes).
- **Sitewide** — Contact Sales, Enterprise features included.

Source: https://www.nagios.com/products/pricing/ (observed 2026-05-22).

Nagios Core, NCPA, NRPE, NSCA, NRDP, and the standard plugin set remain free
and open source (GPLv2/GPLv3 / MIT, depending on project).

## Key Repositories (github.com/NagiosEnterprises)

`nagioscore` (1,997 stars, C, GPLv2) · `nrpe` (274, C) · `ncpa` (203, Shell/Python) ·
`ndoutils` (52, C) · `nrdp` (51, PHP) · `nsca` (46, C) ·
`nagiosvshell` (34, PHP) · `nsti` (15, HTML) · `automation` (10, Python) ·
`nagiosbpi` (8, PHP) · `nagprom` (2, Python — Prometheus exporter) ·
`nagios-mod-gearman` (3, C) · `napiv2` (Python client for Nagios XI API v2).

## License and Governance

Nagios Core: **GPL-2.0**, maintained by Nagios Enterprises, LLC (commercial
backer of Nagios XI / Log Server / Network Analyzer / Fusion).
