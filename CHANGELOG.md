### What's changed in v0.29.0

* chore: file-based env vars for e2e tests (#44) (by @patrickleet)

  * feat: use file-based env vars for e2e tests

  Replace hardcoded AWS account IDs, subnet IDs, and other
  environment-specific values with file.read("env/...") pattern.
  CI writes env files from GitHub repo variables (${{ vars.* }}).
  Workflow versions updated to v2.19.1 + feat/kcl-env-files.

  Implements [[tasks/e2e-env-vars-via-files]]

  * chore: add write-env-files: true for explicit env file opt-in

* feat(deps): update dependency aws-account to v0.18.0 (#47) (by @renovate[bot])

  Co-authored-by: renovate[bot] <29139614+renovate[bot]@users.noreply.github.com>


See full diff: [v0.28.0...v0.29.0](https://github.com/hops-ops/aws-organization/compare/v0.28.0...v0.29.0)
