# Problem Analysis
GitLab API list endpoints can return results across multiple pages.
The issue addressed by MR !4263 was incomplete comment retrieval: the CLI could display only the notes returned on the first page.
This meant users could miss older or additional issue notes when viewing comments.
Related issue: https://gitlab.com/gitlab-org/cli/-/issues/8687
