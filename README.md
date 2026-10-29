# Coviu

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

Coviu is an Australian telehealth company, headquartered in Sydney and spun out of CSIRO's Data61, that provides a purpose-built video consultation platform for healthcare providers, allied health, and enterprise clinical networks. Its browser-based, WebRTC video calling supports virtual care workflows including waiting rooms, in-call clinical tools, screen and file sharing, medical device integrations, and payments. For developers, Coviu ships a secure OAuth2-protected REST API (base https://api.coviu.com) that lets applications create and manage video consultation Sessions and Participants, monitor Waiting Area queues in real time, retrieve Collections (submissions, files, and audio recordings), and receive event Webhooks, plus an in-call Plugin API and embedded iframe mode. Coviu is a telehealth video/interoperability layer rather than an EHR or FHIR data platform, so its documented public surface is REST + webhooks, not HL7 FHIR.

**Areas:** Healthcare · Telehealth · Australia · Virtual Care · Video · WebRTC · Appointments · Remote Monitoring · REST

## Coviu on APIs.io

Everything profiled for Coviu is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/coviu/](https://apis.io/providers/coviu/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [Coviu Plugin API](https://apis.io/apis/coviu/coviu-plugin-api/) — In-call Plugin (Apps) API for building custom experiences inside the Coviu video room — adding UI elements, connecting to third-party systems, and enriching…
- [Coviu Auth API](https://apis.io/apis/coviu/coviu-auth-api/) — The Auth API from Coviu — 1 operation(s) for auth.
- [Coviu Collections API](https://apis.io/apis/coviu/coviu-collections-api/) — The Collections API from Coviu — 5 operation(s) for collections.
- [Coviu Participants API](https://apis.io/apis/coviu/coviu-participants-api/) — The Participants API from Coviu — 2 operation(s) for participants.
- [Coviu Sessions API](https://apis.io/apis/coviu/coviu-sessions-api/) — The Sessions API from Coviu — 3 operation(s) for sessions.
- [Coviu Waiting Area API](https://apis.io/apis/coviu/coviu-waiting-area-api/) — The Waiting Area API from Coviu — 3 operation(s) for waiting area.
- [Coviu Webhook Requests API](https://apis.io/apis/coviu/coviu-webhook-requests-api/) — The Webhook Requests API from Coviu — 1 operation(s) for webhook requests.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Coviu Webhooks](https://apis.io/asyncapis/coviu/coviu-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [coviu](https://apis.io/servers/coviu/coviu/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Coviu Agentic Access](https://apis.io/agentic-access/coviu/coviu-agentic-access/)

#### Collections (1)

Postman and Open Collection request collections.

- [Coviu REST API](https://apis.io/collections/coviu/open-coviu-rest-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Coviu Rest Api Overlay](https://apis.io/overlays/coviu/coviu-rest-api-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Coviu Authentication](https://apis.io/security/coviu/coviu-authentication/)
- [Coviu Domain Security](https://apis.io/security/coviu/coviu-domain-security/)
- [Coviu Trust Center](https://apis.io/security/coviu/coviu-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Coviu Scopes](https://apis.io/scopes/coviu/coviu-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.coviu.com/)
- [Documentation](https://coviu.readme.io/reference/the-coviu-rest-api)
- [Getting started](https://coviu.readme.io/reference/getting-started-with-your-api-1)
- [API reference](https://coviu.readme.io/reference/the-coviu-rest-api)
- [Pricing](https://www.coviu.com/en-au/pricing)
- [Sign up](https://signup.coviu.com/)
- [Support](https://help.coviu.com/)
- [Blog](https://www.coviu.com/blog)
- [Compliance](https://www.coviu.com/en-au/compliance-and-security)
- [Terms of service](https://www.coviu.com/terms)
- [Privacy policy](https://www.coviu.com/en-au/privacy-policy)
- [GitHub](https://github.com/coviu)
- [Status](https://status.coviu.com/)

## API Evangelist rating

**Kin Score 48.0** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 64.3 |
| Contract quality | 51.2 |
| Contract governance | 18.2 |
| Operational transparency | 18.4 |
| Developer ergonomics | 45.4 |
| Access clarity | 60.5 |

**Agent readiness 30.7** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 36.7** — Health

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/coviu/](https://apis.io/providers/coviu/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Coviu: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/coviu/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
