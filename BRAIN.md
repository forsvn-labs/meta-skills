# Brain

Knowledge home: Git repository, public package source and records · Confirmed: not yet (knowledge policy drafted from repository evidence)

Visibility: public

Project key: `forsvn-labs/meta-skills`. Resolve any private sources in the
owner's private registry. No private mapping or account is verified here.

## Where knowledge lives

| Knowledge | Home | Access |
| --- | --- | --- |
| Package behavior and reusable procedures | `skills/` | Git |
| Installation and host limits | [README.md](README.md) | Git |
| Skill versions | Each skill's frontmatter; [VERSIONS.md](VERSIONS.md) is the matching index | Git |
| Decisions and source history | Repository commits and GitHub pull requests | Git and GitHub CLI |
| Release evidence | [GitHub releases](https://github.com/forsvn-labs/meta-skills/releases) | GitHub CLI |
| Work tracking | [PROGRESS.md](PROGRESS.md) and [open issues](https://github.com/forsvn-labs/meta-skills/issues) | Git and GitHub CLI |

## Retrieve

1. Read the relevant skill and only the workflows or standards it names.
2. Use Git history, pull requests, and releases to check dates and provenance.
3. Open the original. A version label or a mirror commit does not prove release.

## Save

- Keep package behavior in its existing skill files. Keep work state in
  PROGRESS and paths in STRUCTURE. Record decision rationale in the pull request.
- Persistence is optional. Follow the existing project convention before the
  fallback described in [the coding adapter](skills/conquistador/adapters/coding-agent.md).
- Durable learning and shared product context require explicit approval under
  [learning](skills/conquistador/standards/learning.md) and
  [context](skills/conquistador/standards/context.md). Keep evidence labels and dates.
- Do not save secrets, personal data, private workspace content, or internal
  strategy in this public repository. Do not copy drafts or hidden reasoning
  into durable learning.

## Key decisions

- 2026-08-11: Mirror commit [a6b770d](https://github.com/forsvn-labs/meta-skills/commit/a6b770d2bb1f112b888e410b1fe3f383c0812a06)
  replaced the previous package tree with the current Conquistador source.
  This is source history, not evidence of a new public release.

## Access rules

- Scope: public repository evidence. No external knowledge account or
  destination is established by the source. Use Git and the GitHub CLI here.
- Keep private source identifiers in the owner's private registry, under the
  project key above. Do not put private links, account emails, or machine paths here.
- The host owns tools, identity, memory, permissions, and approval state.
  Installing this package grants no service access.
- External actions and persistence retain the approval requirements in
  [PROGRESS.md](PROGRESS.md#gates).

## Access problems

- Missing or inaccessible source: report it. Do not change accounts, sharing,
  credentials, providers, or settings to obtain access.
- A link proves neither access nor an installed capability. Do not infer
  Slack or Buzz access from the package's workspace instructions.

## Open questions

- Is this mirror an authoring source or only a distribution copy? Commit
  a6b770d records a sync, but the checkout has no sync procedure. Hung decides.
- Is a separate private knowledge home approved? No destination is recorded.
  Hung decides before any external write.
