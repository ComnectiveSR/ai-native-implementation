# Evidence Note — MNavi Provider-Status Repair

## Evidence chain

| Stage | Evidence |
|---|---|
| Symptom | Live Pilot fell back to provider-disabled state |
| Root cause | frontend `/api/provider-status` vs backend `/provider-status`; proxy preserved prefix |
| Repair | bounded dual route + explicit safe readiness payload |
| Automated verification | endpoint 2/2 PASS; component 11/11 PASS; lint PASS |
| Runtime verification | local backend probe HTTP 200 |
| Safety verification | no raw URLs, token environment name, or secret-shaped fields in payload |
| Scope verification | no engine install, map data, credentials, telemetry, persistence or deployment change |
| Commit | `57e149e5fc9c60c46bc695342c7a798d456d6b86` |

## Why this evidence matters

A model saying “the route is fixed” is not proof.

The proof is the combination of:
1. a reproduced failure;
2. an explicit root cause;
3. a narrow correction;
4. automated checks;
5. a live-state check;
6. a negative safety check.

This is the pattern I reuse for AI-assisted implementation work.
