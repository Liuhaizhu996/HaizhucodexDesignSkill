# Prompt and Pattern Library

Use this reference as a relevance filter. Select the smallest combination of patterns that clearly supports the product goal.

## Selection Questions

Before choosing a source, answer:

1. What user behavior or comprehension problem should the pattern solve?
2. Is the effect structural, navigational, feedback-oriented, or decorative?
3. Can CSS or an existing dependency solve it more simply?
4. Does it remain understandable with motion disabled?
5. Does it preserve keyboard, touch, SSR, and responsive behavior?

## Motion Sites

Use for launches, portfolios, editorial pages, storytelling, premium hero sections, and spatial transitions.

Relevant prompt vocabulary:

- scroll-linked narrative with restrained depth and clear reading order
- cinematic hero transition that preserves headline legibility
- masked image reveal synchronized with section entry
- sticky scene with progressive disclosure and an obvious exit
- low-amplitude layered parallax with a reduced-motion fallback
- section transition driven by color, scale, clipping, or spatial continuity
- one hero moment, subtle section entrances, and quiet micro-interactions
- narrative pacing with short dwell points and immediate navigation access

Avoid scroll hijacking, continuous animation, delayed navigation, hidden content, and motion that competes with reading.

## React Bits

Use for reusable React animation primitives, animated text, lists, cards, decorative backgrounds, cursors, and transitions.

Relevant prompt vocabulary:

- reusable typed React animation primitive with a composition-friendly API
- animated list with stable layout, keyed transitions, and no content jumping
- text reveal that remains visible before hydration and with reduced motion
- interactive card supporting pointer, keyboard, focus, and touch input
- decorative background isolated from semantic content and pointer events
- animation lifecycle with cleanup and no orphaned listeners
- component suitable for server-rendering with client behavior isolated at the boundary
- animation props exposing duration, delay, intensity, trigger, and disabled state

Review framework version, rendering model, bundle impact, hydration, cleanup, and accessibility before adoption.

## Uiverse

Use for focused UI details such as buttons, toggles, loaders, inputs, tooltips, checkboxes, switches, and cards.

Relevant prompt vocabulary:

- expressive control based on semantic HTML with a visible focus state
- compact hover and press feedback using transform, color, and shadow
- loading indicator that communicates progress without blocking assistive technology
- persistent input label with validation, helper text, and adequate hit target
- toggle with explicit on and off states and keyboard support
- community component restyled with project tokens instead of isolated pasted CSS
- micro-interaction with clear default, hover, focus, active, disabled, and loading states

Treat snippets as inspiration. Inspect source quality, license, semantics, browser support, contrast, and accessibility before use.

## Anime.js

Use for coordinated timelines, SVG motion, staggered sequences, state-driven animation, and effects that CSS cannot express cleanly.

Relevant prompt vocabulary:

- deterministic Anime.js timeline with entry, emphasis, hold, and exit phases
- stagger based on visual order with a bounded total duration
- SVG path or transform animation without layout thrashing
- component lifecycle tied to mount, state changes, cancellation, and cleanup
- user-controlled playback with pause, replay, and reduced-motion behavior
- transform and opacity-first animation with measured runtime performance
- animation scoped to a local component rather than global selectors
- timeline recreated safely when dependencies change

Do not add Anime.js for a single hover, simple opacity transition, or basic accordion animation.

## Aceternity UI

Use for premium React landing pages, feature showcases, navigation, cards, backgrounds, spotlights, and interactive hero compositions.

Relevant prompt vocabulary:

- premium hero with one dominant message and a restrained ambient effect
- feature grid with varied hierarchy instead of identical cards
- spotlight or tracing effect bound to a meaningful interaction region
- animated navigation preserving orientation, focus, and keyboard behavior
- atmospheric background clipped to its section and separated from content contrast
- component adapted to project Tailwind tokens, breakpoints, and dark mode
- advanced visual treatment isolated behind accessible semantic content
- mobile fallback that removes pointer-dependent interaction

Avoid stacking several signature effects in one viewport or using atmospheric effects behind dense content.

## Product Relevance Matrix

- **SaaS landing page:** shadcn foundation, Aceternity composition, Motion Sites transitions, Impeccable audit.
- **Dashboard:** UI UX Pro Max information architecture, Design MD tokens, shadcn components, restrained Uiverse feedback.
- **Portfolio:** Taste Skill direction, Motion Sites storytelling, React Bits text or media transitions.
- **E-commerce:** UI UX Pro Max conversion patterns, Design MD brand rules, shadcn accessibility, light Uiverse feedback.
- **Developer tool:** shadcn structure, React Bits transitions, Anime.js only for coordinated product demonstrations.
- **Editorial site:** Taste Skill typography, Design MD system, Motion Sites progressive storytelling.
- **Marketing experiment:** Aceternity hero pattern plus one React Bits or Anime.js enhancement, not both by default.
- **Mobile-first utility:** shadcn-compatible semantics, compact Uiverse feedback, minimal ambient motion.

## Motion Budget

Use one motion family per level:

- **Hero:** one memorable spatial or reveal sequence.
- **Section:** one consistent entrance pattern.
- **Component:** short feedback for state changes.
- **Ambient:** optional, low-contrast, nonessential, and disabled under reduced motion.

Recommended behavior:

- interactions should acknowledge input immediately
- common transitions should remain short and reversible
- stagger should have a bounded total duration
- motion should stop when content leaves the viewport
- reduced-motion mode should preserve meaning without animation

## Prompt Assembly Template

```text
Create a [PRODUCT TYPE] interface for [AUDIENCE] whose primary task is [TASK].
Use [VISUAL THESIS] with [TYPOGRAPHY CHARACTER], [COLOR BEHAVIOR], [SHAPE LANGUAGE], and [SPACING DENSITY].
Build from accessible shadcn-compatible primitives and project design tokens.
Use [SELECTED SOURCE] patterns only for [SPECIFIC PURPOSE].
Motion hierarchy: [HERO MOTION], [SECTION MOTION], [MICRO-INTERACTION].
Include responsive composition, keyboard interaction, visible focus, loading/empty/error/disabled states, and reduced-motion fallbacks.
Preserve [EXISTING BEHAVIOR OR CONTENT].
Avoid [ANTI-PATTERNS].
Run [FORMAT/LINT/TYPECHECK/TEST/BUILD COMMANDS] and fix regressions introduced by the implementation.
```

## Final Audit Checklist

- Is the primary action visually obvious?
- Does every section have a clear hierarchy and purpose?
- Are typography, spacing, radii, color, and elevation internally consistent?
- Are loading, empty, error, disabled, success, selected, hover, active, and focus states covered?
- Does keyboard order match visual order?
- Are focus indicators visible against every background?
- Are touch targets large enough?
- Does mobile preserve hierarchy instead of simply stacking desktop sections?
- Is animation meaningful, bounded, cancellable, and reduced-motion compatible?
- Are runtime errors, hydration warnings, type failures, lint failures, and build failures resolved?
