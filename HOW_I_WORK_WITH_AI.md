# How I Work With AI

## 1. Observe before building
I start with the real work, user, operating problem, baseline, constraints, failure modes, authority boundaries and acceptance criteria before choosing tools. AI is not the default intervention.

## 2. Design the whole system
I treat feedback first as either a changed constraint or a local papercut. For structural UI or workflow changes, I explore several bounded alternatives before editing production when practical. I prefer reusable components and remove unnecessary elements before adding more.

## 3. Use agents as leverage
I use ChatGPT, Claude and Codex for research, specifications, implementation assistance, testing and documentation. Tool choice follows the process. New tools remain experiments until a repeated gap justifies them. I prefer native connectors, APIs and CLIs over fragile browser automation.

## 4. Keep authority deterministic
Permissions, privacy boundaries, consequential claims, acceptance gates, external writes and irreversible actions must not depend on a model deciding to behave correctly. Human approval remains required where consequence or reversibility demands it.

## 5. Make agents verify their work
I define proof before execution. Appropriate proof can include automated tests, schema validation, screenshots, browser or DOM checks, synthetic fixtures, source checks, measured before/after results or human acceptance. Agent self-review is useful, but it is not independent proof for high-consequence work.

## 6. Correct narrowly
When proof fails, I fix the observed failure and adjacent regression, then re-run the exact failing path. I do not redesign or widen scope while an acceptance path is failing.

## 7. Measure workflow value
When changing an operating process, I require a named owner, baseline, new path, operating measure, outcome measure, quality guard and stop or rollback condition. I do not claim ROI until measured evidence supports it.

## 8. Record learning without creating a backlog
A project should leave a reusable primitive: a skill, test, template, architecture pattern, checklist or decision rule. A new tool, article or case study creates a hypothesis, not an automatic project.
