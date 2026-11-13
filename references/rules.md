# Rules (Do & Do Not)

## MUST DO
- **Right Angles & Chamfers**: `border-radius: 0` is MANDATORY. All interactive elements must use straight corners or `clip-path` chamfers.
- **High Contrast (Dark Frame + Light Paper)**: The main canvas is deep charcoal/blue-black. Content blocks, reading areas, and modals MUST be light beige paper (`#e6e2d8`) with dark ink text.
- **Physical Staggering & Collage**: DO NOT align cards symmetrically. Use `transform: rotate(-1deg to 1deg)`, overlapping margins, and heavy, hard-edged drop shadows to simulate physical paper taped to the screen.
- **Extreme Typographic Contrast**: Combine massive English serif watermarks (semi-transparent) + ultra-light CJK Serif text + tiny, wide-tracked uppercase English tags (e.g., `letter-spacing: 0.2em`, `font-size: 10px`).
- **Dense Data Layouts**: Use 1px solid lines to separate list items. Numbers, dates, and indices must use tabular figures (e.g., `01`, `2026.10`).
- **Script Annotations**: Use cursive fonts (e.g., `Caveat`, `Dancing Script`) for character signatures, sub-headers, or hand-drawn circling/underlining effects.

## DO NOT
| NEVER DO THIS | WHY |
| --- | --- |
| Use rounded corners, pill buttons, or standard Material cards | Instantly destroys the vintage archive aesthetic. |
| Use perfect centering or rigid, symmetrical grid layouts | The core essence of 1999 is "staggered, collaged, scattered." |
| Use smooth CSS gradients or soft `box-shadow` | Use hard edges, 1px wireframes, or diagonal hatching (`repeating-linear-gradient`) instead. |
| Fill large areas with saturated colors | 90% of the UI is black/white/beige. Orange (`#c56032`) is ONLY for active tabs, primary buttons, and key highlights. |
| Put long paragraphs of text directly on a dark background | Text MUST be placed on the light beige paper panels. |
| Use default system form controls (`<select>`, `<input type="range">`) | They must be custom-built with chamfered rectangles and diamond-shaped thumbs. |
