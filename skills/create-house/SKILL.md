---
name: create-house
description: Create or revise an editable HouseCraft home model from plans, photos, or measurements; add renovation variants and preview them locally.
---

# Create a HouseCraft project

1. Use the viewer checkout and ref in the project’s local HouseCraft setup record. If the toolchain is not set up or its recorded checkout or tools no longer match, follow [setup](../setup/SKILL.md). If a prerequisite is missing, report it and which steps it blocks.
2. Read `docs/project-format.md` in the viewer checkout. Use `examples/two-room/housecraft.json` as a reference for structure. Keep the user's editable project outside both the viewer and plugin checkouts, and keep original plans, photos and other inputs untouched and outside the preview project. Use descriptive source labels without embedding personal paths or URLs.
3. Establish scale from the inputs. Ask for missing dimensions that block a usable model, mark estimates and their basis, and flag multi-level inputs rather than flattening them. Describe the existing home as the baseline. For proposed changes, copy a validated snapshot to a new variant and keep the baseline and other variants intact. Preserve any existing project when generation or validation fails. Record structural changes as conceptual and unassessed.
4. Use the default viewer and proxy furniture. Consider extras only if the viewer checkout documents a compatible plugin and that plugin has been reviewed. Follow the checked-out project format and the viewer's supported features.
5. From the viewer checkout run `node bin/housecraft.mjs validate "/absolute/path/to/housecraft.json"` on the candidate. Resolve validation failures before saving over an existing file. Then run `node bin/housecraft.mjs preview "/absolute/path/to/housecraft.json" --port 0` on the saved project. Report the actual project path, the localhost URL printed by the running process, and any estimates or unresolved inputs. If preview cannot run, report the failure and give the command the user can run locally.
