# HouseCraft Plugin

This public repository holds the portable agent workflow. The separate [HouseCraft Viewer](https://github.com/pankajvaghela/housecraft-viewer) repository owns the CLI, browser viewer and project format. Keep this repository independent of local checkout paths and private repositories.

Read README.md and the relevant skill before changes. The workflow is account-free, handles one house per project and previews on localhost. Keep generated projects outside the repositories. Never copy private planning, photographs, identifying home geometry, secrets or local paths into the plugin. Update README.md, the skill and CHANGELOG.md at substantial checkpoints.

## Documentation checkpoints

After a substantial change (accepted plan/architecture decision, milestone, feature, fix or material verification result), update the relevant existing documentation and progress record automatically. Prefer updating a canonical document over creating a new note for every edit. Record what changed, why, checks run and remaining limits; never claim unrun checks.

At a coherent checkpoint, inspect the diff and unrelated changes, run appropriate checks, then prepare a concise proposed commit summary. Ask the user before committing. After an approved commit, ask separately before pushing. Never treat commit approval as push approval. Batch related changes into one reviewable checkpoint rather than asking for every file. If approval is pending, report the prepared state and stop before the gated operation.

Do not include secrets, local dependency folders, unrelated work or unreviewed personal assets. Public changes require a privacy/provenance review. Never force-push or alter repository visibility as part of a checkpoint. This is an agent-maintained workflow, not a background watcher; manual edits are reconciled when an agent next works in the repository.
