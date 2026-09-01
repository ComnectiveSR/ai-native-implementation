# AGENTS.md

This repository uses evidence-first, bounded implementation.

## 1. Preflight before editing
Read the target files, current acceptance contract, current branch or head, existing tests and relevant evidence. Do not assume a requested object, file, state or capability exists.

## 2. Classify external evidence before using it
Treat articles, screenshots, social posts, newsletters, vendor claims and case studies as hypotheses until verified. Record what is FACT, HYPOTHESIS, CONTRADICTION or UNSUPPORTED. Do not encode a viral claim into product logic, strategy or public copy without stronger evidence.

## 3. Keep scope bounded
Change only what the current observed failure or acceptance gap requires. Do not widen product scope while an acceptance path is failing.

## 4. Remove and simplify before adding
Prefer existing components, connectors, APIs and CLIs. Add a dependency, framework, browser/session automation layer or new agent only when a verified recurring gap justifies it.

## 5. Treat design as a constraint system
For structural UI or workflow changes, write the constraints first. When practical, compare 3–4 bounded variants outside production before choosing one. Reuse components, remove clutter and verify desktop plus 390px when the product is responsive.

## 6. Define proof before implementation
A task is not complete because an agent reports PASS. Use the proof appropriate to the change: automated tests, schema checks, browser or DOM checks, screenshots, source verification, synthetic fixtures, measured before/after evidence or human acceptance.

## 7. Preserve authority boundaries
Never hardcode or expose secrets. Do not perform unsupervised sends, deployments, payments, destructive writes or other consequential external actions unless the current task explicitly authorizes them. Keep human approval where consequence or reversibility requires it.

## 8. Run the closed loop
Observe -> Quantify -> Decide -> Implement -> Verify -> Handover.

When verification fails, fix the first observed failure and its adjacent regression, then re-run the exact failing path. Do not respond to failure with conceptual redesign unless the evidence changes a governing constraint.

## 9. Measure operating value
For workflow changes, preserve a named owner, baseline, new operating path, operating measure, outcome measure, quality guard and stop or rollback condition. Do not describe estimated impact as verified ROI.

## 10. Protect expected-value discipline
If a task concerns a lead, offer, partnership, job or commercial opportunity, do not optimize for headline revenue alone. Surface evidence strength, access/warmth, cash probability, strategic fit, repeatability, delivery burden, scope risk, payment quality, reversibility and learning/career capital. Preserve a power-law exception only when downside is bounded and information gain is high.

## 11. Keep claims buyer-observable
For business-facing copy, prefer measurable transition language: consequence, pain removed, time/risk reduced, capability gained, proof and next action. Avoid identity-heavy or emotional claims that are not observable or falsifiable.

## 12. Promote learning only after verification
Record only durable learning that has earned promotion into a test, skill, template, checklist, architecture pattern or decision rule. Tool discovery and internet case studies are inputs to evaluate, not backlog items.
