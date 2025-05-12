# Chess AI Game using Minimax Algorithm

This is a graphical chess game built with Python using Pygame. The game supports human vs AI, human vs human, and includes a custom chess engine and AI opponent using a Minimax algorithm with alpha-beta pruning and quiescence search.

## 🧠 Features

- Playable chess game with graphical interface
- AI opponent using Minimax with Alpha-Beta pruning
- Quiescence search for more accurate evaluation in tactical positions
- Piece-square evaluation tables for better positional play
- Castling, en passant, promotion, and checkmate logic fully implemented
- Move history panel with clickable undo
- Keyboard shortcuts:
  - `Z`: Undo move
  - `R`: Reset game
  - `Q`: Set AI as white
  - `E`: Set AI as black

## 📁 Project Structure

```
.
├── ChessMain.py       # Main file to run the game with GUI
├── ChessEngine.py     # Core engine handling game logic, rules, and board state
├── AgentMimax.py      # AI logic using Minimax algorithm with alpha-beta pruning
└── images/            # Folder containing chess piece images (e.g., wp.png, bQ.png, etc.)
```

## ▶️ How to Run

1. **Install dependencies**
   ```bash
   pip install pygame
   ```

2. **Prepare assets**
   - Create a folder named `images/` in the same directory as the scripts.
   - Add images of chess pieces named: `wp.png`, `wR.png`, ..., `bK.png`.

3. **Run the game**
   ```bash
   python ChessMain.py
   ```

## 🎮 Controls

- Click squares to select and move pieces
- Moves are highlighted
- Move history displayed to the right (click to rewind)

## 🤖 AI Strategy

The AI in `AgentMimax.py` uses:

- Minimax with Alpha-Beta pruning
- Quiescence Search (up to depth 5)
- Evaluation based on material and positional piece-square tables
- Transposition table to reduce repeated evaluations

## 📌 Notes

- The AI's depth is fixed to 3 by default for performance reasons.
- The AI will automatically play when it's its turn if enabled via keypresses (`Q` or `E`).
- The GUI supports undo and reset for ease of play and testing.

## 📷 Screenshots

> (Add images of the gameplay and UI here)

## 📜 License

This project is open source and can be freely used or modified for educational purposes.