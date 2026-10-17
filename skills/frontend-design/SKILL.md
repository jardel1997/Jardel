---
name: frontend-design
description: Create distinctive, premium, production-ready websites with strong visual identity, polished typography, purposeful motion, responsive layouts, accessibility, and performance. Use whenever creating or redesigning a website, landing page, portfolio, or frontend UI.
---

# Frontend Design Skill — Jardel's Website Quality Standard

## Mission
Build memorable, polished, context-specific websites. Avoid generic AI-generated layouts and make every design decision intentional. The result must be both visually excellent and genuinely functional.

## Required workflow
1. **Inspect first.** Review the existing repository, framework, package scripts, assets, components, and design constraints before changing code.
2. **Understand the business.** Identify audience, conversion goal, brand personality, content, and the single most memorable visual idea.
3. **Choose a clear art direction.** Commit to a coherent design concept rather than combining random trends. Document palette, typography, composition, imagery, motion, and spacing.
4. **Build working code.** Implement the real interface and interactions. Do not stop at mockups, descriptions, or static hero sections.
5. **Polish deliberately.** Review desktop, tablet, and mobile, fix awkward spacing and overflow, and check every interaction.
6. **Validate.** Run available lint, type-check, build and tests. Fix errors introduced by your changes and report any remaining blockers honestly.

## Visual quality rules
- Create a specific visual identity that fits the business, audience, and reference.
- Use a deliberate palette with dominant colors and a controlled accent; define reusable CSS variables/design tokens.
- Pair a distinctive display typeface with a highly readable body typeface. Avoid defaulting automatically to Arial, Roboto, or Inter.
- Use a clear hierarchy, precise spacing, strong alignment, generous negative space, and intentional asymmetry where appropriate.
- Use high-quality, context-relevant photography, product imagery, illustration, or 3D assets. Never use broken images or unrelated stock imagery as final content.
- Make backgrounds atmospheric when the concept calls for it: subtle texture, gradients, layered surfaces, light, depth, or restrained shadows.
- Make buttons, links, navigation, forms, cards, and hover/focus states feel designed as one consistent system.
- Favor a few strong, memorable moments over dozens of decorative effects.
- Do not repeat the same layout, color scheme, hero composition, or card grid across unrelated sites. Each website must feel designed for its own business.

## Anti-generic checklist — never ship these by default
- A generic hero with a heading, two buttons, and three identical cards without a differentiated concept.
- Overused purple-on-white gradients, glassmorphism everywhere, excessive rounded cards, random blobs, or arbitrary glowing borders.
- Generic icons or emojis used in place of real brand imagery.
- Excessive centered content with no variation in composition.
- Stock photos that do not represent the business.
- Placeholder copy, fake reviews, invented statistics, fake awards, or unsupported claims.
- Decorative animations that do not support storytelling, hierarchy, or usability.
- A beautiful screenshot with nonfunctional controls.

## Motion and interaction
- Motion must reinforce the concept and guide attention.
- Use a coordinated page-load sequence, purposeful scroll reveals, polished hover/focus states, and coherent transitions.
- Keep animations smooth and avoid animating many unrelated elements simultaneously.
- For scroll storytelling, prefer GSAP + ScrollTrigger when suitable; use Three.js/WebGL only when actual 3D adds value and assets/performance allow it.
- Handle resize, cleanup, reduced-motion preferences, and mobile differences.
- Do not lock scrolling for long periods or allow animation to hide important content.
- Provide a graceful fallback when WebGL or heavy effects are unavailable.
- Never claim an image-based parallax effect is a true 3D model.

## Content and conversion
- Write specific, concise copy appropriate to the real business and its audience.
- Establish one clear primary action, supported by sensible secondary actions.
- Make contact details, pricing, services, products, and other business facts configurable.
- Every visible button or link must have a real, appropriate action. Never simulate a successful form submission if nothing was actually sent or stored.
- Do not fabricate business facts. Clearly mark unknown values for replacement.

## Responsive design
- Design mobile deliberately; do not merely shrink desktop.
- Verify common narrow widths, tablet, laptop, and wide desktop.
- Prevent horizontal overflow, clipped headings, overlapping fixed elements, and unreadable text.
- Support touch interaction and do not rely on hover.
- Respect prefers-reduced-motion and retain access to core content when animation is disabled.

## Accessibility and SEO
- Use semantic HTML, logical heading order, accessible labels, visible focus states, useful alt text, and sufficient contrast.
- Do not put essential text only inside images, canvas, or WebGL scenes.
- Preserve crawlable text and real internal links.
- When relevant, implement unique titles and meta descriptions, canonical URLs, Open Graph metadata, sitemap/robots setup, appropriate structured data, local business details, and descriptive image alternatives.
- Never promise top Google rankings.

## Code quality and performance
- Preserve the existing stack unless there is a concrete reason to change it.
- Reuse the project's components and conventions; avoid unnecessary dependencies and rewrites.
- Separate reusable components, content data, styling tokens, and animation logic when appropriate.
- Optimize image formats and dimensions, lazy-load below-the-fold assets, defer heavy 3D, and avoid layout shifts.
- Do not introduce console errors, broken imports, invalid links, or nonfunctional navigation.
- Keep code maintainable and explain non-obvious implementation decisions.

## Final review gate
Before finishing, confirm:
- [ ] The design is distinctive and business-specific.
- [ ] Typography, colors, spacing, imagery, and components form one cohesive system.
- [ ] The main visual idea is immediately apparent.
- [ ] All controls and contact actions work.
- [ ] Mobile and desktop layouts are both polished.
- [ ] Animations are purposeful, performant, and reduced-motion aware.
- [ ] Content and business facts are accurate or clearly marked as placeholders.
- [ ] Relevant accessibility and SEO basics are in place.
- [ ] Build/lint/tests were run when available and errors were addressed.
- [ ] Remaining limitations are reported honestly.

**Operating rule:** Do not settle for the first acceptable-looking result. Refine the actual implementation until it looks intentional, coherent, premium, and specific to the project.
