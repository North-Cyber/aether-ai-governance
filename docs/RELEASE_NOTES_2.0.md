# Aether 2.0 release notes

## What changed

- Kept the original ivory, evergreen and editorial visual design. Added a restrained 2.0 badge, balanced hero typography, clearer keyboard focus on case cards/links, subtle border/shadow refinements, and moved the decorative review-card mark away from footer text. Rechecked the final homepage at desktop and phone widths.
- Made `index.html` the single homepage source. The old `aether-landing.html` filename forwards to it.
- Fixed links to use explicit HTML files, including opening the lab after unzipping locally. Removed instructions to edit a nonexistent `dist/` directory.
- Clarified that R-01 observations are reported in notes, not backed by retained transcripts. Kept P-01 scenario-based and E-01 a fictional tabletop with unknown likelihoods and unrun tests.
- Added an E-01 release-gate worksheet with proposed owners, required evidence, open status, and decision/reviewer fields. Linked risk and test rows to the gates.
- Separated model/version, test time/timezone and fresh-chat self-reports per lab scenario. Reports now state the intended method instead of asserting unverified test execution.
- Protected unreadable saved browser data from automatic replacement and added an original-data download option. Loading itself does not write over storage. Valid legacy entries remain readable on the same browser/origin.
- Preserved verbatim response backticks in Markdown exports, included the shared brief, and made report filenames timestamped.
- Added visible synthetic-data guidance, an explicit response label, a skip link, keyboard focus retention for ratings, readable supporting text, and a selectable full-prompt fallback.
- Fixed the E-01 risk table causing page-wide overflow at phone widths. The table scrolls inside its own region.
- Retained the supplied prompt verbatim in `ORIGINAL_FRIEND_PROMPT.md`; refreshed the current handoff and maintainer guides.

## Verification

This is verification of the local website, not testing an AI model or validating the portfolio claims.

- JavaScript syntax check passed with the existing Node runtime.
- Six HTML pages passed relative-link, anchor and duplicate-ID checks.
- Chrome preview used a temporary loopback-only HTTP server. Homepage and lab were inspected at desktop and phone widths; the E-01 page was rechecked after the table fix. Observed layout widths: 1423 px desktop, 375 px phone, without page-level horizontal overflow after the fix.
- Followed all three case links and the lab/home navigation. The legacy homepage entry forwarded to the canonical homepage.
- Synthetic UI-only text, metadata, notes and ratings persisted across navigation and reload. No AI provider was contacted or scored.
- Actual JSON and Markdown downloads were found and read back. Scores, incomplete cases, unknown metadata, and literal response backticks were checked.
- Independent acceptance review verified the copy control by pasting through native Windows Chrome into an isolated local test field: the complete R-01 prompt matched exactly (1,083 characters). The earlier automation clipboard mismatch was caused by its separate virtual clipboard. The complete prompt also remains selectable for manual copying. No clipboard permission or browser setting was changed.
- Reset visibly cleared only the synthetic UI test entries. The cancel branch was not independently established by the browser automation.
- Isolated Node tests cover saved-data migration, malformed data preservation, blocked/unavailable storage, report formatting, unknown metadata and completion rules. See `QA_LOGIC_RESULTS.json` for exact cases and final source hash.

## Independent acceptance corrections

- Added an accessible name to the phone header’s arrow-only lab link. At 375 px, keyboard Tab reaches it and Enter opens the lab.
- Darkened two small lab labels and corrected the dark-sidebar decision label. Calculated contrast is 5.62:1, 5.75:1 and 6.67:1 against their backgrounds.
- See `ACCEPTANCE_AUDIT.md` for the exact-prompt requirement matrix and remaining verification limits.

## Remaining evidence gaps

R-01 still needs full transcripts, model/version labels, dates/settings and repeated trials. P-01 remains a hypothetical privacy review. E-01 still needs actual product boundaries, architecture/data/vendor evidence, accountable reviewers and the planned tests before any launch decision. The lab cannot verify pasted responses or human scores.

No cross-browser, assistive-technology certification or live `file://` runtime test is claimed. Browser storage under `file://` differs by browser and path; export before moving the folder or clearing browser data. External framework links were retained, not revalidated, because framework-specific wording was not changed.

The project remains static, local and unpublished. No accounts, model connections, tracking, backend or new dependencies were added. Nothing was sent to the friend. Original input files were preserved.

## Follow-up after the 2026-11-13 audit

- Added lab P-03, a shared-phone reminder scenario directly related to portfolio case P-01. The lab now has six scenarios and 18 criteria; the existing five scenarios retain their IDs.
- Added `PORTFOLIO_WALKTHROUGH.md` for a five-minute reviewer tour and `EVALUATION_RECORD_TEMPLATE.md` for preserving exact prompts, actual responses, metadata, ratings, and limitations.
- This follow-up was not run against an AI model and has not received a new browser or acceptance audit. The prior audit describes the earlier five-scenario source only. P-03 results remain untested; no response or score is claimed.
