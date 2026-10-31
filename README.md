# GitLab CLI: Issue Notes Pagination
A technical showcase documenting my contribution to GitLab CLI.
## Contribution
**GitLab Merge Request:** [!4263 - Fetch all issue notes when viewing comments](https://gitlab.com/gitlab-org/cli/-/merge_requests/4263)
**Related issue:** [gitlab-org/cli#8687](https://gitlab.com/gitlab-org/cli/-/issues/8687)
The change addresses an issue where `glab issue view --comments` could return only the first page of issue notes.
The implementation fetches subsequent pages until pagination is complete.
## What changed
- Added pagination for issue-note retrieval.
- Used the shared `gitlab.ScanAndCollect` helper.
- Added a two-minute context timeout.
- Added regression tests for multi-page retrieval and starting from a requested page.
- Updated generated issue and incident view documentation.
## Verification
- GitLab CI pipeline: **Passed**
- Pipeline coverage: **74%**
- Merge request status: **Open**
- Merge status: **Not merged**
[View pipeline](https://gitlab.com/gitlab-community/gitlab-org/cli/-/pipelines/3012274345)
## Review and iteration
The initial review highlighted pagination conventions, timeout handling, CLI flag descriptions, and test conventions.
Follow-up commits incorporated changes to use the shared pagination helper, align the tests with the project's mock conventions, and clarify the CLI documentation.
## Repository structure
- `docs/` — problem analysis, design, and implementation notes
- `technical-notes/` — code changes, testing, and learnings
- `evidence/` — screenshots and supporting records
- `CONTRIBUTION.md` — contribution details and attribution
## Attribution
This repository is an independently maintained technical showcase of my contribution.
The original project and source code belong to the GitLab CLI project and its maintainers. The upstream merge request remains the authoritative record of the contribution and its review status.
