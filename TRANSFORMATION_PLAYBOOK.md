# Transformation Playbook

A reusable method for converting a messy operating workflow into a bounded, measurable implementation.

This is not a claim that every step has already been sold as a consulting product. It is the operating method derived from shipped and in-progress implementation work in this repository.

## 1. Start from the workflow, not the tool

Capture:

- where work enters;
- who touches it;
- what information is required;
- where handoffs occur;
- what is repeated;
- what fails;
- what must remain human-controlled;
- how completion is proven.

Do not start with an AI feature list.

## 2. Quantify the current loss

Measure what can be measured:

- hours per week;
- wait time;
- rework;
- error frequency;
- support volume;
- missed revenue;
- cost of delay;
- compliance or operational risk.

If the problem cannot be connected to a material cost, risk, or customer outcome, it is usually not the first problem to automate.

## 3. Separate buyer, user, and owner

For each workflow identify:

- **Buyer:** who approves money or resources;
- **User:** who performs the work;
- **Owner:** who is accountable for the result;
- **Affected party:** who carries downside if the system is wrong.

Misalignment here is a common reason technically correct systems fail to get adopted.

## 4. Define the outcome before the solution

Write one measurable target.

Example:

> Reduce manual exception triage from 6 hours per week to under 2 hours without increasing unresolved-error rate above the agreed threshold.

Then define what must not break.

## 5. Rank intervention options by expected value

Compare options using:

- success probability;
- upside;
- implementation time;
- required resources;
- operational risk;
- reversibility;
- future reuse.

The best answer may be process redesign, a rule, a form, an integration, a script, an AI-assisted step, or full automation.

## 6. Choose the smallest meaningful test

The first implementation should be large enough to produce decision-grade evidence and small enough to reverse.

Define:

- exact scope;
- permitted systems/files;
- expected proof;
- stop condition;
- rollback boundary.

Do not expand scope because an adjacent opportunity looks interesting.

## 7. Set primary and guardrail metrics before launch

### Primary metric

What should improve?

Examples:

- completion time;
- conversion;
- error rate;
- cases processed;
- support load;
- revenue per workflow.

### Guardrails

What must not become materially worse?

Examples:

- error severity;
- AOV or margin;
- response latency;
- support tickets;
- unresolved exceptions;
- privacy exposure;
- user adoption;
- manual recovery time.

Set rollback thresholds before seeing results.

## 8. Implement with explicit authority boundaries

Decide what the system may:

- read;
- suggest;
- write;
- approve;
- send;
- delete;
- escalate.

Consequential actions should not be delegated implicitly.

## 9. Verify the actual failure path

Verification may include:

- automated tests;
- live endpoint probes;
- screenshots;
- logs;
- structured UI state;
- negative tests;
- operator walkthroughs;
- reconciliation against source evidence.

A build passing is not the same as the workflow working.

## 10. Handover an operable system

Leave behind:

- operating steps;
- owner;
- exception path;
- failure and rollback procedure;
- metric definitions;
- evidence location;
- known limitations;
- next review point.

The implementation is not complete if only the builder can operate it.

## 11. Decide what happens next

After the test, choose one:

- scale;
- refine;
- hold;
- roll back;
- kill.

Use actual evidence. Do not keep a project alive because of sunk cost.

## Compact diagnostic output

A useful first engagement can produce one page with:

| Field | Output |
|---|---|
| Workflow | Exact process being examined |
| Current loss | Time, money, error, delay, or risk |
| Buyer / user / owner | Named roles |
| Bottleneck | Highest-value failure point |
| Proposed intervention | Smallest useful change |
| Primary metric | What should improve |
| Guardrails | What must not get worse |
| Proof | Test, log, screenshot, reconciliation, or live result |
| Rollback | How to reverse safely |
| Next decision | Scale / refine / stop |

This structure can be used for internal transformation work, implementation consulting, solution delivery, AI adoption, and SME workflow improvement.
