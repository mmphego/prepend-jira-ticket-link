# Prepend-JIRA-Ticket-Link

Pre-Commit hook that prepends JIRA ticket number and URL in the commit message.

## Adding to your `.pre-commit-config.yaml`

```yaml
-   repo: https://github.com/mmphego/pygrep-hooks
    rev: master
    hooks:
    -   id: prepend-jira-link
    # ...
```

## Provided hooks

- [x] **prepend-jira-link** - Adds [JIRA](https://www.atlassian.com/software/jira) ticket number and link to commit message.
    - If JIRA ticket ID is not present in commit message, it will check the branch name, if it contains a ticket id.
    - If found will append it to the commit message.
