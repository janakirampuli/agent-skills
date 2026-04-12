---
name: frontend-design
description: Use this skill to design or refine web interfaces with strong UX quality, visual clarity, accessibility, responsiveness, and performance. Applies to components, pages, dashboards, landing pages, and design system work.
---

# Frontend Design

Use this skill when a task changes how a web interface looks, behaves, or feels.
This skill is for both:
- Building new UI (components, pages, flows, layouts)
- Reviewing existing UI for UX, accessibility, and design quality issues

Do not use this skill for backend-only, API-only, or infra-only work.

Before coding, understand the context and commit to a BOLD aesthetic direction:
- **Purpose**: What problem does this interface solve? Who uses it?
- **Tone**: Pick an extreme: brutally minimal, maximalist chaos, retro-futuristic, organic/natural, luxury/refined, playful/toy-like, editorial/magazine, brutalist/raw, art deco/geometric, soft/pastel, industrial/utilitarian, etc. There are so many flavors to choose from. Use these for inspiration but design one that is true to the aesthetic direction.
- **Constraints**: Technical requirements (framework, performance, accessibility).
- **Differentiation**: What makes this UNFORGETTABLE? What's the one thing someone will remember?


## Core Principles

- Design with intent, not defaults. Every interface should have a clear point of view.
- Function before decoration. Visual style must support user goals and task completion.
- Accessibility is non-negotiable, not a final polish step.
- Responsive behavior is part of design, not an afterthought.
- Motion should communicate state and hierarchy, not distract.
- Performance is UX. Slow or unstable UI is poor UX.

## Workflow

Follow this sequence for every task.

1. Frame the problem
- Identify user type, primary tasks, and context of use.
- Capture hard constraints: framework, deadline, browser/device support, branding rules.
- If key inputs are missing, ask concise questions or make explicit assumptions before coding.

2. Set direction
- Define a visual thesis in one sentence (tone, style, energy).
- Define information hierarchy (what must be seen first, second, third).
- Define interaction thesis (what feedback or motion patterns make this UI feel coherent).

3. Design the system
- Use tokens/variables for color, spacing, radius, shadows, and typography.
- Choose consistent component patterns (buttons, inputs, cards, nav, states).
- Keep a single style language across the feature.

4. Implement
- Build semantic, production-grade code.
- Ensure keyboard support, visible focus states, and accessible labels.
- Implement responsive behavior for small and large screens from the start.

5. Validate
- Run accessibility, responsive, and interaction checks.
- Check for visual consistency and remove generic/template-like patterns.
- Check runtime performance and layout stability.

6. Handoff
- Summarize design direction and major tradeoffs.
- List non-obvious decisions (type, color, spacing, motion, structure).
- Provide clear next-step edits for real content/data integration.

## Build Mode (New UI)

When building UI, ensure these outcomes:
- Distinct visual direction suited to product context
- Clear hierarchy and scannable content
- Cohesive component behavior and interaction states
- Real, runnable code (not pseudo markup)
- Mobile and desktop usability

### Design Guidelines

- Typography: avoid generic stacks when possible; pair display/body fonts intentionally.
- Color: define semantic tokens (`--bg`, `--surface`, `--text`, `--muted`, `--primary`, `--danger`, etc.).
- Layout: favor clear rhythm with an explicit spacing scale (4/8-based is preferred).
- Depth: use elevation, contrast, and borders intentionally; avoid noisy decoration.
- Motion: 150-300ms for micro-interactions; respect `prefers-reduced-motion`.
- Imagery and accents: use them to create identity, not as filler.

## Review Mode (Existing UI)

When reviewing UI, prioritize findings by severity:
- `critical`: breaks task completion, accessibility, or core usability
- `major`: significant UX inconsistency, layout/responsive issues, unclear hierarchy
- `minor`: polish issues that do not block usage

Report findings with:
- Location (`file:line` when available)
- Problem (what fails and why)
- Fix direction (what to change)

## Non-Negotiable UX Checks

- Contrast meets WCAG AA baseline (4.5:1 for normal text).
- All interactive elements are keyboard reachable and have visible focus.
- Icon-only controls include accessible names.
- Forms have visible labels and inline error feedback.
- Touch targets are usable on mobile (target around 44px minimum).
- No horizontal overflow on standard mobile widths.
- Navigation is predictable; active state is clear.
- Motion can be reduced/disabled via user preference.
- Loading, empty, error, and success states are explicit.
- Layout shifts are minimized (reserve space for async content/media).

## Common Anti-Patterns

- Generic template output with no product-specific visual identity
- Placeholder-only form labels
- Hover-only interactions with no keyboard/touch equivalent
- Over-animation or zero-motion snap transitions
- Inconsistent spacing/radius/shadow values across components
- Decorative effects that reduce readability or contrast
- Large component APIs with many booleans instead of composable patterns
- Shipping without mobile checks

NEVER use generic AI-generated aesthetics like overused font families (Inter, Roboto, Arial, system fonts), cliched color schemes (particularly purple gradients on white backgrounds), predictable layouts and component patterns, and cookie-cutter design that lacks context-specific character.

Interpret creatively and make unexpected choices that feel genuinely designed for the context. No design should be the same. Vary between light and dark themes, different fonts, different aesthetics. NEVER converge on common choices (Space Grotesk, for example) across generations.

**IMPORTANT**: Match implementation complexity to the aesthetic vision. Maximalist designs need elaborate code with extensive animations and effects. Minimalist or refined designs need restraint, precision, and careful attention to spacing, typography, and subtle details. Elegance comes from executing the vision well.

Remember: You are capable of extraordinary creative work. Don't hold back, show what can truly be created when thinking outside the box and committing fully to a distinctive vision.