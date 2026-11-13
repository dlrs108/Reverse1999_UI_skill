# Layout Patterns

## 1. Archive Data List (e.g., System Logs, Task Trackers, Notifications)
- **Background**: Dark canvas with a subtle geometric watermark or noise texture.
- **Cards**: Horizontal light beige paper cards. Left column features a massive, faded decorative number (e.g., `01`) with 3 small orange dots below it.
- **Staggering**: Alternating cards must have slight left/right offsets (`margin-left: 1%`, `margin-right: -1%`) to create a physical stack.
- **States**: 
  - Default/Pending: Clean paper.
  - Completed/Archived: Apply a 45° diagonal hatch pattern (`--hatch-pattern`) over the card and add a large, semi-transparent watermark text (e.g., "ARCHIVED") across it.

## 2. Magazine Dossier (e.g., User Profiles, Product Details, Long-form Articles)
- **Typography**: Simulate a vintage magazine. Use a massive orange Drop Cap (首字下沉) for the first letter of the text block. Use justified text with tight line-height.
- **Watermarks**: Place huge, semi-transparent serif English letters (e.g., "PROFILE", "DOSSIER") in the background behind the text.
- **Geometric Accents**: Use 1px hollow wireframes (e.g., overlapping triangles, intersecting lines) as visual anchors.
- **Signatures**: Place a tilted, handwritten cursive signature near the title or main image. 

## 3. Immersive Dashboard (e.g., Analytics, Settings, Checkout Flow)
- **Chamfered Navigation**: Tabs at the top must be chamfered rectangles. The active tab is filled with burnt orange (`#c56032`) and has a tiny downward triangle `▼` in the corner.
- **Constellation Gauges**: NEVER use standard progress bars. Use SVG to draw a network of nodes and thin lines. Light up the nodes sequentially to show progress.
- **Form Controls**: 
  - Dropdowns: Dark panels with 1px borders.
  - Sliders: The thumb must be a diamond shape (`width: 12px; height: 12px; transform: rotate(45deg); background: var(--accent-orange); border-radius: 0;`).
