# Magic UI catalog

Generated from Magic UI's `registry.json`. Install with `npx shadcn@latest add @magicui/<slug>` (the `@magicui` namespace resolves without extra config). Docs per component: `https://magicui.design/docs/components/<slug>`.

79 components. Each line: `slug`: what it is. *(npm dependencies)*

## Hero sections and blocks

- `hero-video-dialog`: A hero video dialog component. *(motion)*

## Device and browser mockups

- `android`: A mockup of an Android device.
- `iphone`: A mockup of the iPhone.
- `safari`: A safari browser mockup to showcase your website.

## Buttons and CTAs

- `animated-theme-toggler`: Theme toggle with View Transitions and animated clip-path masks (circle, polygons, star), optional viewport-centered origin. *(lucide-react)*
- `interactive-hover-button`: .
- `pulsating-button`: An animated pulsating button useful for capturing attention of users.
- `rainbow-button`: An animated button with a rainbow effect.
- `ripple-button`: An animated button with ripple useful for user engagement.
- `shimmer-button`: A button with a shimmering light which travels around the perimeter.
- `shiny-button`: A shiny button component with dynamic styles in the dark mode or light mode. *(motion)*

## Text and numbers

- `animated-gradient-text`: An animated gradient background which transitions between colors for text.
- `animated-shiny-text`: A light glare effect which pans across text making it appear as if it is shimmering.
- `aurora-text`: A beautiful aurora text effect.
- `comic-text`: Comic text animation. *(motion)*
- `dia-text-reveal`: A horizontal color band sweeps across text, revealing a gradient shine before settling on the base color. *(motion)*
- `highlighter`: A text highlighter that mimics the effect of a human-drawn marker stroke. *(motion, rough-notation)*
- `hyper-text`: A text animation that scrambles letters before revealing the final text. *(motion)*
- `kinetic-text`: A text component that animates font weight of characters on hover.
- `line-shadow-text`: A text component with a moving line shadow. *(motion)*
- `morphing-text`: A dynamic text morphing component for Magic UI.
- `noise-texture`: An SVG fractal noise layer using feTurbulence, desaturation, and contrast controls for subtle texture overlays.
- `number-ticker`: Animate numbers to count up or down to a target number. *(motion)*
- `sparkles-text`: A dynamic text that generates continuous sparkles with smooth transitions, perfect for highlighting text with animated stars. *(motion)*
- `spinning-text`: The Spinning Text component animates text in a circular motion with customizable speed, direction, color, and transitions for dynamic and engaging effects. *(motion)*
- `text-3d-flip`: A text effect that flips each letter in 3D with a staggered animation on hover. *(motion)*
- `text-animate`: A text animation component that animates text using a variety of different animations. *(motion)*
- `text-reveal`: Fade in text as you scroll down the page. *(motion)*
- `typing-animation`: Characters appearing in typed animation. *(motion)*
- `video-text`: A component that displays text with a video playing in the background.
- `word-rotate`: A vertical rotation of words. *(motion)*

## Cursor and pointer effects

- `confetti`: Confetti animations are best used to delight your users when something special happens. *(canvas-confetti, @types/canvas-confetti)*
- `cool-mode`: Cool mode effect for buttons, links, and other DOMs.
- `glare-hover`: A diagonal glare on hover using a ::before gradient and CSS variables (angle, size, duration, color).
- `lens`: A interactive component that enables zooming into images, videos and other elements. *(motion)*
- `pointer`: A component that displays a pointer when hovering over an element. *(motion)*
- `smooth-cursor`: A customizable, physics-based smooth cursor animation component with spring animations and rotation effects. *(motion)*

## Backgrounds, patterns and ambient effects

