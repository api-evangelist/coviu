---
name: Retrieve Coviu collection submissions and recordings
description: Walk a team's collections down to submission files and audio recordings for downstream clinical record-keeping.
api: openapi/coviu-rest-api-openapi.json
operations: [access-token, getCollections, listSubmissions, getSubmission, getSubmissionFile, getAudioRecording]
---

# Retrieve Coviu collection submissions and recordings

Use this to pull consultation artifacts (submissions, files, audio recordings) into a clinical record system.

## Auth
1. Get a bearer token via `access-token` (`POST /v1/auth/token`, `grant_type=client_credentials`).

## Steps
2. List the team's collections with `getCollections` (`GET /v1/collections/{teamId}`).
3. List submissions in a collection with `listSubmissions`
   (`GET /v1/collections/{teamId}/collection/{collectionId}`).
4. Read one submission with `getSubmission`
   (`GET /v1/collections/{teamId}/collection/{collectionId}/submission/{submissionId}`).
5. Download an attached file with `getSubmissionFile` (`.../file/{fileId}`) and an audio recording
   with `getAudioRecording` (`.../recording/{submissionId}`) — both return binary content.

## Rules
- List reads are paginated (offset/limit/page/page_size); a 206 Partial Content is returned for ranged reads.
- Recordings and submission files contain ePHI — handle per HIPAA/ISO 27001 obligations
  (see conformance/coviu-conformance.yml); do not log binary bodies.
