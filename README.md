# Renovate commit messages for groups

Changing commit message for a package group does not seem to have any effect.

As an attempt to configure this the repo sets both the deprecated `commitMessage` and the individual action, prefix, suffix, topic and extra parts.

## Expected behaviour

A PR with a commit message other than `"chore(deps): update jest monorepo"`.

Since `commitMessage` is set to literal `"commit message"` I would expect the commit message to be `"commit message"`.

If I remove `commitMessage` and rely on non-deprecated configuration I would expect the commit message to be `"prefix action topic extra suffix"`.

## Actual behaviour

Commit message is always `"chore(deps): update jest monorepo"`.
