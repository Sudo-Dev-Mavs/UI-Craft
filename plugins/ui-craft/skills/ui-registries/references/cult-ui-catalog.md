# Cult UI catalog

Generated from Cult UI's `registry.json`. Install with `npx shadcn@latest add https://www.cult-ui.com/r/<slug>.json`, or register the namespace once (see SKILL.md) and use `npx shadcn@latest add @cult-ui/<slug>`. Docs per component: `https://www.cult-ui.com/docs/components/<slug>`. Tailwind CSS v4 and shadcn theme tokens; most components animate with Motion.

137 components. Each line: `slug`: what it is. *(npm dependencies)*

## Hero sections and blocks

- `hero-color-panel`: Split-layout hero section with responsive ColorPanels shader visuals, CTA, and tech stack badges. *(@paper-design/shaders-react)*
- `hero-dithering`: Split-layout hero section with responsive dithering shader visuals, CTA, and tech stack badges. *(@paper-design/shaders-react)*
- `hero-heatmap`: Split-layout hero section with responsive Heatmap shader visuals, CTA, and tech stack badges. *(@paper-design/shaders-react)*
- `hero-liquid-metal`: Split-layout hero section with responsive LiquidMetal shader visuals, CTA, and tech stack badges. *(@paper-design/shaders-react)*
- `hero-static-radial-gradient`: Split-layout hero section with responsive StaticRadialGradient shader visuals, CTA, and tech stack badges. *(@paper-design/shaders-react)*
- `marketing-hero-analytics`: Analytics hero section for marketing pages.

## Device and browser mockups

- `apple-iphone-17-pro`: iPhone-style device frame with Dynamic Island, status bar, and configurable frame colors. *(lucide-react, motion)*
- `apple-keyboard`: Compact Apple-style keyboard with labeled keys and media row. *(@tabler/icons-react)*
- `apple-pro-display-xdr`: Studio Display–style aluminum frame, screen modes, and interactive macOS dock. *(@tabler/icons-react, motion)*
- `apple-watch-ultra`: Watch Ultra–style case, complications, crown, and action button. *(lucide-react, motion)*
- `mock-browser-window`: A customizable browser window mockup component with support for Chrome, Safari, and generic styles, customizable sidebars, and themes.

## Buttons and CTAs

- `bg-animate-button`: Button component with animated background effects and gradient transitions. *(@radix-ui/react-slot, class-variance-authority)*
- `border-beam-button`: Shadcn Button wrapped in Border Beam: animated border glow with compact icon and text variants. *(border-beam)*
- `copy-button`: Button that copies content to clipboard with feedback. *(lucide-react, motion)*
- `cosmic-button`: Animated button/link with cosmic gradient border effect, renders as anchor or button.
- `family-button`: Button component with family-style design and interactive hover effects. *(lucide-react, motion)*
- `gradient-button-group`: Premium layered button group with animated active state, gradient ring accents, and theme toggle underlay. *(motion, next-themes)*
- `halo-button`: Primary action button with animated gradient rim, frosted fill, staggered label, and loading spinner. *(@base-ui/react, motion)*
- `metal-button`: Shadcn Button wrapped in MetalFx: animated liquid metal ring with text and icon variants. *(metal-fx, class-variance-authority)*
- `neumorph-button`: Neumorphic button component with soft shadows and tactile interaction effects. *(class-variance-authority, lucide-react, motion)*
- `organic-button`: Anchor-based CTA with fixed SVG end caps, shared surface colors via CSS variables, and size and animation variants. *(@radix-ui/react-slot, class-variance-authority, lucide-react)*
- `texture-button`: Button component with texture overlay effects and customizable variants. *(@radix-ui/react-slot, class-variance-authority)*

## AI, data and feedback widgets

