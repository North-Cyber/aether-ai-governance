# Aether 2.0

AI Governance & Product Risk Portfolio

AETHER is an independent, hands-on learning and portfolio project about how teams can evaluate AI products before release. The site is a static, locally runnable prototype: it includes a portfolio homepage, three scenario-based case files, and a browser-based evaluation lab.

## Project highlights

- Turn AI product concerns into concrete test scenarios, risk hypotheses, and proposed release gates.
- Explore reliability, privacy, safety, and accessibility through fictional healthcare-support scenarios.
- Keep observed evidence separate from assumptions, plans, and unknowns.
- Run the interface locally with plain HTML, CSS, and JavaScript; no framework, backend, model connection, or API key is required.

The project is educational and evidence-limited. It demonstrates a review method; it does not certify a model or product.

## Open the site

1. Clone or download this repository, or extract the share-ready ZIP.
2. Open `index.html` in a current browser.
3. Use the homepage links to visit the case files and `lab/`.

There is no build step, account, model API key, analytics, or backend. In the lab, the person running an evaluation copies a fictional test prompt into a separate AI chat, pastes the actual response back, rates it, and may export a Markdown or JSON report. Lab entries are kept in that browser's local storage when available.

## What's included

- `index.html` — portfolio homepage and project overview.
- `case-studies/r-01.html` — reliability exercise about unverified clinic hours.
- `case-studies/p-01.html` — privacy exercise about a healthcare reminder on a shared phone.
- `case-studies/e-01.html` — fictional tabletop launch review with a risk register, proposed test plan, evidence gaps, launch gates, and decision memo.
- `lab/` — five manual, fictional AI evaluation scenarios and report export.
- `docs/` — project brief, case-study template, update guidance, review notes, risk register, and sharing checklist.
- `FRIEND_PROMPT.md` — current Aether 2.0 handoff for a collaborator or AI assistant.
- `docs/ORIGINAL_FRIEND_PROMPT.md` — unchanged original v1 request, retained for provenance.
- `docs/E-01_RELEASE_GATES.csv` — proposed gate owners, evidence deliverables, and closure records.
- `SEND_TO_FRIEND.md` — a short message to send with the ZIP.

## Update the site

Edit the files in this extracted folder directly. `index.html` is the canonical homepage; case pages are in `case-studies/`, and the evaluation lab is in `lab/`. Shared case styling is `case-studies/case-study.css`. There is no `dist/` folder and no build step. `aether-landing.html` is a legacy entry point; maintain the homepage in `index.html`, not two separate copies.

Keep relative links explicit, such as `lab/index.html`, so navigation works when opening local files as well as on a static host. Keep a copy of the original ZIP before editing.

See `docs/ADDING_A_CASE_STUDY.md` for a simple case-file workflow and `docs/CASE_STUDY_TEMPLATE.md` for a reusable outline.

## Scope and evidence

All clinic, patient-support, and product examples in this project are fictional. R-01 summarizes notes about two early responses; the underlying transcripts and complete model/version metadata are missing. P-01 records a scenario-based privacy review. E-01 is a tabletop exercise: no product or model was tested, its likelihood ratings are unknown, and its “hold” recommendation reflects missing evidence rather than an observed product failure.

The work is educational. It is not a real organization audit, clinical evaluation, security certification, legal or regulatory determination, or proof that any model is safe. Use invented data only; never paste real health information or identity data into the lab.

## Sharing and publishing

The ZIP is a portable handoff package. It intentionally does not include account-specific hosting metadata, credentials, or private evaluation results. The static website is structured for a future static host, but it has **not been published**. Review `docs/BEFORE_SHARING_OR_PUBLISHING.md` before making it public.

## Continue with evidence, not invented results

1. For R-01, obtain the original transcripts or run a newly documented evaluation. Do not reconstruct missing responses.
2. For P-01, preserve the exact reminder scenario and explain the consent and shared-device assumptions.
3. For E-01, start with the product boundary and proposed release-gate worksheet. All gates remain open, all planned tests unrun, and likelihoods unknown.
4. Export lab evidence before clearing browser storage or moving the project. Local storage is browser- and location-dependent, not an encrypted archive or a backup.

The portfolio P-01 is a **shared-phone reminder review**. The lab P-01 is a **different related scenario about another person's appointment**; matching IDs do not mean the lab is a reproduction of that case file. The fictional CareNav lab suite is not a tested implementation of the CareGuide tabletop product.
