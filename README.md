# ココAI design directions

Clickable prototypes of the ココAI chat panel for KokoMart, one folder per design direction,
so the team can compare them side by side. Products, prices and chat replies are sample data;
nothing talks to the real Agent API.

- `index.html`: the chooser page that links to every direction, with a desktop and a phone screenshot of each
- `previews/`: those screenshots (`<letter>-desktop.webp`: the panel showing the set results; `<letter>-phone.webp`: what the AI tab opens), captured at 2x in headless Chrome
- `direction-a/`: 案A, white panel with a soft glow, floating round controls, compact set cards
- `direction-b/`: 案B, dark full-height panel with drifting aurora light, glass surfaces, sets side by side to swipe
- `direction-c/`: 案C, AI-search stage: one big box, a step checklist while it works, sets compared in columns
- `direction-d/`: 案D, guided concierge in a bottom sheet: one question per screen with big tiles, one best-match result

## Adding a direction

1. Create the next folder, e.g. `direction-e/index.html` (a complete, self-contained HTML page).
2. Add a card for it in `index.html`, with its two screenshots in `previews/`.
3. Commit and push. GitHub Pages republishes within a minute or two.

## Hosting

GitHub Pages serves the `main` branch from the repository root
(Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)`).
`.nojekyll` makes Pages serve the files as they are.
