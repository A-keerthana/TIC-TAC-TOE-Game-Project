

# TIC-TAC-TOE Game Project 🎮

## Overview
This is a **Tic-Tac-Toe** game implemented in Python. It supports both **single-player (AI vs Player)** and **multiplayer (Player vs Player)** modes. The game allows users to play in a turn-based manner, with a simple AI using the **Minimax algorithm** for decision-making.

## Features
✅ Supports **Single Player (against AI)** and **Multiplayer** modes.  
✅ AI uses the **Minimax Algorithm** for optimal moves.  
✅ Simple **console-based interface** for easy gameplay.  
✅ Detects win/loss/draw conditions automatically.  

## Installation

### Prerequisites
Ensure you have **Python 3.6+** installed on your system.

### How to Run
1. Clone this repository or download the `main.py` file.
2. Open a terminal/command prompt in the project directory.
3. Run the script:
   ```bash
   python main.py
   ```
4. Follow the on-screen instructions to play the game.

## How to Play
1. **Select Game Mode**  
   - Enter `1` for **Single Player Mode** (You vs AI).  
   - Enter `2` for **Multiplayer Mode** (Player X vs Player O).  

2. **Turn-based Gameplay**  
   - Players take turns placing `X` or `O` in a **3x3 grid**.
   - Input a position from `1-9` (corresponding to board positions).
   - The game detects **win conditions** and declares the winner.

3. **Winning Conditions**  
   The game ends when:
   - A player aligns **three symbols in a row, column, or diagonal** (Winner declared).
   - The board is full (Result: **Draw**).

## File Structure
```
📂 TIC-TAC-TOE-Game-Project
 ├── TIC_TAC_TOE_Game_Project.ipynb  # Jupyter Notebook Implementation
 ├── README.md                        # Project Documentation
```

## Game Logic Breakdown
- **Board Representation:** The game board is stored as a **1D list** of size `9`.
- **Minimax Algorithm:** The AI evaluates the best possible move.
- **User Input Handling:** Ensures valid moves and prevents overwrites.
- **Win Condition Checks:** The game detects win/loss/draw conditions.

## Example Gameplay

---

#### **Step 1: Choose Game Mode**
When you run the script, you will be prompted to choose the game mode:
```
Enter 1 for Single Player, 2 for Multiplayer: 2
```
- If you enter **1**, you will play against the computer (AI).  
- If you enter **2**, you will play against another player.

#### **Step 2: Initial Board State**
The game starts with an empty **3x3 grid**, where each position is represented by `_` (underscore):

```
Current State of the Board: 

_  _  _  
_  _  _  
_  _  _  
```
Each position in the grid is mapped to a number from **1 to 9**, like this:

```
1  2  3  
4  5  6  
7  8  9  
```
When a player chooses a position, their symbol (`X` or `O`) replaces `_` at the corresponding spot.

---

### **Step 3: Players Take Turns**
The game prompts **Player X** to make a move:
```
Enter X's position from [1-9]: 1
```
If Player X chooses **position 1**, the updated board looks like this:

```
X  _  _  
_  _  _  
_  _  _  
```
Now, it’s **Player O's** turn:
```
Enter O's position from [1-9]: 5
```
If Player O places their move at **position 5**, the board updates:

```
X  _  _  
_  O  _  
_  _  _  
```

---

### **Step 4: Continue Playing**
The game continues as players take turns:

```
Enter X's position from [1-9]: 9
```
After Player X chooses **position 9**:

```
X  _  _  
_  O  _  
_  _  X  
```

```
Enter O's position from [1-9]: 2
```
After Player O places **position 2**:

```
X  O  _  
_  O  _  
_  _  X  
```

```
Enter X's position from [1-9]: 8
```
Player X updates **position 8**:

```
X  O  _  
_  O  _  
_  X  X  
```

```
Enter O's position from [1-9]: 7
```
Player O updates **position 7**:

```
X  O  _  
_  O  _  
O  X  X  
```

---

### **Step 5: Winning Condition**
The game continues until one player **wins** or the board is **full (draw).**

```
Enter X's position from [1-9]: 3
```
Player X places their move at **position 3**:

```
X  O  X  
_  O  _  
O  X  X  
```

```
Enter O's position from [1-9]: 6
```
Player O places **position 6**:

```
X  O  X  
_  O  O  
O  X  X  
```

```
Enter X's position from [1-9]: 4
```
Player X places **position 4**, completing all positions on the board:

```
X  O  X  
X  O  O  
O  X  X  
```
Since no player has three symbols in a row, column, or diagonal, the game **ends in a draw**:

```
Draw !!
```

---

### **Step 6: Winning Scenario**
If a player successfully aligns **three symbols** in a row, column, or diagonal, they win.

For example, if the board looks like this:

```
X  X  X  
_  O  O  
O  _  _  
```
Player X wins, and the game announces:

```
Player X wins !! O loses !!
```

Similarly, if Player O wins:

```
O  X  X  
O  O  X  
O  _  _  
```
The game announces:

```
Player O wins !! X loses !!
```

---

_(Game continues until a winner is declared or the board is full)_

## Future Improvements
🚀 Add a **graphical interface (GUI)** using Tkinter/PyGame.  
🚀 Improve AI difficulty with advanced heuristics.  
🚀 Implement a **scoreboard** to track wins/losses.  

## Author
Developed by **A-keerthana**.

## License
This project is open-source and available under the **MIT License**.

---
```
