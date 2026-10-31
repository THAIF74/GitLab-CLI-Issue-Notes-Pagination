# Project Overview
This showcase documents a contribution to GitLab CLI related to issue-note pagination.
The affected command is:
`glab issue view --comments`
The problem was that retrieving issue notes could stop after the first API page. The contribution changes the retrieval path to collect subsequent pages.
