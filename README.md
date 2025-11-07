# Tic-Tac-Toe
Simple, lightweight Tic-Tac-Toe game built with only HTML, CSS and vanilla JavaScript — no frameworks, no build step. Perfect for beginners who want a compact example of DOM manipulation, game state management, and simple UX.

## How to run

1. Clone or download the repo.
2. Open `index.html` in your browser (double-click or `File → Open`).

No web server or build tools required.

## Gameplay

- Two players alternate turns placing X and O.
- The first player to align 3 of their marks horizontally, vertically or diagonally wins.
- If all 9 squares are filled with no winner, the game ends in a draw.
- Use the **Reset** button to start a new game.

## Files

- `index.html` — markup and minimal inline CSS (or link to `styles.css` if you split it).
- `script.js` — game logic: board state, player turns, win/draw detection, UI updates.

## How it works (brief)

- The board is represented as a 1D array of 9 cells `['', '', ...]`.
- When a cell is clicked:
  - If the cell is empty and the game is ongoing, set it to the current player's symbol (`'X'` or `'O'`).
  - Update the DOM to show the symbol.
  - Check for a win using a fixed list of winning index combinations.
  - If a win is found, highlight the winning cells and stop further input.
  - If no win and the board is full, declare a draw.
  - Otherwise, toggle the current player.
- The Reset button clears the board and resets state.

## Possible improvements

- Add an AI opponent (minimax algorithm) for single-player mode.
- Add animations and sound effects.
- Keep persistent score using `localStorage`.
- Add keyboard controls and accessibility features (ARIA attributes).
- Make the board size configurable (n×n Tic-Tac-Toe).

## License

MIT License — feel free to reuse and modify.