- `animated-beam`: An animated beam of light which travels along a path. Useful for showcasing the integration features of a website. *(motion)*
- `animated-grid-pattern`: A animated background grid pattern made with SVGs, fully customizable using Tailwind CSS. *(motion)*
- `backlight`: A backlight glow effect for videos, images, and SVGs.
- `bento-grid`: Bento grid is a layout used to showcase the features of a product in a simple and elegant way. *(@radix-ui/react-icons)*
- `blur-fade`: Blur fade in and out animation. Used to smoothly fade in and out content. *(motion)*
- `border-beam`: An animated beam of light which travels along the border of its container. *(motion)*
- `dither-field`: An animated WebGL2 background of Bayer-dithered square dots. The dots follow a light pattern, an image or a video, take one color or a three-stop ramp, and brighten under the pointer.
- `dot-pattern`: A background dot pattern made with SVGs, fully customizable using Tailwind CSS.
- `dotted-map`: A component with a dotted map. *(svg-dotted-map)*
- `flickering-grid`: A flickering grid background made with SVGs, fully customizable using Tailwind CSS.
- `floating-3d-particles`: A canvas-based pseudo-3D particle field with perspective projection, continuous rotation and buoyant drift.
- `globe`: An autorotating, interactive, and highly performant globe made using WebGL. *(cobe@^0.6.4, motion)*
- `grid-pattern`: A background grid pattern made with SVGs, fully customizable using Tailwind CSS.
- `hexagon-pattern`: A background hexagon pattern made with SVGs, fully customizable using Tailwind CSS.
- `icon-cloud`: An interactive 3D tag cloud component. *(lucide-react)*
- `interactive-grid-pattern`: A interactive background grid pattern made with SVGs, fully customizable using Tailwind CSS.
- `light-rays`: A component with animated light rays which shine down from above. *(motion)*
- `meteors`: A meteor shower effect.
- `neon-gradient-card`: A beautiful neon card effect.
- `orbiting-circles`: A collection of circles which move in orbit along a circular path.
- `particles`: Particles are a fun way to add some visual flair to your website. They can be used to create a sense of depth, movement, and interactivity.
- `progressive-blur`: The Progressive Blur component adds a smooth blur gradient effect to scrollable content, indicating more content below or above.
- `retro-grid`: An animated scrolling retro grid effect.
- `ripple`: An animated ripple effect typically used behind elements to emphasize them.
- `striped-pattern`: A background striped pattern made with SVGs, fully customizable using Tailwind CSS.
- `warp-background`: A card with a time warping background effect. *(motion)*

## Media

- `client-tweet-card`: A client-side version of the tweet card that displays a tweet with the author's name, handle, and profile picture. *(react-tweet)*
- `pixel-image`: A component that displays an image with a pixelated effect, creating a retro aesthetic.
- `tweet-card`: A card that displays a tweet with the author's name, handle, and profile picture. *(react-tweet)*

## Cards, panels and surfaces

- `magic-card`: A spotlight effect that follows your mouse cursor and highlights borders on hover. *(motion)*
- `shine-border`: Shine border is an animated background border effect.

## Navigation, lists and layout

- `animated-list`: A list that animates each item in sequence with a delay. Used to showcase notifications or events on your landing page. *(motion)*
- `code-comparison`: A component which compares two code snippets. *(shiki, @shikijs/transformers)*
- `dock`: An implementation of the MacOS dock using react + tailwindcss + motion. *(motion)*
- `file-tree`: A component used to showcase the folder and file structure of a directory.
- `marquee`: An infinite scrolling component that can be used to display text, images, or videos.
- `scroll-based-velocity`: Scrolling text whose speed changes based on scroll speed. *(motion)*
- `scroll-progress`: Animated Scroll Progress for your pages. *(motion)*
- `terminal`: A terminal component.

## Forms, inputs and controls

- `animated-circular-progress-bar`: Animated Circular Progress Bar is a component that displays a circular gauge with a percentage value.

## Other

- `avatar-circles`: Overlapping circles of avatars.
- `glyph-matrix`: An animated grid of subtly shifting glyphs with fade effect and theme support.
