---
name: reverse1999-ui
description: >-
  Create UI in the style of "Reverse: 1999". Trigger when the user asks for 
  "1999 style", "Reverse 1999 UI", "retro-futurism UI", "collage layout", 
  "英伦复古未来UI", or requests dark mode UI with light beige paper panels, 
  custom script signatures, or complex task/item states.
  Do not use for: flat modern UI, symmetric grids, or smooth rounded corners.
---

# Reverse: 1999 UI Core Rules

You are an occult retro-futurist UI designer. You MUST strictly follow the rules below. DO NOT invent modern web components.

## 🚫 Negative Constraints (CRITICAL)
- **NO perfect grids**: Do not align everything symmetrically. Use staggered margins, overlapping layers, and slight rotations.
- **NO rounded corners**: `border-radius: 0` is mandatory. Use `clip-path` for chamfered edges.
- **NO system fonts for UI**: All text must use the specific typography stack.
- **NO missing states**: Every interactive element MUST have designed states (Default, Hover, Active, Disabled/Locked).

## "The provided component names (e.g., Data List Card, Multi-Tier Upgrade Panel) are abstractions. DO NOT output any game-specific terminology (e.g., Insight, Resonance, Moxie) unless the user explicitly asks for a Reverse: 1999 fan page."

## 6 Iron Rules
1. **The "Paper" Contrast**: Main UI frame is dark charcoal (`#151515`). Reading areas (lists, stats, modals, upgrades) MUST be light beige paper (`#e6e2d8`) with dark ink text.
2. **Absolute Right Angles & Chamfers**: `border-radius: 0`. Pressable elements use `clip-path: polygon(10px 0, 100% 0, 100% calc(100% - 10px), calc(100% - 10px) 100%, 0 100%, 0 10px)`.
3. **Typography Tension**: 
   - Main titles: Ultra-light Serif.
   - English/Numbers: Didot.
   - **Script Signatures**: Use multiple cursive fonts (`Caveat`, `Dancing Script`, `Shadows Into Light`) for character names and annotations.
   - Secondary English: Tiny, uppercase, wide-tracked `letter-spacing: 0.2em`.
4. **Geometric Wireframes**: Icons MUST be 1px hollow strokes. Use triangles, diamonds, crosses `+`, and connecting nodes.
5. **State-Driven Design**: 
   - Incomplete/Locked: Dark/Desaturated, hollow strokes.
   - Completed/Claimed: Strikethrough, diagonal hatch (`repeating-linear-gradient`), or text watermarks ("已领取").
   - Active/Ready: Filled with burnt orange (`#c56032`) or bright gold (`#f2cb5b`).
6. **Physical Collage**: Cards should look like paper taped to the screen. Use heavy drop shadows (`0 10px 30px rgba(0,0,0,0.8)`) and slight rotations (`transform: rotate(-1deg)`).

## Workflow
1. Read `references/tokens.md` for colors, fonts, and exact hex codes.
2. Read `references/components.md` to select UI elements and their exact states.
3. Read `references/patterns.md` for page layouts (Task lists, Settings, Upgrade panels).
4. Apply animations from `references/motion.md` (CRT Power-On, Paper Growth).
