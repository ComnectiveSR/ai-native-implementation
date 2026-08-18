# How I Work With AI

## 1. Shape the build
I start with the operating problem, user, constraints, acceptance criteria and failure modes before choosing tools.

## 2. Use agents as leverage
I use ChatGPT, Claude and Codex for research, specifications, implementation assistance, testing and documentation. Tool choice follows the task; I do not optimize for allegiance to one model.

## 3. Keep high-risk rules deterministic
Permissions, privacy boundaries, acceptance gates and irreversible actions should not depend on a model deciding to behave correctly.

## 4. Verify
A task is not complete because an agent says it is complete. I require the appropriate proof: automated tests, schema validation, screenshots, browser/DOM checks, synthetic fixtures, source checks or human acceptance.

## 5. Correct narrowly
When proof fails, fix the observed failure and adjacent regression, then re-run the exact failing path.

## 6. Record learning
A project should leave a reusable primitive: a skill, test, template, architecture pattern, checklist or decision rule.
