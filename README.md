# Tower Defence Game

This is a classic tower defence game where players strategically place towers to defend against waves of enemies. The game features:

- **Strategic Tower Placement**: Choose from a variety of towers with unique abilities.
- **Wave-based Combat**: Defend against increasingly challenging waves of diverse enemies.
- **Upgradable Towers**: Enhance your towers to improve their damage, range, and special effects.
- **Multiple Levels**: Play through different levels, each with unique layouts and challenges.
- **Responsive UI**: The game interface adapts to various screen sizes for an optimal experience on different devices.
- **Dynamic Update Logs**: Stay informed with in-game updates and version history, dynamically loaded from a CSV file.

## How to Play

1. **Place Towers**: Select a tower from the available options and place it on designated spots on the map.
2. **Defend**: Watch your towers automatically attack incoming enemies.
3. **Upgrade**: Earn in-game currency by defeating enemies and use it to upgrade your towers or build new ones.
4. **Survive**: Prevent enemies from reaching the end of the path to win the level.

## Features to be added:

- More diverse enemies and boss battles.
- Additional tower types with unique mechanics.
- Special abilities and power-ups for players.
- A campaign mode with a compelling storyline.
- Leaderboards and achievements.

Enjoy defending your territory!

## Local Debug Menu (Development Only)

- The debug menu is available only in local development via a separate script `debug-local.js`.
- This file is excluded from version control by `.gitignore`, ensuring no debug code ships to production.
- The game’s main module conditionally loads the debug script if it exists; otherwise, no debug UI or logic is included.

### Enabling Locally
- Keep `debug-local.js` in the project root (same folder as `index.html`).
- Start a local server (e.g., `python3 -m http.server 8000`) and open `http://localhost:8000/index.html`.
- Press `D` to toggle the debug menu in the browser.

### Verification
- Run `git status` to confirm `debug-local.js` is ignored and not staged.
- Remove or rename `debug-local.js` to simulate a production build; the debug UI will not load.
