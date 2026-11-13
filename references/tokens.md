# Design Tokens

## Colors
- `--bg-dark`: `#151515` (Main background)
- `--bg-panel-dark`: `#1e1e1e` (Dark UI panels)
- `--paper-light`: `#e6e2d8` (Light beige for tasks, lists, modals)
- `--paper-white`: `#f4f0ea` (Brighter paper for character items)
- `--ink-dark`: `#1a1a1a` (Text on paper)
- `--ink-light`: `#eaeaea` (Text on dark)
- `--accent-orange`: `#c56032` (Primary CTA, active tabs, highlights)
- `--accent-gold`: `#f2cb5b` (Energy full, special rarity)
- `--state-disabled`: `#555555` (Locked text/icons)
- `--danger-red`: `#9e3e35` (Delete only)

## Typography
- **CJK Main**: `"Noto Serif SC", "Songti SC", serif` (Ultra-light for titles, regular for body).
- **English Accent**: `"Didot", "Bodoni MT", serif` (High contrast).
- **Script Pool (CRITICAL)**: Use a `<style>` import for multiple script fonts and apply them randomly: `"Caveat", "Dancing Script", "Shadows Into Light", cursive`. 
- **Micro English**: `font-size: 10px; letter-spacing: 0.2em; text-transform: uppercase;`

## UI Elements
- `--border-thin`: `1px solid rgba(255,255,255,0.2)`
- `--border-ink`: `1px solid rgba(0,0,0,0.3)`
- `--hatch-pattern`: `repeating-linear-gradient(45deg, transparent, transparent 2px, rgba(0,0,0,0.1) 2px, rgba(0,0,0,0.1) 4px)`
