# Game of Life (Python + NumPy + Pygame)

This project is an implementation of **Conway's Game of Life** using **Python**, **NumPy**, and **Pygame**.  
I built it as a **learning project** to practice working with **NumPy arrays** and basic **Pygame visualization**.

---

## 🎮 Features
- Classic **Game of Life** simulation.
- Interactive grid:
  - **Draw live cells** with mouse clicks.
  - **Start / Pause** simulation with `SPACE`.
  - **Reset** the board with `R`.
- Uses **NumPy arrays** for fast and efficient grid updates.
- Simple and clean **Pygame-based UI**.

---

## 🕹️ Controls
| Key / Action     | Description |
|------------------|-------------|
| **Left Mouse**   | Add a live cell |
| **SPACE**        | Start / Pause the simulation |
| **ESC**            | Reset the grid (clear all cells) |
| **Close Window** | Quit the program |

---

## 🖼️ How It Works
- The game grid is stored as a **2D NumPy array**:
  - `0` → Dead cell  
  - `1` → Alive cell
- For every cell, neighbors are counted using **NumPy slicing**.
- Game rules:
  - Live cell with < 2 neighbors → **dies** (underpopulation)  
  - Live cell with > 3 neighbors → **dies** (overpopulation)  
  - Dead cell with exactly 3 neighbors → **becomes alive** (reproduction)  

---

## 📦 Requirements
Install the dependencies:
```bash
pip install numpy pygame
````
### ▶️ Run the Project
````bash
python game_of_life.py
````
## 🧑‍💻 What I Learned
- How to represent grids with **NumPy arrays**.
- How to use **array slicing** to count neighbors efficiently.
- Basics of **Pygame** for drawing and event handling.
- Implementing a **cellular automaton** from scratch.

---

## 🚀 Future Improvements
- Add **random initial patterns**.
- Allow changing **grid size dynamically**.
- Add **simulation speed controls**.
- Include famous patterns like **gliders** and **oscillators**.

---

## 📚 About Conway’s Game of Life
The Game of Life is a **cellular automaton** devised by mathematician **John Conway**.  
It’s a **zero-player game**: once started, it evolves automatically from the initial state, following simple rules.  
Despite its simplicity, it can generate very **complex and beautiful patterns**.

### I used Cursor for everything in this repo.
