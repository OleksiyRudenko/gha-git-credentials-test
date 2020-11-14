# Git Credentials GitHub Action test repo

Purpose: Test [gha-git-credentials](https://github.com/OleksiyRudenko/gha-git-credentials)

The approach is not really consistent and is a sort of manual testing.
Quick and dirty yet allows to test if the action is basically working as expected.

## How to

1. Change `source.md` (e.g. update the ISO formatted date therein with current date)

2. Commit and push to master

3. Success if there is a commit on `master` authored by GitHub (github-action\@users.noreply.github.com)
and file `target.md` is identical to `source.md`

## Notes

By default [.github/workflows/replicate.yml](./.github/workflows/replicate.yml)
uses `gha-git-credentials` tagged as `@latest`.
Feel free replacing with a specific [version](https://github.com/OleksiyRudenko/gha-git-credentials/releases)
or branch name (`master` or a feature branch).
