# Tinkerer Octocat

This repository contains the original "Tinkerer Octocat" designs prepared for the GitHub Octocat Drawing Contest.

Included files:
- `ratchet-tinkerer-neon-cyberpunk.svg` — Neon cyberpunk palette (static vector).
- `ratchet-tinkerer-animated.svg` — Same artwork with a simple tentacle sway animation (open in a browser to view).
- `ratchet-tinkerer-action-pose.svg` — Action pose with wrench raised.

What the repository will do:
- A GitHub Actions workflow is included to render high-resolution PNG exports from the SVGs and commit them back into `exports/`.

How to get the files locally (Windows):
1. Open PowerShell.
2. Clone the repository into the folder you requested:
   git clone https://github.com/best-ed/tinkerer-octocat "C:\dev\challenges"

Where PNGs will appear after Actions runs:
- After the workflow runs, look for the generated files in `exports/` inside the repo (e.g. `exports/ratchet-tinkerer-neon-cyberpunk.png`).

Manual trigger / re-run the workflow:
- In GitHub: Actions → Render SVGs → Run workflow (workflow_dispatch) to render PNGs on demand.

Notes:
- The workflow will skip re-rendering if it detects the render marker in the last commit message to avoid loops.