- `agent-suggest-card-stack`: Stack of suggestion cards for AI agent responses.
- `ai-blob-warp`: Circular avatar with Paper Design Warp shader; motion-safe pulse, pauses off-screen and when reduced motion is preferred. *(@paper-design/shaders-react, motion)*
- `ai-instructions`: Manage and toggle AI instructions with a popover, search, and create-dialog. *(@hugeicons/core-free-icons, @hugeicons/react)*
- `analytics-chart`: Vercel-style gradient line chart with floating tooltip cards.
- `choice-poll`: Poll component with single or multiple selection, optional results, and keyboard navigation. *(@radix-ui/react-use-controllable-state, lucide-react, class-variance-authority)*
- `feature-poll`: Feature poll component with single or multiple selection, optional results, and keyboard navigation. *(@radix-ui/react-use-controllable-state, lucide-react, class-variance-authority)*
- `feature-voting`: List of features with up-vote support, optional sorting by vote count, and controlled or uncontrolled state. *(@radix-ui/react-use-controllable-state)*
- `fluid-ai-workloads`: Fluid visualization for AI workload states.
- `poll-widget`: Poll widget with inline, popover, and dialog modes, optional results, and animations. *(@radix-ui/react-use-controllable-state, class-variance-authority, lucide-react, motion)*
- `prompt-composer`: Multiline prompt field with shader avatar, staggered placeholder, loading line, and send/attach chrome. *(@base-ui/react, @paper-design/shaders-react, lucide-react, motion)*
- `prompt-library`: Browse, insert, and manage prompt templates with categories and custom prompts. *(@hugeicons/core-free-icons, @hugeicons/react)*
- `vote-tally`: List of items with up-vote support, optional sorting by vote count, and controlled or uncontrolled state. *(@radix-ui/react-use-controllable-state)*

## Text and numbers

- `bg-image-texture`: Background texture component with multiple texture variants and customizable opacity.
- `gradient-heading`: Heading component with gradient text effects and customizable styling. *(@radix-ui/react-slot, class-variance-authority)*
- `neumorph-eyebrow`: Neumorphic eyebrow component with soft shadow effects and modern styling. *(class-variance-authority)*
- `pixel-heading-character`: Per-character pixel-font heading with four animation modes using Geist pixel fonts. *(geist)*
- `pixel-heading-word`: Whole-word pixel-font heading that swaps or cycles fonts on hover using Geist pixel fonts. *(geist)*
- `pixel-paragraph-words`: Paragraph where specific words render in an interactive pixel font that swaps or cycles on hover. *(geist)*
- `pixel-paragraph-words-inverse`: Paragraph in pixel font where specific words escape into interactive sans/mono with hover swap or cycle. *(geist)*
- `rolling-number`: Number component with smooth counting animations and customizable formatting. *(motion)*
- `text-animate`: Animated text component with customizable reveal effects and timing. *(motion)*
- `text-gif`: Text component with GIF-like animation effects and customizable styling. *(class-variance-authority)*
- `texture-card`: Card component with texture background and customizable styling options.
- `texture-overlay`: Texture overlay component with various CSS gradient patterns for adding visual texture to backgrounds.
- `typewriter`: Typewriter effect component with customizable typing speed and cursor animation. *(motion)*

## Cursor and pointer effects

- `illustration-cursor`: Cursor illustration and demo for collaboration UI.
- `shader-lens-blur`: WebGL shader component with lens blur effects and mouse interaction. *(motion, three, jotai, next-themes)*

## Backgrounds, patterns and ambient effects

- `bg-animated-fractal-dot-grid`: Background animated fractal dot grid with performance optimization and responsive design. *(motion)*
- `bg-animated-gradient`: Animated gradient background component with customizable color transitions. *(motion)*
- `bg-media`: Background media component with video/image support and overlay effects. *(class-variance-authority)*
- `border-beam-card`: border-beam around compound Card API with balanced title and description. *(border-beam)*
- `border-beam-input`: border-beam on Base UI input and input-group primitives with line or full border glow. *(@base-ui/react, border-beam)*
- `canvas-fractal-grid`: Interactive canvas-based fractal dot grid with mouse tracking and wave effects. *(motion)*
- `circuit-board`: Animated SVG circuit illustration with glowing traces and a central chip, for hero or product sections. *(lucide-react, motion)*
- `distorted-glass`: A glass morphism effect component using SVG filters with fractal noise to create visual transitions between sections.
- `dither-image`: Compound Next.js image figure with CSS Bayer dither via dither-plugin, partial reveal overlays, and typed tuning props. *(dither-plugin)*
- `edge-blur`: Stacked backdrop-blur layers with a gradient mask for soft top or bottom screen edges.
- `fluted-glass`: Paper Design fluted-glass image shader with sensible defaults — ribbed, streaked distortions over a source image. *(@paper-design/shaders-react)*
- `gateway-endpoint-illustration`: Illustration for gateway endpoint concepts.
- `gateway-route-illustration`: Illustration for gateway routing.
- `gateway-svg-illustration`: SVG illustration for gateway overhead.
- `globe`: COBE-powered 3D globe with showcase presets, markers, arcs, DOM overlays, and theme-aware styling. *(cobe, motion, next-themes)*
- `grid-beam`: Canvas grid beam animation with palette presets, SVG dividers, and composable headless pieces via useGridBeam.
- `illustration-card-grid`: Grid of cards with gateway illustrations.
- `illustration-comment-bubble`: Comment bubble illustration for code or chat UI.
- `illustration-fluid-rendering`: Fluid rendering illustration.
- `illustration-globe-vercel`: Globe deployment illustration.
- `illustration-graph`: Graph illustration component.
- `squiggle-arrow`: A playful, hand-drawn squiggly arrow component with customizable variants, directions, and sizes.
- `stripe-bg-guides`: Stripe-style background guides component with animated patterns and effects. *(motion)*
- `svg-bands`: Wide SVG section bands, battlement and zigzag trims, steep hero edges, and ornamental frames.
- `svg-shapes`: Wide-aspect SVG shape and panel components for backgrounds and hero decorations.
- `svg-shapes-animated`: Scroll-triggered stroke-draw animations for wide SVG shapes and panels using Motion. *(motion)*
- `tabs-illustration-vercel`: Tabs with Vercel-style illustrations.
- `tweet-grid`: Grid layout component for displaying tweet-like content cards. *(class-variance-authority)*

