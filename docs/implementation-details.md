# Implementation Details
The primary implementation file is:
`internal/commands/issuable/view/issuable_view.go`
The regression test file is:
`internal/commands/issuable/view/issuable_view_pagination_test.go`
Documentation changes were made in:
- `docs/source/issue/view.md`
- `docs/source/incident/view.md`
The test coverage includes collecting notes from two pages and starting retrieval from a specified page.
See the exact upstream diff:
https://gitlab.com/gitlab-org/cli/-/merge_requests/4263/diffs
