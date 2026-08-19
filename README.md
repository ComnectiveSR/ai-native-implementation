# Wei Sheng Lee — AI Implementation & Digital Transformation Proof

I turn ambiguous operational problems into verifiable working systems.

This repository is a public, sanitized evidence layer for my work under **Comnective Sphere Resources** and related implementation projects. It is designed for hiring managers and clients who want to see shipped work, technical judgment, verification discipline, and clear limits — not generic claims of being “AI-native”.

## 60-second proof

| Question | Evidence |
|---|---|
| **Have you shipped something real?** | Live bilingual wedding invitation + RSVP product used for a real event: https://wilchi-weddinginvitation.pages.dev/ |
| **Can you show source?** | Public source: https://github.com/ComnectiveSR/wilchi-wedding-invitation |
| **Can you debug a real failure?** | MNavi provider-status case: observed 404 → traced frontend/backend contract mismatch → bounded correction → automated tests + live probe + negative data-exposure check. See `case-studies/MNAVI.md`. |
| **Do you know what AI should not decide?** | `HOW_I_WORK_WITH_AI.md` separates AI acceleration from human ownership of problem selection, scope, acceptance, privacy/authority boundaries, and final ship decisions. |
| **Can you work in compliance-heavy environments?** | TaxMY/InvoisMY cases use explicit evidence, exception, human-review, fail-safe and authority boundaries. See `PROOF_MATRIX.md`. |
| **Can you explain failures and trade-offs?** | `INTERVIEW_PROOF.md` answers six AI-era interview questions using shipped work, including what broke, what was cut, and where I overrode the tool. |

## What I actually do

My strongest role is not “prompt engineer” or pure software engineer. I work at the boundary between operations, customers, technology, and delivery:

**observe the real workflow → find the important problem → define the contract → use AI for leverage → implement narrowly → verify the result → keep consequential authority explicit → capture the learning**

That operating pattern comes from earlier customer-embedded engineering and AMHS delivery, and now extends into digital products, compliance-heavy workflows, and AI-assisted implementation.

## Proof cases

### 1. Shipped product — live bilingual RSVP system

**Why it matters:** this is not a mock-up. It went through release packaging, guest/admin flow testing, accessibility checks, live-friction fixes, and real-user operation.

- Live product: https://wilchi-weddinginvitation.pages.dev/
- Public source: https://github.com/ComnectiveSR/wilchi-wedding-invitation
- Interview summary: `INTERVIEW_PROOF.md`

### 2. Implementation judgment — MNavi provider-status repair

**Observed failure:** the UI reported the local routing provider as unavailable even when the service was healthy.

**Root cause:** frontend `/api/provider-status` and backend `/provider-status` did not match; the proxy retained the `/api` prefix and returned 404.

**Bounded correction:** fix the interface contract without expanding into routing-engine installation, map data, credentials, telemetry, persistence, or unrelated architecture.

**Verification:** endpoint tests **2/2 PASS**, component tests **11/11 PASS**, lint **PASS**, live backend probe **HTTP 200**, plus a negative check that secret-shaped configuration was not exposed.

See `case-studies/MNAVI.md` and `evidence/MNAVI_PROVIDER_STATUS_REPAIR.md`.

### 3. Control and governance — TaxMY / InvoisMY

These projects are useful because they force explicit decisions about:

- source evidence;
- deterministic validation;
- exceptions and failure states;
- human approval;
- privacy boundaries;
- production authority;
- truthful claims;
- acceptance evidence.

They are not presented as proof of regulatory approval or enterprise-scale production adoption.

## AI versus human responsibility

AI assists research, first-pass specifications, implementation support, testing, debugging, and documentation.

I retain responsibility for:

- problem selection;
- user and business context;
- scope and stop conditions;
- acceptance criteria;
- privacy and authority boundaries;
- trade-offs and guardrails;
- final verification and ship/no-ship decisions.

See `HOW_I_WORK_WITH_AI.md`.

## Interview path

If you have five minutes, read in this order:

1. `INTERVIEW_PROOF.md`
2. `case-studies/MNAVI.md`
3. `evidence/MNAVI_PROVIDER_STATUS_REPAIR.md`
4. `HOW_I_WORK_WITH_AI.md`
5. `PROOF_MATRIX.md`

For a live discussion, `demo/FIVE_MINUTE_SCREEN_SHARE.md` is the walkthrough I use.

## What this repository does not claim

I do **not** present myself as a senior ML engineer, enterprise architect, or frontier-model researcher.

My current target is customer-facing **AI implementation, digital transformation, solution delivery, implementation consulting, and AI adoption/governance execution** — roles where technical understanding, stakeholder communication, commercial judgment, and verification matter together.

## Contact

**Wei Sheng Lee** — Kuala Lumpur, Malaysia  
LinkedIn: https://www.linkedin.com/in/heywilsonlee  
Email: hiwilsonlee@gmail.com
