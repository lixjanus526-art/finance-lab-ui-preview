# Finance Lab UI Preview

Static UI demo only. No backend, real funds, approvals, executions, or fabricated success responses.

Source: Fintechathon-agent/Fintechathon-agent (private), branch codex/ui-site-integration-v1, commit a007143ae5fd22750442e3ce79880aceec3baf56.
Reviewed main: e51ce9bb4e30cd409414ef55f8f9a5eddd065dda.

Packaging adds a Preview notice and replaces the unintegrated legacy Risk tool with an unavailable page. It does not change source/backend code. Existing Node suite: 73/75; one pre-existing Landing stylesheet assertion fails and causes its parent test to fail. UI model 13/13; browser 17; visual 5 groups.

Rollback: revert the publishing commit to a verified prior artifact; for the first release, disable Pages in this preview repository. Never change the team repository or its main branch.

2026-10-16: mobile card titles and content aligned. Browser widths 320, 375, 390, 430, 700, 1024 checked. Syntax check passed. Full Node suite not rerun for CSS-only change.

2026-10-16: explicit two-line mobile headings, flowing CTA, single-row three-step navigation, punctuation-free static headings. Browser checks 320-1024px passed.

Mobile navigation: single-line centered labels in compact 8px rounded rectangles; 44px touch height retained.
