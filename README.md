# 🔠 Building Wordle game

This is a fun, interactive browser-based word game inspired by the popular game **Wordle**. The player must guess a randomly selected 5-letter English word in six tries or less. After each guess, the letters are marked with colors to indicate how close the guess was to the target word.

Built entirely with **HTML, CSS, and JavaScript**, this game demonstrates DOM manipulation, responsive UI design, and asynchronous API usage to validate words via an English dictionary.

---

## 🎯 Game Objective

- Guess the 5-letter word in **six or fewer attempts**.
- Each letter of your guess will provide feedback:
  - 🟩 **Green**: The letter is in the correct spot.
  - 🟨 **Yellow**: The letter is in the word but the wrong spot.
  - ⬛ **Gray**: The letter is not in the word at all.
- After each attempt, the input row locks and the next row is activated.

---

## 🧠 Game Logic

- Words are randomly picked from a pre-defined word list in `script.js`.
- The game dynamically creates 6 rows of 5 input boxes.
- On each keystroke:
  - The character is uppercased and stored.
  - The player can delete characters using **Backspace**.
- When all 5 letters are entered and **Enter** is pressed:
  - The word is validated via the Dictionary API.
  - If valid, the game checks each character against the solution.
  - Visual feedback is applied using CSS classes (`.correct`, `.exists`, `.incorrect`).
- The game ends with a **win screen** or **loss message**.

---

## 🖼️ Visual Layout

- The layout is styled with a vibrant gradient background and a centered wrapper box.
- Mobile responsive: Stacks game board and rules image vertically on small screens.
- Colored boxes provide immediate visual clues.
- `rules.svg` is shown to help users understand the mechanics.

# 🖼️ Interactive Image Processing Gallery – Web Project

This project is a dynamic **image gallery web application** that allows users to perform real-time **image processing tasks** directly in the browser using **HTML, CSS, and JavaScript**. It includes features such as grayscale conversion, brightness control, image duplication, QR code generation, resolution adjustment, and avatar creation.

---

## 🎯 Project Highlights

- 📸 **Image Gallery** with multiple sample images
- 🎨 **On-Click Image Processing**: Apply grayscale, brightness boost, resolution reduction
- 🌀 **Circular Avatar Generation** from any image
- 💡 **Color Filters**: Reddish, Greenish, Blueish using CSS filters
- 📦 **Thumbnail Preview** from dropdown menu
- 📲 **QR Code Generator** for image URLs using `qrious.js`

---

## 🧠 Features Explained

### 🖼️ Image Display & Hover
Each image in the gallery:
- Can be previewed in full size.
- Has individual processing buttons.
- Displays hover effects via CSS.

### 🛠️ Image Processing Options

| Feature | Description |
|--------|-------------|
| **Duplicate** | Clones the selected image and adds it to the gallery. |
| **Grayscale** | Converts the image to black & white using CSS filters. |
| **Brightness** | Increases brightness using pixel manipulation on `<canvas>`. |
| **Avatar** | Creates a circular version of the image (rounded with `border-radius: 50%`). |
| **Resolution Reduction** | Lowers image resolution using `<canvas>` rescaling. |

### 🎛️ Filter Effects
You can apply hue-based filters to all images:
- 🔴 Reddish
- 🟢 Greenish
- 🔵 Blueish

### 🧩 Thumbnails
Dropdown lets you:
- Choose an image by name
- Preview it as a 100×100 thumbnail

### 🔳 QR Code Generator
- Converts the selected image filename into a **scannable QR code**.
- Useful for linking to images or using them in other apps.

# ❌⭕ Tic Tac Toe – JavaScript Game Project

Welcome to **Tic Tac Toe**, a fully interactive and web-based game where you can challenge a friend or take on an unbeatable computer opponent! Designed using **HTML5 Canvas**, styled with **CSS3**, and powered by **pure JavaScript**, this game combines simplicity, fun, and smart AI for an engaging experience.

---

## 📖 About the Project

This project simulates the classic **Tic Tac Toe (also known as Noughts and Crosses)** game. It features both **single-player mode (vs. AI)** and **double-player mode (local multiplayer)**, allowing users to enjoy the game with a friend or challenge themselves against a computer opponent that uses the **Minimax algorithm**.

This game was built as a personal learning project and serves as a strong example of DOM manipulation, HTML5 canvas drawing, game loops, condition checking, and AI integration.

---

## 🎮 Gameplay Overview

- The game is played on a **3x3 grid**.
- Player 1 and Player 2 (or the Computer) take turns placing **X or O**.
- The first player to get three of their marks in a **horizontal, vertical, or diagonal** row wins.
- If all 9 squares are filled and no player has won, the game ends in a **tie**.

---

## ✨ Features

| Feature | Description |
|--------|-------------|
| ✅ **Single Player Mode** | Play against a smart computer opponent (Minimax AI). |
| ✅ **Two Player Mode** | Play locally against a friend on the same device. |
| ❌⭕ **Symbol Selection** | Choose whether to play as X or O. |
| 🎨 **Canvas Rendering** | Game board and moves rendered on HTML5 `<canvas>`. |
| 🎉 **Game Over Screen** | Animated result screen shows winner or tie and offers "New Game" button. |
| 🧠 **Unbeatable AI** | Computer uses Minimax algorithm for perfect play. |
| 🖼️ **Image Assets** | Custom icons (e.g., `X.png`, `O.png`) for gameplay visuals. |
| 💻 **Responsive Layout** | Easily playable on laptops and desktops. |
| 🪄 **Smooth UI Transitions** | Hover effects, active states, and feedback visuals. |

---

## 🧠 AI: How the Computer Thinks

In **Single Player Mode**, the computer opponent is powered by the **Minimax Algorithm**:
- Evaluates every possible move and counter-move.
- Calculates a numerical score for win/loss/tie outcomes.
- Picks the best move based on scoring.
- Guarantees **perfect play** — you can never beat it, only tie or lose if you make a mistake.

---

## 🛠 Tech Stack

| Technology | Role |
|------------|------|
| **HTML5**  | Base structure and game canvas |
| **CSS3**   | Styling, layout, buttons, hover animations |
| **JavaScript** | Game logic, AI, state management, canvas drawing |
| **Canvas API** | Grid rendering and image placement |
| **Minimax Algorithm** | AI strategy for unbeatable moves |






