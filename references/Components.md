# Components & States (Abstracted)

## 1. Data List Card (Paper Style)
*Replaces the "Task List" component.*
- **Container**: Light beige paper (`var(--paper-light)`), dark ink text. Heavy shadow (`0 10px 30px rgba(0,0,0,0.8)`).
- **Left Column**: Large, faded decorative number (e.g., `01`) with 3 small orange dots below it.
- **State: Incomplete / Pending**
  - Normal colors. Action button (e.g., "Edit", "View") has a thin border.
- **State: Completed / Claimed**
  - Apply a diagonal hatch pattern (`--hatch-pattern`) over the container.
  - Add a large, semi-transparent watermark text (e.g., "COMPLETED") across the card.
  - Action button is disabled (`:disabled`), replaced by a slashed-circle icon `⊘`.

## 2. Collectible Item Card (Portrait Style)
*Replaces the "Character Belongings" component.*
- **Container**: Vertical paper card (`var(--paper-white)`), sharp corners.
- **State: Locked**
  - Apply `opacity: 0.5; filter: grayscale(100%)`. 
  - Show a lock icon 🔒 and text (e.g., "Unlock at Level 100").
- **State: Unlockable**
  - Full color. Show a highlighted badge or text in `var(--accent-orange)`.
- **State: Unlocked**
  - Normal paper card, no lock icon.

## 3. Advanced Form Controls (Settings)
- **Custom Dropdown**: Do NOT use native `<select>`. Create a div with `border: 1px solid rgba(255,255,255,0.4)`, background transparent. When opened, the dropdown list is a dark panel with 1px borders. The active option has an orange background and a small downward triangle `▼`.
- **Diamond Slider**: The track is a 2px solid line. The thumb is a diamond shape: `width: 12px; height: 12px; transform: rotate(45deg); background: var(--accent-orange); border-radius: 0;`.
- **Rectangular Toggle**: Not a pill. Active = `var(--accent-orange)` block. Inactive = dark gray block.

## 4. Multi-Tier Upgrade Panel
*Replaces the "Insight/Breakthrough" component.*
- **Main Visual**: A large, intersecting geometric shape (e.g., three overlapping triangles) made of 1px glowing lines.
- **Content**: A list of attribute increases (e.g., "Base ATK +10"). Use tiny, wide-tracked English text next to Chinese labels.
- **Action Button**: Full-width, chamfered right edge, filled with `var(--accent-orange)`.

## 5. Notice Modal (Paper style)
- Full screen dark overlay with `backdrop-filter: blur(4px)`.
- Central panel: `background: var(--paper-light)`.
- Title: Centered, with a `^` wireframe symbol above.
- Buttons: Cut-corner rectangles. Confirm button is `var(--accent-orange)`.
