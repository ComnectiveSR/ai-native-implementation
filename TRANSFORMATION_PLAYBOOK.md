# Workflow Transformation Diagnostic — Public Preview

This page shows enough of my operating method for a hiring manager or prospective client to understand how I approach transformation work.

It is intentionally **not** the full commercial delivery playbook. Detailed scoring logic, discovery prompts, qualification thresholds, implementation templates, commercial assumptions, customer-specific decision rules, and internal operating assets are retained for live engagements.

The principle is simple:

> Start with the operating problem. Measure the loss. Improve the system. Use AI only where it creates positive expected value. Verify the result before scaling.

## 1. Map the real workflow

Capture where work enters, who touches it, where handoffs occur, what information is required, where rework happens, what fails, and how completion is currently proven.

Do not begin with an AI feature list.

## 2. Quantify the current loss

Estimate the material consequence of the current workflow, such as:

- staff hours consumed;
- waiting time;
- rework;
- error frequency;
- support burden;
- missed revenue;
- cost of delay;
- compliance or operational risk.

A problem with no meaningful economic, customer, or risk consequence is usually not the first problem to automate.

## 3. Identify buyer, user, owner, and affected party

A technically correct system can still fail when incentives or accountability are unclear.

For every workflow, identify who pays, who uses the process, who owns the outcome, and who carries the downside when it fails.

## 4. Define what good looks like before building

Set one measurable improvement target and the conditions that must not become materially worse.

Example:

> Reduce manual exception triage while holding unresolved-error rate below the agreed threshold.

The exact target, baseline and guardrails must be established from real operating evidence.

## 5. Choose the smallest useful intervention

The right answer may be:

- remove a step;
- clarify ownership;
- redesign a form;
- standardise an input;
- add a deterministic rule;
- connect two systems;
- add AI assistance;
- automate a bounded task;
- or leave the step human-controlled.

The goal is not maximum automation. It is maximum expected value after implementation cost, failure risk, adoption friction and ongoing operating cost.

## 6. Build within explicit authority boundaries

Before implementation, decide what the system may read, suggest, write, approve, send, delete or escalate.

High-impact actions need named human accountability, review thresholds, logging, escalation and rollback.

## 7. Verify the real user outcome

Evidence may include tests, logs, screenshots, endpoint probes, reconciliation against source data, operator walkthroughs, before/after measurements and user acceptance.

**Built ≠ working. Working ≠ usable. Usable ≠ valuable.**

## 8. Decide: scale, refine or stop

A bounded test should end with a business decision, not an endless improvement loop.

Scale only when evidence supports it. Otherwise refine, hold, roll back or kill the intervention.

## What a first diagnostic produces

A first engagement should leave the customer with a decision-ready summary rather than an AI demo.

| Output | Purpose |
|---|---|
| Workflow map | Shows the current operating path |
| Baseline loss | Quantifies time, money, delay, error or risk |
| Bottleneck | Identifies the highest-value failure point |
| Buyer / user / owner map | Makes accountability and adoption explicit |
| Intervention options | Separates process, rule, integration and AI choices |
| Expected-value case | Tests whether improvement is worth implementing |
| Primary metric + guardrails | Defines what good looks like and what must not break |
| Proof plan | States how the result will be verified |
| Next decision | Implement / pilot / hold / stop |

## Free-filter → paid implementation model

The public diagnostic can be used as a low-friction qualification layer before implementation work:

1. **Free workflow screen** — determine whether a material repeated problem exists.
2. **Decision-grade diagnostic** — establish baseline, bottleneck, economics, risks and implementation options.
3. **Bounded pilot** — test the highest-EV intervention on a controlled slice.
4. **Implementation** — integrate the proven change into the operating workflow.
5. **Measurement and handover** — verify cost, revenue, speed, quality or risk impact and make the process operable without the builder.

The diagnostic is useful even when the correct answer is **do not automate**.

## What remains private

The public repository proves judgment and implementation discipline. It does not publish the full commercial system.

Private engagement assets include detailed discovery scripts, scoring weights, qualification thresholds, pricing logic, customer-specific economics, internal prompts, reusable implementation templates, account-specific data mappings, security details and proprietary delivery shortcuts.

A buyer should be able to understand **how I think and what evidence I require** without receiving every implementation asset required to reproduce the service independently.
