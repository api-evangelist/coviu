# Coviu (coviu)

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
