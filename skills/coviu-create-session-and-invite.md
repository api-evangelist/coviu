---
name: Create a Coviu session and invite a participant
description: Authenticate, create a video consultation session, add a guest participant, and share their join link.
api: openapi/coviu-rest-api-openapi.json
operations: [access-token, createSession, addParticipant, getParticipant]
---

# Create a Coviu session and invite a participant

Use this to stand up a telehealth video consultation and hand a patient a join link.

## Auth
1. Obtain an OAuth2 access token via `access-token` (`POST /v1/auth/token`). Send HTTP Basic auth
   (Client ID as username, Client Secret as password) with `application/x-www-form-urlencoded`
   body `grant_type=client_credentials`. Use the returned bearer token on every subsequent call.

## Steps
2. Create the session with `createSession` (`POST /v1/sessions`). Optionally pass `feature_flags`
   to customise the room (exit/return URLs, disable menu, enforce participant uniqueness).
3. Add the patient with `addParticipant` (`POST /v1/sessions/{session_id}/participants`), setting
   their name, role (host/guest), and avatar. The response includes the participant join link.
4. Optionally re-read the participant with `getParticipant` (`GET /v1/participants/{participant_id}`)
   to confirm the join link and status before sending it.

## Rules
- No idempotency key is supported; do not blindly retry `createSession`/`addParticipant` — on a
  timeout, `listSessions` to check whether the session already exists before retrying.
- A session that has already finished cannot accept new participants; a started session cannot be cancelled.
- Errors surface as HTTP status codes (400/401/403/404); there is no problem+json envelope
  (see errors/coviu-problem-types.yml).
