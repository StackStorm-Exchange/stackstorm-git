# Changelog

## 0.6.1

- Add explicit support for Python 2 and 3

## 0.6.0
- Update GitPython dependency version to <3.0 (PR #9)

## 0.5.1
- Fix typo in action name

## 0.5.0

- Added 4 new actions
- `checkout_remote_branch` - checkout a remote branch for a repository
- `remote_branch_exists` - Check the remote repository if a branch exists
- `commit_and_push` - Adds all files (.), commits with message (-m), and pushes to remote. Requires SSH certificates inplace and ssh-keyscan already ran against git server (for non interactive), as well as an author alias in `~/.gitconfig`
- `new_local_branch` - Create a new local branch for a repository

## 0.4.2

- Version bump to fix tagging issue, no code changes

## 0.4.0

- Rename `config.yaml` to `config.schema.yaml` and update to use schema.
- added missing `commit_message` to payload schema
