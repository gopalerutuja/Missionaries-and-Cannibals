# Missionaries and Cannibals Problem

This project implements the **Missionaries and Cannibals** puzzle using Python.
It’s a classic AI problem that demonstrates **state-space search** and **constraint satisfaction** concepts in an interactive way.

---

## Problem Description

Three missionaries and three cannibals must cross a river using a boat that can carry a maximum of **two people** at a time.
At no point can **cannibals outnumber missionaries** on either bank, or the missionaries will be eaten!

### Goal:

Safely transport all missionaries and cannibals from the **right bank** to the **left bank** without breaking the rule above.

---

## How It Works

* The boat starts on the **right side** with all 3 missionaries and 3 cannibals.

* The player decides how many missionaries and cannibals to move each turn.

* After each move, the program updates the state and displays it in the format:

  ```
  M = (left missionaries) C = (left cannibals) |-----B| M = (right missionaries) C = (right cannibals)
  ```

* The player must ensure the rules are followed:

  * Only 1 or 2 people can travel at once.
  * You can’t move more people than available on a side.
  * Missionaries should **never be outnumbered** by cannibals on either side.

---

## Game Rules

| Rule | Description                                                                     |
| ---- | ------------------------------------------------------------------------------- |
| 1    | Boat can carry **1 or 2 people** maximum.                                       |
| 2    | **Missionaries cannot be outnumbered** by cannibals on any side.                |
| 3    | Enter the number of missionaries and cannibals you want to move.                |
| 4    | If an invalid move is made, the program prints an error message and asks again. |
| 5    | The game ends when you either **win** or **lose**.                              |

---

## 🏁 Win & Lose Conditions

* **You Win:**
  When all 3 missionaries and 3 cannibals reach the **left bank**.

* **You Lose:**
  If, on either side, the number of cannibals exceeds missionaries while missionaries are still present.

---

## 💻 Example Output

```
Right Side
M = 0 C = 0 |-----B| M = 3 C = 3
ENTER THE NUMBER OF MISSIONARIES ON BOAT: 1
ENTER THE NUMBER OF CANNIBALS BOAT: 1
M = 1 C = 1 |B-----| M = 2 C = 2
...
YOU WIN
GAME OVER
```

---

## 🚀 How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/<your-username>/Missionaries-and-Cannibals.git
   cd Missionaries-and-Cannibals
   ```

2. Run the Python file:

   ```bash
   python missionaries_and_cannibals.py
   ```

3. Follow the on-screen prompts to play the game.

## 🧠 Concepts Demonstrated

* State-space representation
* Constraint checking
* Loop control and conditional logic
* Basic human-computer interaction via CLI


