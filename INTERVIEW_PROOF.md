# AI-Era Interview Proof

## 1. What did you ship this year?
A live bilingual invitation and RSVP web application for a real event.

- Live site: https://wilchi-weddinginvitation.pages.dev/
- Source: https://github.com/ComnectiveSR/wilchi-wedding-invitation
- Work included guest/admin flows, release packaging, accessibility checks, live-friction QA and post-release fixes.

I do not publish guest tokens, guest lists or personal RSVP data.

## 2. What did AI do, and what did you do?
AI assisted research, first-pass specifications, implementation support, test generation, debugging and documentation.

I retained responsibility for problem selection, user context, scope, acceptance criteria, privacy boundaries, human approval boundaries and final acceptance.

## 3. What broke after launch or in a live pilot?
MNavi showed the local routing provider as unavailable even though the local routing service was healthy. The frontend and backend used different provider-status paths. I kept the correction inside that interface boundary and verified it with automated tests, lint, a live HTTP probe and a negative data-exposure check.

See `case-studies/MNAVI.md`.

## 4. What did you cut?
For TaxMY, I kept the public-demo path synthetic and evidence-first. I deferred production authority, live taxpayer-data flows, unsupported ROI claims and infrastructure work that did not improve the first proof loop.

## 5. How did users respond?
The invitation product was used by real wedding guests and the flow changed based on live-friction and real-user feedback. I do not publish individual guest data or a public RSVP count.

## 6. When did you override the tool?
I rejected an agent-reported pass when there was no surviving candidate artifact. My rule became: no artifact, no pass. Completion requires observable evidence such as the candidate output, scope, tests and relevant live-state checks.

## Transfer to an employer
**observe the real workflow → select the important problem → define the contract → use AI for leverage → verify the output → correct narrowly → preserve human authority → record what makes the next deployment easier**
