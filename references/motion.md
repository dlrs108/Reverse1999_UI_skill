# Motion System

Reverse: 1999 NEVER uses standard web `ease-in-out`. It combines "Paper, Film, and CRT".

## Core Easing
- `--ease-snap`: `cubic-bezier(0.2, 0.9, 0.3, 1.2)` (Fast-in, slow-out, used for modals, cards).
- `--ease-flicker`: `steps(4, end)` (Glitch, CRT flicker).

## 7 Signature Animations

### A. Paper Growth (Modals, Horizontal Alerts)
- DO NOT scale from center. 
- Use horizontal `clip-path` or `width` animation from one side with a distinct pause. 
- Vertical cards use `transform: rotateX()` simulating unrolling.

### B. Film Stagger (Lists, Cards)
- Elements appear sequentially (`animation-delay` +50ms).
- `opacity: 0` & `translateY(10px)` with brief `filter: blur(4px)` fading to clear.

### C. CRT Power-On (Screen transitions, Dark Modals)
- A horizontal scanline appears first, stretching vertically to fill the panel in 0.15s. Text fades in left-to-right like a typewriter.

### D. Vacuum Tube Glow (Hover states)
- Use `::before` with `radial-gradient(circle, rgba(255,180,100,0.3) 0%, transparent 70%)`.
- On hover, opacity 0 to 1, scale up slightly.

### E. ASCII Drift (Background decoration)
- `Courier New` green/gold characters (`0`, `>`, `*`), extremely low opacity drifting from bottom to top slowly (10s-20s loop).

### F. Constellation Charge (Energy full)
- Use SVG `stroke-dasharray` and `stroke-dashoffset`. Lines light up tracing the path.
- Nodes snap: `scale(1.5) -> scale(1)`.

### G. Glitch Hover (Primary buttons)
- Borders and text have a red/cyan offset layer shifting by 1px for 0.1s.
