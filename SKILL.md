---
name: haizhucodex-design-skill
description: Design, redesign, audit, and implement distinctive production-ready frontend interfaces by orchestrating Taste Skill, Impeccable, shadcn, UI UX Pro Max, and Design MD Collection, with relevant motion and component patterns inspired by Motion Sites, React Bits, Uiverse, Anime.js, and Aceternity UI. Use for landing pages, dashboards, portfolios, e-commerce, design systems, interaction design, responsive frontend development, accessibility, animation planning, component selection, and final UI polish.
---

# Haizhucodex Design Skill

Create polished frontend experiences with a clear visual thesis, usable interaction model, accessible components, restrained motion, and verified implementation quality.

## Operating Modes

Choose one mode from the request and project state:

- **Design:** establish hierarchy, visual direction, tokens, components, states, and motion before implementation.
- **Build:** implement a supplied brief, screenshot, mockup, or existing design system in the current frontend stack.
- **Redesign:** preserve product behavior while improving hierarchy, branding, responsiveness, accessibility, and perceived quality.
- **Audit:** inspect an existing interface, rank issues by impact, and fix the highest-value problems.
- **Design system:** create or refine `DESIGN.md`, tokens, component rules, motion rules, and reusable patterns.

## Core Workflow

1. Inspect the repository before editing. Identify framework, package manager, routes, components, styling system, tokens, dependencies, build commands, and project conventions.
2. Extract a compact design brief containing product type, audience, primary task, content hierarchy, brand attributes, platform, responsive targets, accessibility requirements, and technical constraints.
3. Select one visual thesis. Define typography character, color behavior, spacing density, shape language, elevation, imagery, and motion hierarchy.
4. Route work through the five specialist skills when available:
   - **UI UX Pro Max:** product-category UX patterns, information architecture, palette and typography options, platform conventions, and accessibility constraints.
   - **Design MD Collection:** project-level design language, tokens, reusable component rules, and `DESIGN.md` guidance.
   - **Taste Skill:** composition, differentiation, visual judgment, anti-generic constraints, and art direction.
   - **shadcn:** accessible React primitives, component APIs, forms, overlays, navigation, data display, and states.
   - **Impeccable:** final audit covering hierarchy, typography, spacing, polish, responsiveness, and accessibility.
5. Read `references/prompt-library.md`. Select only the source patterns that serve a specific product or interaction goal.
6. Produce an implementation map covering page sections, reusable components, content states, responsive behavior, interactions, animation ownership, reduced-motion behavior, and verification commands.
7. Implement directly in the existing stack. Reuse current dependencies and conventions unless a new dependency provides clear value.
8. Verify loading, empty, error, disabled, hover, focus, active, selected, success, and destructive states where applicable.
9. Test keyboard navigation, focus visibility, semantic structure, contrast, touch targets, responsive layout, runtime errors, and `prefers-reduced-motion`.
10. Run formatter, lint, typecheck, tests, and production build. Fix failures introduced by the work.
11. Perform an Impeccable-style final critique and address the highest-impact remaining defects.

## Pattern Selection Rules

- Use **Motion Sites** for scroll narratives, editorial transitions, launches, portfolios, and immersive hero sections.
- Use **React Bits** for reusable React animation primitives, animated text, lists, cards, backgrounds, and transitions.
- Use **Uiverse** for focused controls and micro-interactions such as buttons, inputs, toggles, loaders, and tooltips.
- Use **Anime.js** for coordinated timelines, SVG sequences, staggered animation, and state-driven motion that CSS alone cannot express cleanly.
- Use **Aceternity UI** for premium React landing-page compositions, feature showcases, navigation, cards, and atmospheric backgrounds.

Do not stack signature effects merely because they are available. Every effect must support hierarchy, feedback, orientation, storytelling, or comprehension.

## Design Guardrails

- Establish one dominant visual idea and apply it consistently.
- Prioritize task completion and information architecture over decoration.
- Avoid generic gradient-heavy AI styling, excessive glassmorphism, random floating cards, ornamental charts, uniform rounded rectangles, and animation on every element.
- Limit prominent typefaces, accent colors, elevation levels, border radii, and motion families.
- Use semantic HTML and accessible component primitives.
- Treat mobile as a deliberate composition rather than a compressed desktop layout.
- Prefer CSS transitions for simple state changes and introduce JavaScript animation only when coordination or sequencing requires it.
- Animate transforms and opacity where possible. Avoid layout thrashing and unnecessary continuous animation.
- Preserve readable content before hydration and when animation is disabled.
- Respect external licenses. Use documented APIs or installation methods and do not redistribute third-party source without permission.

## Dependency Policy

Before adding a package:

1. Check whether the project already has an equivalent dependency.
2. Confirm framework, rendering model, and version compatibility.
3. Explain why CSS or existing utilities are insufficient.
4. Install with the repository's package manager.
5. Keep imports narrow and remove unused experiments.
6. Record the dependency and its purpose in the final summary.

If a named skill or library is unavailable, perform its role directly and continue. Do not block routine implementation on an optional integration.

## Required Deliverables

For design-only work, return:

1. Design brief.
2. Visual thesis.
3. Page and component architecture.
4. Token and typography direction.
5. Motion plan.
6. Responsive and accessibility requirements.

For implementation work, return:

1. Selected direction and rationale.
2. Files changed and key component decisions.
3. Motion and interaction behavior.
4. Accessibility and responsive verification.
5. Commands run and results.
6. Dependencies added.
7. Remaining assumptions or tradeoffs.
