---
on:
  schedule:
    - cron: daily around 10:00
  workflow_dispatch: null
permissions:
  contents: read
  pull-requests: read
  issues: read
safe-outputs:
  create-pull-request:
    title-prefix: "[docs] "
    labels:
      - documentation
    allowed-base-branches:
      - main
  noop: null
description: Daily workflow to identify out-of-date documentation and open a PR with updates
emoji: 📝
engine:
  id: copilot
  version: "1.0.21"
strict: true
---

# Daily docs sync

Review recent repository changes and documentation files to find out-of-date docs.

If documentation changes are needed:
1. Update only the affected documentation files.
2. Create a pull request using the `create_pull_request` safe-output tool with a clear summary.

If no updates are needed, call `noop` with a short reason.
