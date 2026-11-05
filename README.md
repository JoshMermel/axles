# axles
A logic puzzle about turning axles, on square or hexagonal boards.

**Play it: https://joshmermelstein.com/axles/**

Turn every arrow so it points straight up. Tap a cell to rotate it one step clockwise. The catch: a dot on a cell's edge blocks the neighbor it points at, and a blocked cell can't turn. Dots rotate along with their cell, so turning one cell can free up (or block) others.

- **Square board** (2x2 up to 6x6). Hard mode adds dots on the corners that block diagonally.
- **Hex board** (7, 19 or 37 cells). Six neighbors, 60 degree turns.
- Easy / Normal / Hard control how many dots there are. Every generated puzzle is solvable.

Inspired by https://twistypuzzles.com/forum/viewtopic.php?t=39375 but on a square grid.

I used Gemini for the proof of concept and then refined the UI and the puzzle generation logic by hand. Claude later helped with the help modal, the hex board, and a code review.

The whole game is a single `index.html` (React + Babel loaded from a CDN), so there is no build step.
