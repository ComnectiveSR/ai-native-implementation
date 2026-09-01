# AGENTS.md

This repository uses evidence-first, bounded implementation.

## 1. Preflight before editing
Read the target files, current acceptance contract, current branch or head, existing tests and relevant evidence. Do not assume a requested object, file, state or capability exists.

## 2. Keep scope bounded
Change only what the current observed failure or acceptance gap requires. Do not widen product scope while an acceptance path is failing.

## 3. Remove and simplify before adding
Prefer existing components, connectors, APIs and CLIs. Add a dependency, framework, browser/session automation layer or new agent only when a verified recurring gap justifies it.

## 4. Treat design as a constraint system
For structural UI or workflow changes, write the constraints first. When practical, compare 3–4 bounded variants outside production before choosing one. Reuse components, remove clutter and verify desktop plus 390px when the product is responsive.

## 5. Define proof before implementation
A task is not complete because an agent reports PASS. Use the proof appropriate to the change: automated tests, schema checks, browser or DOM checks, screenshots, source verification, synthetic fixtures, measured before/after evidence or human acceptance.

## 6. Preserve authority boundaries
Never hardcode or expose secrets. Do not perform unsupervised sends, deployments, payments, destructive writes or other consequential external actions unless the current task explicitly authorizes them. Keep human approval where consequence or reversibility requires it.

## 7. Run the closed loop
Observe -> Quantify -> Decide -> Implement -> Verify -> Handover.

When verification fails, fix the first observed failure and its adjacent regression, then re-run the exact failing path. Do not respond to failure with conceptual redesign unless the evidence changes a governing constraint.

## 8. Measure operating value
For workflow changes, preserve a named owner, baseline, new operating path, operating measure, outcome measure, quality guard and stop or rollback condition. Do not describe estimated impact as verified ROI.

## 9. Promote learning only after verification
Record only durable learning that has earned promotion into a test, skill, template, checklist, architecture pattern or decision rule. Tool discovery and internet case studies are inputs to evaluate, not backlog items.
