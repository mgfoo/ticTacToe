## 🎮 Adversarial Search AI: Tic-Tac-Toe
**Course:** CMPT 310 – Artificial Intelligence (Winter 2024)  
**Languages & Tools:** Python · Minimax · Alpha-Beta Pruning · Expectimax · Heuristic Design

As part of an AI coursework assignment, I developed an adversarial AI player for an extended Tic-Tac-Toe game (board size > 6) using advanced search strategies. The project involved implementing various decision-making algorithms from scratch and designing an intelligent evaluation function to allow the AI to play competitively and under time constraints.

### 🔍 What I Built
- Implemented multiple AI agents to support adversarial play:
  - ✅ **Minimax with Depth Cutoff**
  - ✅ **Alpha-Beta Pruning with Depth Cutoff**
  - ✅ **Expectimax with Probabilistic Nodes and Cutoff**
- Designed a custom **evaluation function** to score board states based on:
  - Alignment patterns
  - Blocking opportunities
  - Win potential for each player
- Tuned performance to ensure each move completes in **under 5 seconds**; optimized search depth to maximize strategic foresight within time constraints.
- Developed basic and advanced **probability models** for Expectimax, assigning lower weights to risky moves (e.g., moves enabling opponent wins).
- Ensured all algorithms supported both **X and O** players for full AI vs. AI simulation.

---

### 📁 File Breakdown

| **File**                  | **Purpose**                                                                                         |
|---------------------------|-----------------------------------------------------------------------------------------------------|
| `minmax.py`               | Implemented Minimax algorithm with support for depth-based cutoff and static evaluation.           |
| `alphabeta.py`            | Built Alpha-Beta Pruning version of Minimax, reducing unnecessary tree exploration for performance. |
| `expectimax.py`           | Implemented Expectimax algorithm with probabilistic decision nodes for modeling uncertainty.        |
| `evaluation.py`           | Wrote a smart evaluation function to estimate game state utility; reused across all cutoff-based agents. |
| `game.py`                 | Core game logic and board management; called appropriate agents for move decisions.                 |
| `main.py`                 | Driver script for launching the game, selecting player types (human/AI), and testing algorithms.     |

---

> 📈 **Result:** Achieved smooth, timed AI gameplay on large boards with intelligent, defensive, and probabilistic strategies using custom heuristic design and search algorithms.

---