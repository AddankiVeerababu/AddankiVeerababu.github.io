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




