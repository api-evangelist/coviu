# Coviu (coviu)

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

Coviu is an Australian telehealth company (Sydney; spun out of CSIRO's Data61) providing a purpose-built, browser-based video consultation platform for healthcare and allied-health providers. For developers, Coviu exposes an OAuth2-protected REST API at `https://api.coviu.com` for creating and managing video consultation Sessions and Participants, monitoring Waiting Area queues, retrieving Collections (submissions, files, and audio recordings), and receiving event Webhooks — plus an in-call Plugin (Apps) API and embedded iframe mode. Coviu is a telehealth video/interoperability layer, not an EHR or HL7 FHIR data platform; its documented public surface is REST + webhooks.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/apis.yml)

## Tags

- Healthcare
- Telehealth
- Australia
- Virtual Care
- Video
- WebRTC
- Appointments
- Remote Monitoring
- REST

## Timestamps

- **Created:** 2026-07-24
- **Modified:** 2026-07-24

## APIs

### Coviu Sessions API

Create, list, retrieve, update, and cancel Coviu video consultation Sessions, and pull a Session Summary with participant entry/exit timing.

- **Human URL:** [https://coviu.readme.io/reference/sessions](https://coviu.readme.io/reference/sessions)
- **Base URL:** `https://api.coviu.com/v1`

#### Properties

- [OpenAPI](openapi/coviu-rest-api-openapi.json)
- [Documentation](https://coviu.readme.io/reference/sessions)
- [API Reference](https://coviu.readme.io/reference/createsession)
- [Authentication](https://coviu.readme.io/reference/access-token)

### Coviu Participants API

List, add, retrieve, update, and cancel Participants on a Session, controlling per-participant join links, names, avatars, and host/guest roles.

- **Human URL:** [https://coviu.readme.io/reference/listparticipants](https://coviu.readme.io/reference/listparticipants)
- **Base URL:** `https://api.coviu.com/v1`

### Coviu Waiting Area API

Read the Waiting Area in real time — currently waiting calls for a team, waiting calls for a queue, and individual call detail — for virtual reception and triage.

- **Human URL:** [https://coviu.readme.io/reference/getcurrentlywaitingcalls](https://coviu.readme.io/reference/getcurrentlywaitingcalls)
- **Base URL:** `https://api.coviu.com/v1`

### Coviu Collections API

Retrieve a team's Collections and their Submissions, including submission files and audio recordings captured during consultations.

- **Human URL:** [https://coviu.readme.io/reference/collections](https://coviu.readme.io/reference/collections)
- **Base URL:** `https://api.coviu.com/v1`

### Coviu Webhooks

Real-time event notifications delivered as HTTP POST callbacks to a URL you configure, firing when relevant Coviu events occur (e.g. patient arrival, call conclusion).

- **Human URL:** [https://coviu.readme.io/reference/webhooks-documentation](https://coviu.readme.io/reference/webhooks-documentation)

### Coviu Plugin API

In-call Plugin (Apps) API for building custom experiences inside the Coviu video room — adding UI elements and connecting to third-party systems.

- **Human URL:** [https://coviu.readme.io/reference/getting-started-with-your-api-1](https://coviu.readme.io/reference/getting-started-with-your-api-1)

## Common Properties

- [Website](https://www.coviu.com/)
- [Developer Portal](https://coviu.readme.io/)
- [Documentation](https://coviu.readme.io/reference/the-coviu-rest-api)
- [Getting Started](https://coviu.readme.io/reference/getting-started-with-your-api-1)
- [GitHub Organization](https://github.com/coviu)
- [LinkedIn](https://www.linkedin.com/company/coviu)
- [Status Page](https://status.coviu.com/)
- [Pricing](https://www.coviu.com/en-au/pricing)
- [Blog](https://www.coviu.com/blog)
- [Support](https://help.coviu.com/)
- [Terms of Service](https://www.coviu.com/terms)
- [Privacy Policy](https://www.coviu.com/en-au/privacy-policy)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
