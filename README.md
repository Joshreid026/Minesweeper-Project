# Minesweeper-Project

A simple, classic **Minesweeper** game implemented in Java using **Swing**.
The project features an 8×8 grid, left/right mouse controls, automatic empty-tile clearing, mine generation, and win/loss detection.

---

## 🎮 Features

* **8×8 game board** with 10 randomly placed mines
* **Left-click** to reveal a tile
* **Right-click** to place or remove a flag
* **Recursive clearing** of empty spaces
* **Win detection** when all safe tiles are revealed
* **Game over** display when hitting a mine
* Basic UI built with **JFrame**, **JPanel**, and **GridLayout**

---

## 🚀 Getting Started

### Prerequisites

* **Java 8+**
* A Java-capable IDE (VS Code, IntelliJ, Eclipse) or command-line tools

### Compile & Run

```bash
javac Minesweeper.java
java Minesweeper
```

Or open the project in your IDE and run the `Minesweeper` class.

---

## 🧠 How It Works

* The board is represented by a 2D array of custom `MineTile` buttons.
* Mines are randomly placed and stored in an `ArrayList` for quick lookup.
* Clicking tiles:

  * If the tile has a mine → reveal all mines → **Game Over**.
  * If safe → count nearby mines and show the number.
  * If no nearby mines → recursively reveal surrounding tiles.
* Game finishes when all non-mine tiles are clicked.

---

## 📁 Project Structure

```
Minesweeper.java   // Main game class + UI setup + logic
```

---

## 📝 Notes

* Uses basic emojis (💣 🚩) for mines and flags.
* Uses Swing for layout and user interaction.
* The code is self-contained—no external libraries required.

---

## 📜 License

This project is free to modify, learn from, or extend.
