# Motion System

## Core Easing
- `--ease-snap`: `cubic-bezier(0.2, 0.9, 0.3, 1.2)` (For modals, cards appearing).
- `--ease-flicker`: `steps(4, end)` (For glitch, CRT transitions).

## Animations
1. **CRT Power-On**: When a paper modal opens, a 1px horizontal line appears first, then stretches vertically to fill the panel in 0.15s. Text follows with a typewriter effect.
2. **Paper Unroll**: Cards should not just fade in. Use `transform: rotateX(90deg) to rotateX(0)` to simulate a paper unrolling.
3. **Glitch Hover**: On button hover, add a 1px text-shadow offset (`text-shadow: 1px 0 red, -1px 0 cyan;`) for 0.1s.
4. **Constellation Charge**: For energy bars, use SVG `stroke-dasharray` to draw lines sequentially, making nodes pop (`scale(1.5) -> scale(1)`) as they connect.
