# Lesson 01 specification

## STUDIO-001 · Launch a tested calculator on an existing server

**Status:** New launch recorded; learner chose keep. Repeat verification passed; GitHub completion pending.
**Next step:** Review changes before learner-authorized publication; obtain full E2E from PR CI.
**Instructor implementation:** [issue #9](https://github.com/kaw393939/373_hosting/issues/9).
Create your own issue from the [lesson template](.github/ISSUE_TEMPLATE/studio-calculator.md).

## Agreed result

Launch the supplied published calculator image through your existing Traefik
network and a nonconflicting HTTPS hostname. Preserve unrelated services and
host access. Do not add another proxy/updater or build a substitute image.
The [release selection](studio/calculator-release.json) supplies the expected
commit and multi-platform digest independently of the running website.
An explicitly agreed adoption of a matching existing deployment is recorded
as adoption, not a fresh launch. This bounded lesson does not certify the whole
server baseline or a vulnerability-free image.

- **Public hostname:** https://calc.dhruvi.live.
- **New launch or adopted deployment, and reason:** New launch; first report records provenance launched and new_launch true.
- **Own issue / feature branch:** [Issue #1](https://github.com/dhruvi0805/my-server-studio/issues/1); `codex/studio-001-calculator`.
- **Agreed scope or actual access/configuration gap:** One pinned published calculator image on existing `hosting-web`; preserve proxy and unrelated services. Local Docker is unavailable in WSL; use full PR CI for E2E.

Private SSH targets and configuration stay in ignored local state. Share only
reviewed, selected evidence; never commit credentials or raw server output.

## Evidence to keep

| Evidence | Actual result / link |
|---|---|
| Prepared Black/Pylint/pytest and real-image browser checks | Black/Pylint and 91 tests passed; 2 deselected. Local E2E unrun; PR CI pending |
| Hosted image/commit, trusted HTTPS, valid and rejected API cases | Passed; see [latest evidence](studio/evidence.json) and [first launch](studio/launch-evidence.json) |
| Preservation of unrelated services | Five prior containers unchanged within identity/state/published-ports scope |
| Own prediction, check interpretation, browser observation and keep/revise reason | [LEARNING.md](LEARNING.md); learner contributions recorded with AI help disclosed |
| Accuracy review before publishing learner excerpts | Learner approved current excerpts in this chat |
| Actual PR, latest CI, merge and issue closure | Pending |

Link the exported `studio/evidence.json`, actual CI and issue/PR when available.
CI does not deploy this server. A fixture, green check, timestamp, closed issue
or AI assertion alone does not establish the full result. `status` reports
recorded evidence and readiness for instructor review; it does not grade,
certify authorship or establish understanding.

## Optional instructor history

The records below are background, not steps to repeat. Their original anchors
remain here so earlier links continue to work.

## HOST-001 · Keep the Traefik dashboard private

[Historical requirement and evidence](book/changes/hosting-spec-history.md#host-001--keep-the-traefik-dashboard-private).

## HOST-002 · Controlled host maintenance

[Historical requirement and evidence](book/changes/hosting-spec-history.md#host-002--controlled-host-maintenance).

## HOST-003 · Companion image security maintenance

[Historical requirement and evidence](book/changes/hosting-spec-history.md#host-003--companion-image-security-maintenance).

## Current STUDIO-001 agreement

New launch at https://calc.dhruvi.live on existing `hosting-web`, using the
pinned image in [calculator-release.json](studio/calculator-release.json).
Preserve the existing proxy and unrelated services.
[Own issue #1](https://github.com/dhruvi0805/my-server-studio/issues/1);
branch: `codex/studio-001-calculator`.
Learner-reported doctor result: ready, launch-new, mutates false.
Learner added DNS at Name.com and reported resolution to the droplet.
New launch passed: see [first-launch evidence](studio/launch-evidence.json) and [exported evidence](studio/evidence.json). Image/commit matched, selected API cases and trusted public HTTPS passed. Five prior containers were unchanged within the reported identity/state/ports scope. Fast local checks passed (Black, Pylint, 91 tests; 2 deselected); browser E2E remains unrun. Learner chose keep; reviewed contributions are in LEARNING.md. PR/CI, merge and issue closure remain pending.
