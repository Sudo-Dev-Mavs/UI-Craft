# Upstream sources

UI Craft is assembled from four MIT-licensed projects. This file records exactly which commit each part came from and what was changed, so upstream updates can be diffed and merged by hand.

| Part in this repo | Source | Commit | Date |
| --- | --- | --- | --- |
| `skills/` from Emil Kowalski (19 skills) | [emilkowalski/skills](https://github.com/emilkowalski/skills) via Sudo-Dev-Mavs/skills | `64eb3deb9a5fbfa041faf783e0bc3fd635872e9c` | 2026-11-15 |
| `skills/taste-skill` | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) via Sudo-Dev-Mavs/taste-skill | `f6b76575f949707b4e3c37cd86cb44b0b98643e8` (v2.5.1) | 2026-11-07 |
| `skills/ui-registries` (Magic UI parts) | [magicuidesign/magicui](https://github.com/magicuidesign/magicui) via Sudo-Dev-Mavs/magicui | `b0b2e4974b1b68cd5278277c6837a27736e20c3a` | 2026-11-17 |
| `skills/components-build`, `skills/ui-registries` (Cult UI parts), merged rules | [nolly-studio/cult-ui](https://github.com/nolly-studio/cult-ui) via Sudo-Dev-Mavs/cult-ui | `d71b1428b811c2779d46ea41b7ef8c9f9c9991c2` | 2026-10-28 |

All paths below are under `plugins/ui-craft/`.

## Changes from upstream

**Emil Kowalski's skills**
- `ask-emil` replaced by `which-skill`: same router, extended to every skill in this plugin.
- `animation-performance`: added rules from Cult UI's `fixing-motion-performance` (layout thrashing and FLIP, scroll-driven animation, stopping loops and off-screen work, one-shot vs continuous, view transitions, fixing within the existing stack). Emil's 20px blur ceiling kept.
- `emil-design-eng`: added "Static Craft: Type, Surfaces and Hit Areas" from Cult UI's `frontend-design` (typography, concentric radius, shadows over borders, image outlines, optical alignment, hit areas) and four review-checklist rows. Cult UI's motion rules were dropped where Emil's differ (press scale 0.97, stagger 30–80ms).
- `pick-ui-library`: hands visual components off to `ui-registries`.
- All other Emil skills are unchanged.

**taste-skill** (`design-taste-frontend` upstream)
- Renamed to `taste-skill` so the skill name matches its folder.
- Removed the "gate.mjs not found" diagnostics from the Stop hook in the SKILL.md frontmatter: their `>` redirects put angle brackets in the frontmatter, which claude.ai's plugin validator rejects. The gate itself still runs.
- Upstream repo files outside `skills/taste-skill` (README, install.sh, tests, Codex/Antigravity manifests) are not included.

**Magic UI**
- `magic-ui` skill folded into `ui-registries`. Its recipes are kept as `references/magic-ui-recipes.md`; its partial component list is replaced by a full catalog generated from `registry.json`.

**Cult UI**
- `components-build` kept as its own skill; broken `rules/*/SKILL.md` paths fixed to `rules/*.md`.
- `fixing-motion-performance` merged into `animation-performance`; `frontend-design` merged into `emil-design-eng`. Neither ships as a separate skill.
- New: full Cult UI component catalog generated from `apps/www/registry.json` (deprecated aliases dropped).

## Updating from upstream

1. In each fork, sync with its upstream and note the new commit.
2. Diff the upstream folder against the commit above (`git diff <old>..<new> -- skills/`).
3. Apply the diff here, keeping the changes listed above.
4. Regenerate the registry catalogs if a registry changed.
5. Bump `version` in `plugins/ui-craft/.claude-plugin/plugin.json`, then run `claude plugin validate .`.
