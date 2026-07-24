---
name: Monitor the Coviu waiting area
description: Poll a team's waiting area for arriving patients and inspect individual waiting calls for virtual reception and triage.
api: openapi/coviu-rest-api-openapi.json
operations: [access-token, getCurrentlyWaitingCalls, getCurrentlyWaitingCallsForQueue, getCall]
---

# Monitor the Coviu waiting area

Use this to build a virtual reception / triage view over patients waiting to be seen.

## Auth
1. Get a bearer token via `access-token` (`POST /v1/auth/token`, `grant_type=client_credentials`,
   Client ID/Secret as HTTP Basic).

## Steps
2. List everyone currently waiting for the team with `getCurrentlyWaitingCalls`
   (`GET /v1/waiting/{teamId}`).
3. For a specific reception queue, use `getCurrentlyWaitingCallsForQueue`
   (`GET /v1/waiting/{teamId}/queue/{waitingQueueId}`).
4. Drill into one waiting call with `getCall` (`GET /v1/waiting/{teamId}/calls/{callId}`).

## Rules
- These are read-only endpoints; poll on an interval, or prefer the webhook surface
  (WaitingAreaJoin / WaitingAreaAnswer / WaitingAreaLeave — see asyncapi/coviu-webhooks.yml) for
  push notification instead of tight polling.
- Webhooks are delivered at-most-once with no retry; make your receive handler idempotent.
