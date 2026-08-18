# Case Study — MNavi Provider-Status Repair

## 1. Operating problem

A local-routing Live Pilot showed the provider as unavailable even when the approved local GraphHopper routing service was healthy.

The risk was not only a broken UI. A readiness screen that infers status incorrectly can cause an operator to make the wrong deployment or pilot decision.

## 2. Observed failure

The frontend requested:

`/api/provider-status`

The backend exposed:

`/provider-status`

The Vite proxy preserved the `/api` prefix. The result was a 404, which pushed the UI into its disabled fallback state.

## 3. Bounded correction

The repair stayed inside the provider-readiness boundary.

Changes:
- backend accepts `/provider-status` and `/api/provider-status`;
- readiness payload is built through one bounded helper;
- frontend reads explicit safe fields such as provider enabled state, routing provider, URL validity and engine health;
- the response does not expose raw provider URLs, token environment names or other secret-shaped configuration.

No routing-engine installation, map data, credentials, telemetry, persistence, deployment, lane logic or unrelated architecture was added.

## 4. Verification

The repair was not accepted on code inspection alone.

Evidence:
- provider-status endpoint tests: **2/2 PASS**;
- Live Pilot component tests: **11/11 PASS**;
- lint: **PASS**;
- local backend live probe: **HTTP 200**;
- routing provider observed: `graphhopper-local`;
- map provider observed: `local-osm`;
- map/routing URL checks: true;
- engine health: healthy;
- route request budget: `0 / 1`;
- secret-shaped fields: not present.

Commit:
`57e149e5fc9c60c46bc695342c7a798d456d6b86`

## 5. What AI did and did not do

AI-assisted development was used to accelerate route tracing, implementation, test creation and verification work.

AI did not define completion.

Completion required observable evidence:
- exact failure mechanism;
- bounded scope;
- deterministic tests;
- live endpoint probe;
- explicit safety check;
- no adjacent-scope expansion.

## 6. What this proves

This case demonstrates:
- debugging from observed runtime state rather than assumption;
- translating a vague “provider disabled” symptom into a concrete interface-contract failure;
- targeted implementation rather than broad rewrite;
- deterministic verification plus live-state verification;
- explicit data-exposure boundaries;
- clear stop conditions.

## 7. Limitations

This does not prove:
- large-scale production traffic;
- paid-provider performance;
- customer adoption;
- ML-model development;
- enterprise architecture ownership.

It is evidence of implementation judgment, agent-assisted execution and verification discipline.
