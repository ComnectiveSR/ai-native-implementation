# Verification Pattern

Use the cheapest reliable verifier for each claim.

- Code behavior → automated tests / linters / type checks.
- Data contract → schema validation.
- UX flow → deterministic fixture + browser/DOM + screenshot review.
- Business rule → explicit examples / acceptance cases.
- AI output → task-specific eval + human review when consequences matter.
- Deployment → live-state check, not source-code inspection alone.

Never substitute “agent reported success” for evidence.
