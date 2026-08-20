# Wei Sheng Lee — AI Implementation & Digital Transformation Proof

I turn ambiguous operational problems into controlled, testable working systems.

This repository is the public evidence layer for implementation work completed during my self-employed period under **Comnective Sphere Resources** and related delivery projects. I am **Wei Sheng Lee**, the owner/operator of Comnective Sphere Resources. The repository remains under `ComnectiveSR` to preserve project provenance and continuity with the source work.

It is built for hiring managers and clients who want to answer one question quickly:

> Can this person understand a messy workflow, decide what matters, implement a bounded change, verify that it works, and leave behind a system that another person can operate?

## 60-second proof

| What you need to know | Evidence |
|---|---|
| **Shipped product** | Live bilingual wedding invitation + RSVP system used for a real event: https://wilchi-weddinginvitation.pages.dev/ |
| **Inspectable source** | Public repository: https://github.com/ComnectiveSR/wilchi-wedding-invitation |
| **Real fault diagnosis** | MNavi provider-status failure: traced a frontend/backend contract mismatch, corrected the bounded interface, then re-tested the exact failure path. See `case-studies/MNAVI.md`. |
| **Verification discipline** | Endpoint tests **2/2 PASS**, component tests **11/11 PASS**, lint **PASS**, live backend probe **HTTP 200**, plus a negative secret-exposure check. See `evidence/MNAVI_PROVIDER_STATUS_REPAIR.md`. |
| **Operational judgment** | `HOW_I_WORK_WITH_AI.md` shows what I delegate to AI and what remains human-owned: problem selection, scope, acceptance, trade-offs, privacy, authority, and ship/no-ship decisions. |
| **Reusable method** | `TRANSFORMATION_PLAYBOOK.md` converts the work pattern into a repeatable workflow-diagnostic and implementation method that can be applied to customer operations. |

## What I can be used for

The strongest use of my background is at the boundary between **operations, customers, technology, and delivery**.

Typical problems:

- a business process depends on spreadsheets, messages, manual handoffs, or repeated checking;
- teams know a workflow is inefficient but cannot define what should be automated first;
- a digital or AI initiative exists as a demo but has not been converted into a reliable operating process;
- implementation is blocked by unclear requirements, ownership, data boundaries, testing, or adoption;
- a customer-facing technical project needs someone who can translate between users, commercial stakeholders, and builders;
- a change appears to work, but there is no acceptance evidence, rollback boundary, or guardrail against regressions.

My operating loop is:

**observe the real workflow → identify the costly failure → define outcome and boundaries → choose the smallest useful change → implement → verify with evidence → hand over an operable process → measure what changed**

AI is used as leverage inside that loop. It is not the product by default.

## What makes this different

The differentiation is the combination of:

**engineering background + customer-embedded delivery + commercial exposure + AI-assisted implementation + verification discipline**

My earlier work involved customer-site automation and AMHS implementation where physical constraints, downtime risk, user behavior, supplier coordination, and measurable outcomes mattered. The same implementation discipline now applies to digital workflows and AI-assisted systems.

I am not trying to compete as a frontier ML researcher or senior software architect. I compete on translating real operating problems into changes that can be implemented, tested, adopted, and explained.

## Proof cases

### 1. Shipped product — live bilingual RSVP system

This is a live product, not a mock-up.

Evidence includes:

- real users;
- guest and admin flows;
- deployment and release work;
- accessibility checks;
- live-friction fixes;
- change requests after use;
- public source code.

Live product: https://wilchi-weddinginvitation.pages.dev/  
Source: https://github.com/ComnectiveSR/wilchi-wedding-invitation

### 2. Fault-to-proof implementation — MNavi provider-status repair

**Observed failure:** the UI reported the local routing provider as unavailable even when the service was healthy.

**Root cause:** frontend `/api/provider-status` and backend `/provider-status` did not match; the proxy retained the `/api` prefix and returned 404.

**Decision:** fix the interface contract only. Do not expand into routing-engine installation, map data, credentials, telemetry, persistence, or unrelated architecture.

**Verification:** endpoint tests **2/2 PASS**, component tests **11/11 PASS**, lint **PASS**, live backend probe **HTTP 200**, plus a negative check that secret-shaped configuration was not exposed.

See `case-studies/MNAVI.md` and `evidence/MNAVI_PROVIDER_STATUS_REPAIR.md`.

### 3. Work-in-progress control patterns — TaxMY / InvoisMY

TaxMY and InvoisMY are **not presented as completed production products**.

Their useful evidence is narrower: they show how I structure evidence, validation, exception handling, human review, authority boundaries, and acceptance criteria in compliance-sensitive workflows.

They should be treated as work-in-progress implementation patterns, not as customer outcome proof.

## Reusable transformation package

The repository now includes `TRANSFORMATION_PLAYBOOK.md`.

It converts the proof into a practical engagement pattern:

1. map the current workflow;
2. quantify time, error, delay, risk, and revenue/cost impact;
3. identify the buyer, user, and owner;
4. rank intervention options by expected value and implementation risk;
5. define the smallest paid or production-relevant test;
6. implement inside an explicit scope boundary;
7. set primary and guardrail metrics before launch;
8. verify the result with tests, logs, screenshots, or operating evidence;
9. document the handover and next decision.

That method is intended to be reused for internal transformation teams, implementation consulting, solution delivery, and SME workflow improvement.

## AI versus human responsibility

AI assists:

- research;
- first-pass specifications;
- implementation support;
- testing;
- debugging;
- documentation;
- option generation.

I retain responsibility for:

- problem selection;
- customer and business context;
- scope and stop conditions;
- acceptance criteria;
- economics and trade-offs;
- privacy and authority boundaries;
- guardrail selection;
- final verification;
- ship/no-ship decisions.

See `HOW_I_WORK_WITH_AI.md`.

## Interview path

If you have five minutes, read:

1. `INTERVIEW_PROOF.md`
2. `case-studies/MNAVI.md`
3. `evidence/MNAVI_PROVIDER_STATUS_REPAIR.md`
4. `TRANSFORMATION_PLAYBOOK.md`
5. `HOW_I_WORK_WITH_AI.md`

For a live discussion, use `demo/FIVE_MINUTE_SCREEN_SHARE.md`.

## What this repository does not claim

I do **not** present myself as a senior ML engineer, enterprise architect, or frontier-model researcher.

My target roles are customer-facing **AI implementation, digital transformation, solution delivery, implementation consulting, technical operations, AI adoption, and governance execution** roles where technical understanding, stakeholder communication, commercial judgment, and verification matter together.

## Contact

**Wei Sheng Lee** — Kuala Lumpur, Malaysia  
LinkedIn: https://www.linkedin.com/in/heywilsonlee  
Email: hiwilsonlee@gmail.com
