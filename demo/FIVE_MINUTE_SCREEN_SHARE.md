# Five-Minute Interview Screen Share

Use the MNavi provider-status repair first unless another case is closer to the job.

## 0:00–0:30 — Positioning
“I use AI agents to increase implementation throughput. I keep problem selection, acceptance criteria, privacy/authority boundaries and consequential decisions under explicit human control.”

## 0:30–1:10 — The operational symptom
Show `case-studies/MNAVI.md`.

Explain:
- local routing service was healthy;
- UI still reported provider unavailable;
- the goal was to identify the real failure without widening scope.

## 1:10–2:10 — Root cause and correction
Show the route mismatch:
- frontend `/api/provider-status`;
- backend `/provider-status`;
- proxy retained the prefix and returned 404.

Explain why the fix was bounded rather than a routing-system redesign.

## 2:10–3:20 — Verification
Show `evidence/MNAVI_PROVIDER_STATUS_REPAIR.md`.

Call out:
- endpoint 2/2;
- component 11/11;
- lint;
- live HTTP 200 probe;
- safe response fields;
- negative check for secret-shaped fields.

## 3:20–4:10 — Human/agent boundary
Show `HOW_I_WORK_WITH_AI.md`.

Explain that the agent helped trace, implement and test, but was not allowed to self-declare success.

## 4:10–5:00 — Transfer to employer
Close with:
“This pattern transfers to customer implementation work: observe the real state, define the contract, make the smallest safe change, verify the exact path, preserve evidence, and stop when the proof passes.”

Then state the limitation: this case proves implementation discipline, not enterprise-scale architecture or ML engineering.
