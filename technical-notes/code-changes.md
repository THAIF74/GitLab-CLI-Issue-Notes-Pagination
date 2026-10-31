# Code Changes
The contribution changed the issue-note retrieval path to use `gitlab.ScanAndCollect`.
It also added context timeout handling and regression tests using the project's `gitlabtesting` mock client.
The exact implementation is maintained in the upstream GitLab CLI merge request:
https://gitlab.com/gitlab-org/cli/-/merge_requests/4263