## Media

- `feature-carousel`: Feature carousel component with smooth transitions and customizable layouts. *(motion, clsx, react-wrap-balancer)*
- `hover-video-player`: Video player component that plays on hover with smooth animations. *(motion, lucide-react)*
- `loading-carousel`: Loading carousel component with smooth transitions and customizable content. *(embla-carousel-autoplay, lucide-react, motion)*
- `logo-carousel`: Animated logo carousel with staggered animations and customizable columns. *(motion)*
- `three-d-carousel`: 3D carousel component with perspective effects and smooth item transitions. *(motion)*
- `youtube-video-player`: YouTube video player component with custom controls and smooth animations. *(motion, lucide-react)*

## Cards, panels and surfaces

- `cutout-card`: Image card with cutout corners, hover motion, inset labels, pins, and reveal actions. *(motion, @radix-ui/react-use-controllable-state)*
- `dynamic-island`: iOS-style dynamic island component with expandable content and smooth animations. *(motion)*
- `expandable`: Expandable component system with smooth animations and customizable presets. *(motion, react-use-measure)*
- `expandable-screen`: A full-screen expandable component with morphing animations using shared layout IDs for smooth transitions. *(motion, lucide-react)*
- `family-drawer`: A multi-view drawer component with smooth animations, view navigation, and customizable content views. *(motion, react-use-measure, vaul, @radix-ui/react-slot)*
- `floating-panel`: Floating panel component with backdrop blur and position-aware animations. *(motion, lucide-react)*
- `folded-card`: Card with folded corner clip-path accent.
- `halo-card`: Composable card with animated gradient rim, frosted fill, layered shadow, and Base UI button actions. *(@base-ui/react, motion)*
- `intro-disclosure`: Intro disclosure component with expandable content and smooth animations. *(motion, react-use-measure, lucide-react)*
- `minimal-card`: Clean and minimal card component with subtle styling and hover effects.
- `morph-surface`: A morphing surface component with smooth animations, customizable dimensions, and configurable content. *(motion)*
- `organic-card`: Composable marketing card with optional link root, image slot, eyebrow/title/body, accent band, and footer CTA. *(lucide-react)*
- `organic-card-small`: Compact card with SVG silhouette, category and date, motion morph on hover, and optional link. *(lucide-react, motion)*
- `popover`: Animated popover component with form support and smooth transitions. *(motion, lucide-react)*
- `popover-form`: Form popover component with success states and animated transitions. *(motion, lucide-react)*
- `shadow-card`: Composable marketing card with L-shaped extrusion, optional pixel gradient mesh, and Radix Slot on the root. *(@radix-ui/react-slot)*
- `shift-card`: Card component with shift animation effects and hover interactions. *(motion)*
- `side-panel`: Sliding side panel component with customizable positioning and animations. *(motion, react-use-measure)*
- `toolbar-expandable`: Expandable toolbar component with step-based navigation, smooth animations, and enhanced scrolling. *(motion, @radix-ui/react-scroll-area)*
- `wizard-expandable`: Expandable multi-step wizard with optional forward validation, scrollable step rail, and Motion height transitions. *(@base-ui/react, @radix-ui/react-use-controllable-state, motion)*

