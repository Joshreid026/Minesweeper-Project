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
* UI built with **JFrame**, **JPanel**, and **GridLayout**

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

## 💡 Future Features

Here are some improvements planned or worth considering:

* **Difficulty Levels**
  Add Beginner / Intermediate / Expert settings with different board sizes and mine counts.

* **Timer & Best Times**
  Include a game timer and save fastest records locally.

* **Custom Board Sizes**
  Let users choose their own row/column count and number of mines.

* **Improved UI/UX**
  Better tile graphics, animations, hover effects, or a cleaner theme.

* **Restart Button**
  Easily restart without relaunching the program.

* **Sound Effects**
  Add click, explosion, and win sounds.

* **Safe First Click**
  Guarantee the first click is never a mine.

* **Chord Clicking (Advanced)**
  Allow double-clicking a numbered tile to reveal its neighbors when flags match the number—just like classic Minesweeper.

* **Mobile/Touch Version**
  Rebuild with JavaFX or another framework for touch-screen compatibility.

---

## 🔧 Ways I could Develop This Project Further

Here are some ways I could expand the project:

### 1. **Refactor the Code Structure**

* Move the logic into separate classes (`Board`, `Tile`, `GameController`)
* Improve readability and scalability
* Add unit tests for game logic

### 2. **Add a Menu System**

* Main menu
* Difficulty settings
* Help / About
* Restart game option

### 3. **Add Animations or Themes**

* Light/Dark mode
* Custom tile art packs
* Animations when tiles reveal

### 4. **Support for Multiple Game Modes**

* Hexagonal Minesweeper
* Triangular grid
* “No Guess” mode (algorithm ensures no forced guesses)

### 5. **Persistent Save Files**

* Store high scores
* Save current game state
* Load last played board

### 6. **AI Solver or Hint System**

* Add a solver that explains reasoning
* Provide player hints based on safe moves

### 7. **Online Features (Advanced)**

* Share scores on a leaderboard
* Timed challenge mode
* Multiplayer: race to clear the board first

---

## 📁 Project Structure

```
Minesweeper.java   // Main game class + UI setup + logic
```
