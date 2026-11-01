# Project context

Before project work, read the PROGRESS snapshot and STRUCTURE's
"Read before changing" section. Read the other records when the task needs
them. Use the `horsemen` skill to update them.

- [VISION.md](VISION.md): draft direction, assumptions, and owner questions
- [BRAIN.md](BRAIN.md): knowledge locations, save rules, and access limits
- [PROGRESS.md](PROGRESS.md): current state, gates, and next steps
- [STRUCTURE.md](STRUCTURE.md): package map and required reading

## Package rules

- This repository holds portable skills and plugin metadata. Hosts supply
  tools, permissions, identity, memory, and continuity. No runtime is required.
- Preserve each skill's contract. The default skill uses the smallest relevant
  capability set. Standalone outcome skills remain usable on their own.
- Use the customer's brand. Never invent capabilities, proof, metrics, or consent.
- Keep consequential actions and persistence behind the approval gates in
  [PROGRESS.md](PROGRESS.md#gates). If the host cannot enforce approval, return a draft.
- A skill's frontmatter version is authoritative. Keep [VERSIONS.md](VERSIONS.md)
  in sync without forcing skill versions to equal the package version.
- Keep private data, identifiers, account emails, and machine paths out of
  this public repository. Follow [BRAIN.md](BRAIN.md#access-rules).
- Existing installation instructions are not proof of a tested install.
  Record the evidence and its original date when you report delivery.

Inherited higher-priority instructions continue to apply.
