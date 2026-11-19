---
name: which-skill
description: Ask which UI Craft skill or flow fits your situation. A router over every skill in this plugin - Emil Kowalski's motion and polish skills, taste-skill, ui-registries and components-build.
disable-model-invocation: true
---

# Which Skill

Before stating what a skill does or recommending one, read that skill's SKILL.md: the summaries here are for orientation only. Then recommend **one** skill (or one short sequence) for the user's situation, say why in a sentence, and name the skill they'd reach for next. Don't list the whole map back at them.

## First: what are you making?

| Making… | Start with |
| --- | --- |
| A whole company or product website, landing page, or a redesign of one | **`/taste-skill`**. It decides the page plan, copy, photos and system, builds it, and checks it in a real browser (needs Node 22+ and Chrome, Edge or Chromium). Polish its pieces with the flow below afterwards. |
| A component, screen or feature inside an app | The main flow below. |
| A reusable component or design-system piece (its API, variants, accessibility, how it's published) | **`/components-build`**, then the main flow for its motion. |

## The main flow: idea → ship

1. **Not sure what it should look or feel like?** Detour through **`/prototype`**. It builds several genuinely different versions behind a live picker, then promotes the one you pick into the real code.

2. **Build it.** Pick the builder by what's needed:
   - **`/pick-ui-library`** if the task needs a dependency (dropdown, dialog, toast, drawer, command menu, drag and drop, charts). Don't let the agent hand-roll a toast.
   - **`/ui-registries`** for a ready-made animated component or effect from Magic UI or Cult UI (backgrounds, text effects, device mockups, AI widgets) in a React + Tailwind + shadcn project.
   - **`/animate`** for one animation on the web: whether to animate at all, then tool, properties, curve, duration, interruption, exit.
   - **`/choreograph`** when several elements move together: staggers, hero entrances, view swaps, an item leaving while siblings close the gap.
   - **`/gestures`** when the user's finger drives it: drag, swipe, sheets, snap points, swipe-to-dismiss.
   - **`/animate-expo`** for any of the above in React Native or Expo.
   - **`/ask-sonner`** when the work is toasts with Sonner.

3. **Try to break it.** Before calling it done:
   - **`/break-ui`** feeds it worst-case data (long names, empty lists, huge counts, emoji, non-Latin text) and reports what broke.
   - **`/review-animations`** reviews the motion against a strict bar. Default to flagging; approval is earned.
   - **`/mobile-native`** if it runs on a phone as a web app: sticky hover, the 100vh bug, inputs that zoom, safe areas.
   - **`/animation-performance`** if anything drops frames, including scroll-linked effects and layout measurement.

4. **Learn from the session.** **`/learn-taste`** closes the loop. Run it at the end, before you clear: it turns every design correction you made into a rule with its why in `DESIGN.md`, so the next agent doesn't repeat it.

## Upkeep: a codebase that already exists

- **The motion needs work across the app** → **`/improve-animations`**. Read-only: audits every animation and writes prioritized plans another agent can execute.
- **It feels static** → **`/find-animation-opportunities`**. Read-only: proposes motion with exact values and rejects what shouldn't move. Build the accepted ones with `/animate`.
- **It feels slow or over-animated** → **`/remove-animations`**. Edits code only to subtract.

If the user isn't sure which, ask whether the problem is *bad* motion, *missing* motion, or *too much* motion.

## References underneath

Reach for these directly when **knowledge**, not a process, is what's missing.

- **`/emil-design-eng`**: the core philosophy for UI polish: component interactions, and the still-frame craft (typography, radii, shadows, hit areas). The fallback when no narrower skill fits.
- **`/apple-design`**: Apple's principles for interface design and fluid, physical motion, translated for the web.
- **`/animation-vocabulary`**: when the problem is the **word**. "What's it called when…" gives the exact term to prompt with.

## Standalone

- **`/write-swift`**: modern Swift, Swift 6 concurrency, and native iOS code. Off the web flow entirely.

## When two skills seem to fit

- **Website vs component:** `taste-skill` owns whole pages and brings its own kit and finish gate; inside one of its builds, its house rules win over a registry effect or a general polish rule.
- **Library vs registry:** `pick-ui-library` for functional, accessible primitives; `ui-registries` for visual components you'll own the source of.
- **Polish vs performance:** `emil-design-eng` and `review-animations` judge whether motion is right; `animation-performance` only asks whether each frame lands in time.

## Common situations

| You say | Reach for |
| --- | --- |
| "Build a landing page for…" / "This site looks generic" | `/taste-skill` |
| "Animate this" | `/animate` |
| "These should come in one after another" | `/choreograph` |
| "It doesn't follow my finger" | `/gestures` |
| "It stutters" / "it's janky" | `/animation-performance` |
| "Does this animation feel right?" | `/review-animations` |
| "Make the app feel better" | `/improve-animations` |
| "What could animate here?" | `/find-animation-opportunities` |
| "Too much is moving" | `/remove-animations` |
| "Give me a few options" | `/prototype` |
| "Which library should I use?" | `/pick-ui-library` |
| "Add a Magic UI / Cult UI component" / "I want an animated background" | `/ui-registries` |
| "Design the API for this component" | `/components-build` |
| "Something looks subtly off" | `/emil-design-eng` |
| "Works in Chrome, feels wrong on my phone" | `/mobile-native` |
| "Try the worst case" | `/break-ui` |
| "What's that bouncy thing called?" | `/animation-vocabulary` |
| "Stop making that mistake" | `/learn-taste` |
