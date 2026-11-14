# AETHER 2.0 — five-minute portfolio walkthrough

This short route is for a recruiter, instructor, or collaborator who wants to understand the project without reading every file.

## The five-minute route

| Time | Open | What to look for |
|---|---|---|
| 0:00–0:45 | [`../index.html`](../index.html) | The project question, six-step review method, and scope boundaries. AETHER is a learning portfolio, not a product certification. |
| 0:45–1:45 | [`../case-studies/r-01.html`](../case-studies/r-01.html) | Reliability under pressure. The notes report two responses that avoided an exact clinic closing time, while the missing transcripts and model details stay visible as evidence gaps. |
| 1:45–2:45 | [`../case-studies/p-01.html`](../case-studies/p-01.html) | Privacy judgment. A shared phone changes the recommendation: minimize the reminder, confirm permission, and avoid exposing a sensitive visit reason. |
| 2:45–4:00 | [`../case-studies/e-01.html`](../case-studies/e-01.html) | A fictional launch review. The risk register is explicitly hypothetical, likelihood remains unknown, and proposed release gates connect evidence to accountable decisions. |
| 4:00–5:00 | [`../lab/index.html`](../lab/index.html) | A working manual evaluation interface with five fictional scenarios, a human-scored rubric, local browser saving, and Markdown/JSON export. It has no model connection or automatic scoring. |

## What the work demonstrates

- Turning a broad concern into a bounded scenario and testable risk question.
- Considering how product context changes user impact and the appropriate safeguard.
- Separating observed notes, human analysis, assumptions, proposed tests, and unknowns.
- Communicating a proportionate recommendation with conditions instead of overstating certainty.
- Building a small browser-only tool that lets another person carry out and document a manual review.

## Evidence status to state plainly

- **R-01:** Project notes summarize two early responses, but the full transcripts and complete model/version details are missing. This is not a repeatable benchmark or broad reliability finding.
- **P-01:** A scenario-based privacy review and revised recommendation; no deployed product or model response was audited.
- **E-01:** A tabletop for a fictional product. No product or model tests were run; the likelihoods are unknown and the seven release gates remain open.
- **Evaluation Lab:** A manual test harness. A completed score reflects one human rating of one pasted response; AETHER does not authenticate the response, verify model metadata, or establish safety.

Do not present a scenario analysis or a proposed test as an observed result. Use synthetic information only. Never include real patient, employee, or identity data in prompts or exported evidence.

## Short interview explanation

> I built AETHER to practice pre-release AI product risk review. I take a concrete scenario, identify how a failure could affect someone, separate evidence from assumptions, and propose safeguards and decision gates. The lab is a browser-only manual test tool; I label its results carefully because a few scenario checks cannot establish that a model or product is safe.

## Useful follow-up questions

- **Why keep the recommendation conditional in P-01?** A shared device, sensitive content, and uncertain SMS permission change the likely exposure. The safer default is to minimize the notification and verify channel consent before sending.
- **Why hold the fictional CareGuide launch?** The tabletop has no system evidence. A hold means the decision is premature while essential evidence is missing; it does not mean a test found a defect.
- **What would improve the evidence next?** Run fresh-chat trials from the lab, preserve each exact prompt and response, record the visible model/version label and test timestamp, rate against criteria written before the trial, and document failures as well as passes. See [`EVALUATION_RECORD_TEMPLATE.md`](EVALUATION_RECORD_TEMPLATE.md).

## Source files for a deeper review

- [`PROJECT_BRIEF.md`](PROJECT_BRIEF.md) — purpose, method, inventory, and content rules.
- [`E-01_RISK_REGISTER.csv`](E-01_RISK_REGISTER.csv), [`E-01_TEST_PLAN.csv`](E-01_TEST_PLAN.csv), and [`E-01_RELEASE_GATES.csv`](E-01_RELEASE_GATES.csv) — tabletop artifacts, all clearly marked as proposed or open.
- [`ACCEPTANCE_AUDIT.md`](ACCEPTANCE_AUDIT.md) — documented implementation review and known limitations.
- [`BEFORE_SHARING_OR_PUBLISHING.md`](BEFORE_SHARING_OR_PUBLISHING.md) — owner review required before public release.

