# Structure

A public portable skill package with Claude Code and Codex plugin metadata.
The current tree was mirrored in commit a6b770d on 2026-08-11.

## At a glance

```text
skills/                  Default Conquistador skill and standalone outcome skills
.claude-plugin/          Claude Code plugin and marketplace manifests
.codex-plugin/           Codex plugin manifest and display metadata
VERSIONS.md              Per-skill version index and baseline history
README.md                Installation, host limits, usage, and licensing
```

List the tracked tree with `git ls-tree -r --name-only HEAD`.

## Package source

| Path | Responsibility |
| --- | --- |
| `skills/conquistador/SKILL.md` | Default teammate, routing, output contract, and persistence rules |
| `skills/conquistador/capabilities.md` | Outcome-to-capability map |
| `skills/conquistador/workflows/` | Outcome-specific work contracts |
| `skills/conquistador/standards/` | Quality, safety, context, learning, and Vietnamese rules |
| `skills/conquistador/channels/` | Platform-specific context |
| `skills/conquistador/adapters/` | Coding-agent and workspace host contracts |
| `skills/conquistador/examples/` | Example requests and deliverables |
| `skills/<outcome>/SKILL.md` | Standalone skill behavior and authoritative version |
| `skills/<outcome>/agents/openai.yaml` | Host display metadata |
| `.claude-plugin/plugin.json`, `.claude-plugin/marketplace.json` | Claude Code discovery and package metadata |
| `.codex-plugin/plugin.json` | Codex discovery and package metadata |

No application runtime, package manager manifest, or local build/test runner
is present. The README's installation commands refer to a parent monorepo.
Its referenced version verifier is absent from this checkout. Do not treat
those commands as verification of this mirror.

## Read before changing

- Read the relevant `skills/<outcome>/SKILL.md` before changing its behavior.
- Read `skills/conquistador/SKILL.md` and the affected standard or adapter
  before changing shared behavior. They define routing and approval boundaries.
- Read `VERSIONS.md` before changing skill versions. Frontmatter is
  authoritative; the version index must match it.

## Where new work goes

| To add or change | Put it in |
| --- | --- |
| A standalone outcome | `skills/<outcome>/SKILL.md` and `skills/<outcome>/agents/openai.yaml` |
| Default routing or an outcome contract | `skills/conquistador/capabilities.md` or `skills/conquistador/workflows/` |
| A shared standard or host rule | `skills/conquistador/standards/` or `skills/conquistador/adapters/` |
| Plugin discovery metadata | `.claude-plugin/` and `.codex-plugin/` |
| Current work or a decision needed | [PROGRESS.md](PROGRESS.md) |

Conventions: keep outcome skills self-contained. Use discovery rather than a
hardcoded skill count. Keep per-skill versions independent of package versions.

## Knowledge

| Location | Contents |
| --- | --- |
| `skills/` | Procedures and their supporting source |
| Git history and public GitHub PRs | Source provenance and recorded change rationale |
| [BRAIN.md](BRAIN.md) | Knowledge routing, save rules, access limits, and open questions |

New knowledge follows the save rules in [BRAIN.md](BRAIN.md).

## Other documents

- [VISION.md](VISION.md): unconfirmed direction draft.
- [PROGRESS.md](PROGRESS.md): current state, gates, and dated outcomes.
- [README.md](README.md): public entry and package use.
- [VERSIONS.md](VERSIONS.md): versions and the 2026-08-03 reconstruction baseline.
- [AGENTS.md](AGENTS.md): project entrypoint. [CLAUDE.md](CLAUDE.md) imports it.
- `LICENSE`: MIT license for this portable package.
- `.gitignore`: excludes local state, environment files, and research material.
