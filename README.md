# Tic Tac Toe Game

This is a **Python-based Tic Tac Toe game** that supports both **single-player** (against a computer using the Minimax algorithm) and **multiplayer** modes.

## Features
- **Single Player Mode**: Play against the computer, which uses the Minimax algorithm to make optimal moves.
- **Multiplayer Mode**: Two players can play alternately.
- **Dynamic Board Visualization**: Displays the current state of the board after every turn.
- **Winning Conditions**: Detects and announces the winner or declares a draw when all positions are filled.

---

## How to Run
1. Ensure you have **Python 3.x** installed on your system.
2. Save the script in a `.py` file, e.g., `tic_tac_toe.py`.
3. Run the script:
   ```bash
   python tic_tac_toe.py
   ```

---

## How to Play
1. When the game starts, you will be prompted to choose:
   - **1** for single-player mode.
   - **2** for multiplayer mode.
   
2. In **single-player mode**:
   - Choose whether you want to play as the **1st** player (`X`) or the **2nd** player (`O`).
   - The computer will play optimally using the Minimax algorithm.

3. In **multiplayer mode**:
   - Players take turns entering positions (`1-9`) to place their markers (`X` or `O`).

4. The board is represented as a 3x3 grid with positions numbered as follows:
   ```
   1 | 2 | 3
   ---------
   4 | 5 | 6
   ---------
   7 | 8 | 9
   ```

5. Enter the position number to place your marker.

6. The game announces:
   - **"X Wins!!!"** if player `X` wins.
   - **"O Wins!!!"** if player `O` (or the computer) wins.
   - **"Draw!!!"** if the game ends with no winner.

---

## Key Components
1. **Minimax Algorithm**:
   - Used by the computer to calculate the best possible move.
   - Considers all possible outcomes and selects the move that minimizes the opponent's chances of winning.

2. **Functions**:
   - `ConstBoard(board)`: Displays the current state of the board.
   - `User1Turn(board)`: Handles player `X`'s turn.
   - `User2Turn(board)`: Handles player `O`'s turn (multiplayer mode).
   - `CompTurn(board)`: Handles the computer's move.
   - `analyzeboard(board)`: Checks if there's a winner or a draw.
   - `minimax(board, player)`: Implements the Minimax algorithm.

---

## Example Gameplay
**Single Player:**
```
Enter 1 for single player, 2 for multiplayer: 1
Computer : O Vs. You : X
Enter to play 1(st) or 2(nd): 1
Current State Of Board: 
- - -
- - -
- - -
Enter X's position from [1...9]: 5
```

**Multiplayer:**
```
Enter 1 for single player, 2 for multiplayer: 2
Current State Of Board:
- - -
- - -
- - -
Enter X's position from [1...9]: 1
Current State Of Board:
X - -
- - -
- - -
Enter O's position from [1...9]: 2
```

---

## Future Enhancements
- Add a graphical interface (e.g., using `tkinter` or `pygame`).
- Add a scoring system to track wins, losses, and draws across multiple games.
- Allow customization of the grid size (e.g., 4x4 or 5x5 Tic Tac Toe).

---

Enjoy the game! 🎮
