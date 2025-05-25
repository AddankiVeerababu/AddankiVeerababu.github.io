# 🔠 Wordle-Inspired Word Guessing Game

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