## Navigation, lists and layout

- `code-block`: A beautiful code block component with tabs, copy functionality, and smooth animations. *(motion, lucide-react)*
- `collab-toolbar`: Toolbar component for collaborative editing UI.
- `direction-aware-tabs`: Tab component with direction-aware animations and smooth transitions. *(motion, react-use-measure)*
- `dock`: macOS-style dock component with hover effects and smooth animations. *(motion)*
- `feature-sticky-section`: Sticky section with controllable panels and scroll behavior. *(@radix-ui/react-slot, @radix-ui/react-use-controllable-state)*
- `halo-tabs`: Base UI tabs with gradient indicator: underline or pill variant aligned with Halo Card rim colors. *(@base-ui/react)*
- `marketing-feature-code`: Marketing section for code or network policy features. *(lucide-react)*
- `sortable-list`: Drag-and-drop sortable list component with smooth animations and reordering. *(motion, react-use-measure, lucide-react)*
- `terminal-animation`: Composable terminal animation primitives with typed command playback, tabbed scenarios, and customizable output rendering. *(@radix-ui/react-slot, @radix-ui/react-use-controllable-state)*

## Forms, inputs and controls

- `base-select`: Base UI select primitives used by Halo Select. *(@base-ui/react, @hugeicons/react, @hugeicons/core-free-icons)*
- `base-tooltip`: Base UI tooltip primitives used by Apple Pro Display XDR. *(@base-ui/react, @radix-ui/react-slot)*
- `color-picker`: Interactive color picker component with HSL support and preset colors. *(motion, lucide-react)*
- `halo-badge`: Badge with optional layout animation, live status dot, and gradient rim aligned with Halo Button / Card. *(class-variance-authority, motion)*
- `halo-dropzone`: File dropzone with animated rim, frosted fill, moving border trail, and file-type glyphs. *(lucide-react, motion)*
- `halo-field`: Form field layout (label, description, error) for HaloInput and HaloTextarea.
- `halo-input`: Single-line and multiline inputs with frosted fill and gradient rim for generic forms. *(@base-ui/react, motion)*
- `halo-notification`: Polished notification surface for local AnimatePresence use with rim variants and glyph stagger. *(@base-ui/react, lucide-react, motion)*
- `halo-progress`: Progress bar with spring-driven determinate fill and indeterminate gradient strip. *(@base-ui/react, motion)*
- `halo-search`: Search input with animated gradient border, staggered placeholder, blur deletion on clear, loading line, and Warp shader avatar. *(@paper-design/shaders-react, motion)*
- `halo-segmented`: Segmented control with frosted track, gradient rim, and spring sliding thumb. *(@base-ui/react, motion)*
- `halo-select`: Composable animated select with gradient rim, frosted fill, and staggered label. *(@base-ui/react, lucide-react, motion)*
- `halo-switch`: Toggle switch with spring thumb, frosted track, and extended touch hit area. *(@base-ui/react, motion)*
- `halo-toast`: Sonner-backed polished toasts with rim variants; mount PolishedToaster once in the root layout. *(lucide-react, motion, sonner)*
- `halo-toggle-group`: Segmented single-select control with frosted track, gradient rim, and spring-driven sliding thumb (aligned with Halo Button). *(@base-ui/react, motion)*
- `onboarding`: Composable multi-step onboarding primitives: Onboarding root with step navigation, FeatureCarousel, ChoiceGroup radio selector, TipsList, and StepIndicator with dots and pills variants. *(@radix-ui/react-use-controllable-state, class-variance-authority)*
- `timer`: Countdown timer component with customizable duration and visual styles. *(class-variance-authority, lucide-react)*

## Other

- `collab-avatar`: Collaboration avatar with initials and color. *(motion)*
- `file-icons`: Icon set for file types and languages. *(lucide-react)*
- `kanban-board`: Kanban board with drag-and-drop columns and cards. *(motion)*
- `lightboard`: Interactive lightboard component with customizable grid and lighting effects.
- `mac-screen`: Classic Mac frame with an image or GIF composited into the CRT.
- `merging-bubbles`: Merging bubbles visualization.
- `security-checkpoint`: Security checkpoint illustration or component.
- `speech-bubble`: Speech bubble component.
