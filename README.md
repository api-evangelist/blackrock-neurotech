# Blackrock Neurotech

Blackrock Neurotech is a Salt Lake City, Utah based neurotechnology company that designs and manufactures implantable brain-computer interface (BCI) systems and the research instrumentation around them — Utah Array microelectrode arrays and the Neuralace interface, the NeuroPort / Cerebus / CerePlex Direct neural signal processors, the CereStim stimulation system, and the Central software suite for acquisition, visualization and offline spike sorting.

- Website: https://blackrockneurotech.com/
- Products: https://blackrockneurotech.com/products/
- Software: https://blackrockneurotech.com/products/software/
- Support: https://blackrockneurotech.com/support/
- Knowledge base: https://support.blackrockneurotech.com/portal/en/kb/support
- GitHub: https://github.com/BlackrockNeurotech
- News: https://blackrockneurotech.com/news/

## API surface

Blackrock Neurotech publishes **no public web API**. Its programmatic surface is a set of
device and file-format libraries distributed as GitHub source and as IFU-numbered downloads:

- **cbSDK** — C++ API for real-time interfacing with Blackrock neural signal processors
- **cbMEX** — NSP MATLAB API (IFU LB-0590 Rev 3.00)
- **CereStim API** — stimulation system API (v5.3.0, IFU 0900 Rev 4.00)
- **brPY / brpylib** — Python data loader ([Python-Utilities](https://github.com/BlackrockNeurotech/Python-Utilities))
- **NPMK** — Neural Processing Matlab Kit ([NPMK](https://github.com/BlackrockNeurotech/NPMK))
- **BOSS** — Blackrock Offline Spike Sorter source
- **aqnwb** — C++ acquisition API for the NWB format

CereLink and br_stimpy are community projects; Blackrock's knowledge base states CereLink
is not Blackrock-supported.

## Enrichment (2026-08-02)

Probed and confirmed absent on every Blackrock host: OpenAPI/Swagger, GraphQL, AsyncAPI,
gRPC/protobuf, MCP server, A2A agent card, `llms.txt`, and all `/.well-known/` discovery
documents. No `api.`, `developer.`, `docs.`, `mcp.` or `trust.` subdomain resolves. No
status page, no vulnerability-disclosure program, no trust center.

Artifacts in this repo:

- `packages/` — first-party client libraries and device APIs, plus registry probe results
- `well-known/` — negative probe record for every `/.well-known/` path on every host
- `llms/` — generated `llms.txt` for the company
- `lifecycle/` — product/IFU release versioning surface
- `security/` — probed domain security posture (TLS/HSTS/DNSSEC/CAA/SPF/DMARC)
