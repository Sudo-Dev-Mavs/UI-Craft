# UI Craft

A Claude plugin that merges four sets of UI skills into one: Emil Kowalski's animation and polish skills, taste-skill for full company websites, the components.build spec, and the Magic UI and Cult UI component registries. Overlapping skills were merged so they don't compete for the same requests.

## Install

**Claude (Cowork):** Customize → Plugins → Add marketplace → `Sudo-Dev-Mavs/UI-Craft`, then install **ui-craft**.

**Claude Code:**

```bash
claude plugin marketplace add Sudo-Dev-Mavs/UI-Craft
claude plugin install ui-craft@ui-craft
```

Not sure where to start? Run `/ui-craft:which-skill` and describe the situation.

## Skills (23)

| Area | Skills |
| --- | --- |
| Start here | `which-skill` |
| Whole websites | `taste-skill` (needs Node 22+ and Chrome, Edge or Chromium for its checker and finish gate) |
| Building motion | `animate`, `choreograph`, `gestures`, `animate-expo`, `prototype` |
| Components and libraries | `components-build`, `ui-registries` (Magic UI + Cult UI), `pick-ui-library`, `ask-sonner` |
| Checking and fixing | `review-animations`, `break-ui`, `mobile-native`, `animation-performance` |
| Upkeep | `improve-animations`, `find-animation-opportunities`, `remove-animations` |
| Knowledge | `emil-design-eng`, `apple-design`, `animation-vocabulary` |
| Learning | `learn-taste` |
| Standalone | `write-swift` |

`which-skill`, `learn-taste`, `pick-ui-library`, `prototype` and `review-animations` run only when you call them as slash commands, as upstream designed them.

## Credits and licenses

Built from MIT-licensed work by Emil Kowalski, Leonxlnx (taste-skill), Magic UI, and Cult UI / Nolly Studio (including the components.build spec by Hayden Bleasel and shadcn). Each license is in `plugins/ui-craft/licenses/`. `UPSTREAM.md` records the source commits and every change made.
