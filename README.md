# Finance Lab UI Preview

Static UI demo only. No backend, real funds, approvals, executions, or fabricated success responses.

Source: Fintechathon-agent/Fintechathon-agent (private), branch codex/ui-site-integration-v1, commit 9314e42a60cfe07219b343088331f5750cc685e0.
Reviewed main: 0e0fa1944bce2cd122ad0611644f9346214230a9.

Packaging adds a Preview notice and replaces the unintegrated legacy Risk tool with an unavailable page. It does not change source/backend code. Existing Node suite: 73/75; one pre-existing Landing stylesheet assertion fails and causes its parent test to fail. UI model 13/13; browser 17; visual 5 groups.

Rollback: revert the publishing commit to a verified prior artifact; for the first release, disable Pages in this preview repository. Never change the team repository or its main branch.
