---
name: ui-registries
description: Find, install and integrate ready-made animated React components from the Magic UI and Cult UI shadcn registries (79 and 137 components) - backgrounds, text effects, buttons, cards, device mockups, AI widgets, heroes. Use when the user names Magic UI, Cult UI, @magicui or @cult-ui, asks for a ready component or effect in a React/Next.js + Tailwind + shadcn project, or wants a section built from registry parts. Not for functional primitives like dialogs, toasts or drag and drop (use pick-ui-library) or for planning a whole company website (use taste-skill).
---

# UI Registries: Magic UI and Cult UI

Both are shadcn/ui registries: the CLI copies the component's source into the project, so the user owns the code. Use this skill to choose the right component, install it the right way, and integrate it without breaking the rest of the plugin's rules.

## Pick the source first

| The task is… | Use |
| --- | --- |
| A functional primitive: dialog, menu, toast, drawer, command menu, OTP, drag and drop, virtual list | `pick-ui-library`. A registry effect is not a substitute for an accessible primitive. |
| A whole company or product website, landing page or redesign | `taste-skill`. It plans the page and brings its own kit and finish gate. |
| One visual component or effect in a React/Next.js + Tailwind + shadcn project | This skill. |
| A component that exists in both registries (`dock`, number animation, text reveal) | Prefer the one whose look matches what the project already has. If neither, Cult UI for app/product UI (inputs, AI widgets, panels), Magic UI for marketing effects (backgrounds, text, social proof). |

**Overlaps with the curated list:** for animated numbers, `pick-ui-library` names NumberFlow; use Magic UI `number-ticker` or Cult UI `rolling-number` only when the user asks for them or the project already uses that registry. Cult UI `halo-toast` is built on Sonner, so it agrees with the curated pick.

**Inside a `taste-skill` build:** its kit, motion layer and house rules win. Add a registry component only for a piece the kit doesn't have, and only if it passes taste-skill's "Never" list and its finish gate (no fade-in on every section, no violet or lavender in the page's own design, one or two dealt moments per page).

## Workflow

1. **Name the outcome.** Section type, tone, how much motion, and what it must do on a phone. Pick one primary component and at most one supporting effect per viewport.
2. **Find candidates** in the catalogs below. Read only the catalog you need; open the component's docs page before installing if its props or dependencies matter.
3. **Check prerequisites.** React or Next.js with Tailwind CSS, and shadcn initialized (`components.json` exists). If not:
   ```bash
   npx shadcn@latest init
   ```
   Cult UI targets Tailwind CSS v4 and shadcn theme tokens. On a Tailwind v3 project, say so before installing and expect to adapt classes.
4. **Install.**
   ```bash
   # Magic UI: the namespace works out of the box
   npx shadcn@latest add @magicui/<slug>

   # Cult UI: by URL, no setup
   npx shadcn@latest add https://www.cult-ui.com/r/<slug>.json
   ```
   To install Cult UI by name, register its namespace once in `components.json`:
   ```json
   { "registries": { "@cult-ui": "https://www.cult-ui.com/r/{name}.json" } }
   ```
   then `npx shadcn@latest add @cult-ui/<slug>`.
5. **Integrate.** Import from the generated path (usually `@/components/ui/<slug>`; adapt if the project has no `@/` alias). Customize through props and `className` before editing the generated source. If customization grows, wrap it in a local component instead of rewriting registry output. Add any npm dependency or global keyframes the docs list.
6. **Check it against the plugin's motion rules** before calling it done:
   - `prefers-reduced-motion` respected; auto-scrolling content (marquees, carousels) pauses on hover and focus.
   - No `transition: all`, nothing entering from `scale(0)`; press feedback around `scale(0.97)`.
   - At most two high-motion effects in one viewport; animated backgrounds keep text contrast at 4.5:1.
   - No horizontal overflow at 390px; interactive parts reachable by keyboard.
   - For anything that stutters, run `animation-performance`; for a second opinion on the motion, `review-animations`.

## Troubleshooting

| Symptom | Fix |
| --- | --- |
| `components.json` or registry init error | Run `npx shadcn@latest init` in the project root. |
| `@cult-ui/...` not found | Register the namespace (step 4) or install by URL. |
| Import path errors | The project doesn't use the `@/` alias: use its alias or relative imports. |
| Component renders but looks wrong | A global CSS keyframe or theme token is missing; check the component's docs. |
| Missing package | Install the npm dependencies listed in the catalog line or docs. |

## References (load on demand)

- `references/magic-ui-catalog.md`: every Magic UI component, grouped, with dependencies.
- `references/cult-ui-catalog.md`: every Cult UI component, grouped, with dependencies.
- `references/magic-ui-recipes.md`: section recipes (hero, trust rail, feature grid) with guardrails.

Docs: `https://magicui.design/docs/components/<slug>` and `https://www.cult-ui.com/docs/components/<slug>`.

Sources: Magic UI (MIT, magicuidesign/magicui) and Cult UI (MIT, nolly-studio/cult-ui). Catalogs generated from each project's `registry.json`.
