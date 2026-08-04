# Blackrock Neurotech

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
