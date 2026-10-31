# Contribution Record
## GitLab CLI — MR !4263
- Contributor: THAIF74
- Project: gitlab-org/cli
- Merge request: https://gitlab.com/gitlab-org/cli/-/merge_requests/4263
- Related issue: https://gitlab.com/gitlab-org/cli/-/issues/8687
- Branch: `fix/issue-view-comments-pagination`
- Current status: Open
- CI status: Passed
- Coverage reported by pipeline: 74%
### Contribution summary
Implemented pagination for issue-note retrieval used by `glab issue view --comments`.
The change collects notes across pages, preserves the requested starting page and page size, and uses the shared pagination helper with context timeout handling.
### Tests
Added regression coverage for:
1. Collecting notes across multiple pages.
2. Starting retrieval from a requested page.
### Attribution and status
This is a record of my submitted contribution. It has not yet been merged into the upstream project. Refer to the GitLab merge request for the authoritative review and merge status.
