# renovate-config

The shareable [renovate](https://renovatebot.com/) config preset for repositories under `team-reflect`.

Go to https://github.com/apps/renovate/installations/new to select which repo under `team-reflect` will use renovate.

## Rules defined in this preset

- For remirror packages, a pull request will be created at once when there is a new version.
- For other packages, a pull request will be created *monthly*, which will contains all available updates.
- Renovate will run `yarn-deduplicate --strategy fewer` for every pull requests to make sure that there is not dependency duplication.
- An "Dependency Dashboard" issue will be created for each repository. This issue contains a list of all PRs pending, open, closed (unmerged) or in error.

## links

How to config renovate: https://docs.renovatebot.com/configuration-options/#rangestrategy
