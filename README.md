# 🧩 8-Puzzle Solver using A* Search Algorithm

A Python implementation of the **A\*** (A-Star) search algorithm to solve the classic **8-Puzzle problem**.  
The program explores possible board configurations and finds the shortest sequence of moves from the initial state to the goal state using a heuristic function.

---

## 🔧 Features

- Solves any valid 8-Puzzle configuration  
- Uses the **A\*** search algorithm for optimal pathfinding  
- Incorporates heuristic-based cost evaluation  
- Visualizes the step-by-step board movement  
- Modular class-based code structure for easy expansion  
- Demonstrates core AI search principles  

---

## 🧱 System Overview

### **Problem Definition**
The **8-Puzzle** is a sliding puzzle consisting of a 3×3 grid with tiles numbered 1–8 and one blank space.  
The objective is to move the tiles until the configuration matches the target state.

### **Algorithm Used**
**A\*** search algorithm:  
- **Cost Function:** `f(n) = g(n) + h(n)`  
  - `g(n)` → cost from the start node  
  - `h(n)` → heuristic estimate of distance to goal  
- **Heuristic:** Tile mismatch count (can be upgraded to Manhattan distance for better accuracy)

---

## 🧠 How It Works

1. **Initial State:** A user-defined 3×3 matrix representing the starting board.  
2. **Target State:** The desired final configuration (usually `[1,2,3],[4,5,6],[7,8,0]`).  
3. **Move Generation:**  
   - The blank (0) can move **up, down, left, or right** if space permits.  
4. **Heuristic Evaluation:**  
   - Counts misplaced tiles relative to the goal state.  
5. **Priority Queue:**  
   - The lowest `f(n)` value (cost + heuristic) is explored next.  
6. **Solution Path:**  
   - When the target configuration is found, all moves are printed in sequence.

---

## 💻 Technologies Used

- **Language:** Python  
- **Libraries:** `heapq` (for priority queue management)  
- **Algorithm:** A\* Search  
- **Paradigm:** Object-Oriented Programming  

---

## 📁 Project Structure

