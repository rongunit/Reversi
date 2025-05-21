# 🎲 Reversi (Othello) – Java Console Game

A fully playable, text-based version of **Reversi (Othello)** built in Java with clean modular design and Maven support. Play against a simple AI, manage settings, and track your score on a persistent leaderboard — all from the terminal!

---

## 🚀 Features

- 🎮 Player vs Computer and Player vs Player modes
- ♟️ Smart game engine with valid move detection
- 🧠 Basic AI opponent logic with moves evaluation
- 🛠️ Menu system with settings and options
- 🏆 Leaderboard with persistent score tracking
- 🧱 Built and managed using **Maven**

---

## 🎯 Game Rules

**Reversi (also known as Othello)** is a two-player strategy board game played on an 8×8 grid. Players take turns placing discs to trap and flip their opponent's pieces.

### 🔹 Objective
- End the game with **more pieces of your color** on the board than your opponent.

### 🔹 Core Rules
- Black always goes first.
- A move is valid only if it **captures at least one opponent piece** by bracketing it between the piece placed and another of your own, in any direction (horizontal, vertical, or diagonal).
- All bracketed opponent pieces are **flipped** to your color after the move.
- If a player has no legal moves, they must pass their turn.
- The game ends when **neither player can move** (typically when the board is full).

### 🖥️ Symbols
- `b` – **Black disc**
- `w` – **White disc**
- `-` – **Empty cell**
- `o` – **Legal move indicator** (shows where a player can place a disc each turn)

---

## 📂 Project Structure

<pre>reversi/
├── pom.xml
├── README.md
├── src/
│ ├── main/
│ │ └── java/
│ │ └── com/
│ │ └── rongunit/
│ │ └── reversi/
│ │ | ├── Main.java
│ │ | ├── App.java
│ │ | ├── Game.java
│ │ | └── MenuHandler.java
</pre>

---

## 🧩 Class Responsibilities
- MenuHandler - manages logic of Main, Settings and Leaderboard Menus
- Game - manages the game logic (including Bot-opponent logic), progress, score and ending.
- App - connects MenuHandler and Game (handler) into a single app
- Main - for ease of use/boot up
