# FGP FortuneGod Philippines Standard Conventional Commits
The Conventional Commits specification is a lightweight convention on top of commit messages. It provides an easy set of rules for creating an explicit commit history

## General Commit

`<type>(<optional scope>): <description>`

## Initial Commit
`chore:` init

# Types
- Changes relevant to the API or UI:
  - `feat` Commits that add, adjust or remove a new feature to the API or UI
  - `fix` Commits that fix an API or UI bug of a preceded feat commit
- `refactor` Commits that rewrite or restructure code without altering API or UI behavior
  - `perf` Commits are special type of refactor commits that specifically improve performance
- `style` Commits that address code style (e.g., white-space, formatting, missing semi-colons) and do not affect application behavior
- `test` Commits that add missing tests or correct existing ones
- `docs` Commits that exclusively affect documentation
- `build` Commits that affect build-related components such as build tools, dependencies, project version, CI/CD pipelines, ...
- `ops` Commits that affect operational components like infrastructure, deployment, backup, recovery procedures, ...
- `chore` Miscellaneous commits e.g. modifying .gitignore, ...

# Scopes
The `scope` provides additional contextual information.

- The scope is an **optional** part
- Allowed scopes vary and are typically defined by the specific project
- Do not use issue identifiers as scopes

# Description 
The `description` contains a concise description of the change.
-  The description is a **mandatory** part
-  Use the imperative, present tense: "change" not "changed" nor "changes"
  -  Think of `This commit will...` or `This commit should...`
- Do not capitalize the first letter
- Do not end the description with a period (.)


# Examples

- `feat: add email notifications on new direct messages`
- `feat(shopping cart): add the amazing button`
- `fix(shopping-cart): prevent order an empty shopping cart`
- `fix(api): fix wrong calculation of request body checksum`
- `perf: decrease memory footprint for determine unique visitors by using HyperLogLog`
- `build: update dependencies`
- `build(release): bump version to 1.0.0`
- `refactor: implement fibonacci number calculation as recursion`
- `style: remove empty line`

# References
- https://www.conventionalcommits.org/
- https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13
