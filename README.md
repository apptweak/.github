# AppTweak `.github` repository

> [!WARNING]
> **This repository is public.** Everything in it, including its full Git history, open and closed pull requests, and comments, can be read by anyone on the internet, and may already be mirrored or forked. Treat every change here as a public publication.

## What this repository is for

GitHub treats a public repository named `.github` as the organization-wide default for a few things:

| Path | Effect |
|---|---|
| `profile/README.md` | Public profile page shown at [github.com/AppTweak](https://github.com/AppTweak) |
| `.github/PULL_REQUEST_TEMPLATE.md`, `.github/ISSUE_TEMPLATE/` | Default PR and issue templates for every repository that doesn't define its own |
| `SECURITY.md`, `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SUPPORT.md` | Default community health files for every repository that doesn't define its own |
| `workflow-templates/` | Starter workflows offered under **Actions → New workflow** in our repositories |

A file in an individual repository always overrides the default from here. If your team needs a template with internal or team-specific details, put it **in your own (private) repository**, not here.

What this repository does **not** do: `CODEOWNERS`, `dependabot.yml`, branch protection, rulesets and Actions settings are **not** inherited from here. Those stay per repository or are configured at organization level.

## Golden rule

**Write as if anyone on the internet could read it, because they can.** If something would be harmless in a private repository but you'd hesitate to post it on a public website, it does not belong here.

## Never commit

- **Secrets of any kind**: tokens, API keys, passwords, private keys, webhook URLs (including Slack webhooks), connection strings
- **Infrastructure details**: AWS account IDs, ARNs, role names, bucket names, internal hostnames, IP ranges, VPN or cluster names, database names
- **Internal URLs and tool instances**: links to our Jira, Confluence, Grafana, internal dashboards or private repositories. They require authentication, but they still reveal which tools we use and how they're organized.
- **Customer or partner information**: names, app IDs, contract details, usage data
- **People details**: names, emails or GitHub handles of individual employees (prefer team names), on-call rotations, org charts
- **Internal processes that help an attacker**: how deploys are approved, which checks can be skipped, incident procedures, security tooling and its gaps
- **Product roadmap or unreleased features**, even as examples in a template

## Pull request and issue templates

Keep them **generic**, so they make sense for any AppTweak repository and reveal nothing about our internals.

✅ Good:
```markdown
## What does this PR do?
## Related ticket
<!-- Link to the ticket -->
## How was it tested?
- [ ] Unit tests
- [ ] Manually tested
## Checklist
- [ ] No secrets or credentials in the code
- [ ] Documentation updated if needed
```

❌ Avoid:
```markdown
## Jira ticket
https://<our-company>.atlassian.net/browse/<PROJECT>-
## Deployed to staging?
Check https://<internal-grafana-host>/d/<dashboard-id> before merging
- [ ] Pinged @<colleague-handle> for the prod DB migration
```

If a team needs the second kind, put that template in its own repository's `.github/` folder.

## Making a change

1. Open a pull request. Direct pushes to the default branch are blocked.
2. Before requesting review, re-read your diff with the question: *"Am I OK with this being public forever?"*
3. Get approval from a code owner of this repository.
4. Remember that **PR descriptions and review comments are public too**. Keep internal discussion in Slack or Jira.

## If something sensitive was pushed

Deleting the file or force-pushing is **not enough**. The content may already be cached, forked or scraped.

1. **Rotate or revoke the secret immediately**, treating it as compromised.
2. **Alert the security contact right away**
3. Only after rotation, clean the history if needed (with the security team).