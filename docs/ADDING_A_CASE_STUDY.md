# Add a case study

The site is static HTML and CSS, so a new case file does not need a framework or build tool.

1. Copy `docs/CASE_STUDY_TEMPLATE.md` and complete it with evidence you actually have.
2. Save a visitor-facing page in `case-studies/` and link `case-study.css` for shared styling.
3. Label the status clearly: planned, exploratory, tabletop, or evidence reviewed. Keep scenario assumptions separate from observations.
4. Add a card to the Case Studies section of `index.html` with a relative link to the new page.
5. Add links back to `../index.html#work`, the Evaluation Lab, and related cases where useful.
6. Update the project inventory in `docs/PROJECT_BRIEF.md` and the file list in `README.md`.
7. Edit only the canonical `index.html` homepage; retain `aether-landing.html` as a legacy entry point. Use explicit `index.html` filenames in local links.
8. Package the project folder as one ZIP, retaining its relative directory structure. Do not include credentials, account-specific hosting data, or private lab exports.

## Evidence discipline

- Use exact transcripts where available; otherwise say they are missing.
- Capture the test prompt, model/provider label as shown, date, settings, and number of runs.
- Define rubric criteria before scoring.
- A few responses are observations, not a representative benchmark.
- Mark unrun tests as unrun; do not prefill expected results as findings.
- Revisit conclusions when the model, prompt, product boundary, or evidence changes.
