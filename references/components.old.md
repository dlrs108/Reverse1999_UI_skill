# Components

## 1. Notice Modal
- **Overlay**: Full screen black semi-transparent (`backdrop-filter: blur(4px)`).
- **Title**: `^` wireframe symbol above, "提示" center, "NOTICE" small below.
- **Body**: Full-width light-beige banner (`background: var(--modal-light)`). Black serif text.
- **Buttons**: Two chamfered buttons at bottom. Cancel (white/light gray pattern), Confirm (orange with dark geometric line pattern). Top-right of buttons MUST have a tiny downward triangle.

## 2. Poster Carousel (Collage)
- Overlapping layers. Active card enlarged; adjacent cards tilted and stacked behind like VHS tapes.
- Layout: Poster art on top, Serif CJK title + tiny English typography below.

## 3. Combat Status UI
- **Health Bar**: Parallelogram (`clip-path: polygon(5% 0, 100% 0, 95% 100%, 0% 100%)`). Dark green filling, dark red background.
- **Moxie Slots**: Row of 5 diamonds below health bar. Empty: hollow stroke `◇`. Full: solid bright `◆`. Emits a breathing glow when full.
- **Combat Cards**: Right-angled rectangles. High-contrast printmaking/silhouette art. Thin colored bar at bottom with English labels (ATTACK, BUFF).

## 4. The Scale (Constellation Energy)
- NO standard progress bars.
- Use SVG polygons and connected nodes. Floating elliptical coil with numbers on the left.
- Low energy: Dark gold lines (`opacity: 0.3`). High energy: Nodes glow, lines turn bright yellow.

## 5. Nav & Icons
- 1px hollow strokes only.
- Active state: Icon brightens, rough orange hand-drawn underline appears below, accompanied by cursive English scribbles.
