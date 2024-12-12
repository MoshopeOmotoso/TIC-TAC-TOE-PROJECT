
# Tic-Tac-Toe Project

This project implements a Tic-Tac-Toe game using principles of discrete structures. The game logic uses propositional logic and rules of inference to determine winning, losing, and drawing conditions. Tic-Tac-Toe is a two-player game played on a 3x3 grid. Players take turns marking a square with either `X` or `O`. Each cell can hold one of the following:
- `X` for Player 1's moves
- `O` for Player 2's moves

The goal is to align three marks (in a row, column, or diagonal) while blocking the opponent from doing so.

---

## **Propositional Logic**

### **Definitions**
- **A:** Player 1 makes a move
- **B:** Player 2 makes a move
- **A1:** Player 1 makes a winning move
- **B1:** Player 2 makes a winning move
- **O:** Opponent blocks
- **D:** Draw
- **P1:** Player 1 wins
- **P2:** Player 2 wins

---

## **Winning Condition**
- **Proposition:** If Player 1 (A) plays and all three moves align diagonally, in a row, or in a column without the opponent blocking, then Player 1 wins.
  
  - **Formal Notation:**
    ```
    A ∧ A1 ∧ ¬O → P1
    ```
  - **Using Modus Ponens:**
    1. **Premise 1:** A ∧ A1 ∧ XO (Player 1 plays, makes a winning move, and the move is not blocked).
    2. **Premise 2:** If A ∧ A1 ∧ XO, then P1 (If Player 1 meets the conditions, they win).
    3. **Conclusion:** Therefore, P1 (Player 1 wins). The conclusion follows directly from the premises using Modus Ponens that states that if P, then Q.
P is true.
Therefore, Q is true.


---

## **Losing Condition**
- **Proposition:** If Player 2 (B) plays and all three moves align diagonally, in a row, or in a column without the opponent blocking, then Player 2 wins.
  
  - **Formal Notation:**
    ```
    B ∧ B1 ∧ ¬O → P2
    ```
  - **Using Modus Ponens:**
    1. **Premise 1:** B ∧ B1 ∧ XO (Player 2 plays, makes a winning move, and the move is not blocked).
    2. **Premise 2:** If B ∧ B1 ∧ XO, then P2 (If Player 2 meets the conditions, they win).
    3. **Conclusion:** Therefore, P2 (Player 2 wins). The conclusion follows directly from the premises using Modus Ponens that states that if P, then Q.
P is true.
Therefore, Q is true.


---

## **Draw Condition**
- **Proposition:** If at the end of the game, neither Player 1 nor Player 2 aligns three marks, then the game results in a draw.
  
  - **Formal Notation:**
    ```
    ¬P1 ∧ ¬P2 → D
    ```
  - **Using Modus Ponens:**
    1. **Premise 1:** XP1 ∧ XP2 (Neither Player 1 nor Player 2 wins).
    2. **Premise 2:** If XP1 ∧ XP2, then D (If neither player wins, the game is a draw).
    3. **Conclusion:** Therefore, D (The game results in a draw). The conclusion follows directly from the premises using Modus Ponens that states that if P, then Q.
P is true.
Therefore, Q is true.













