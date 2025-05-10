# Alphabet Wood Puzzle Game

A simple and fun web-based alphabet puzzle game designed for toddlers (approx. 3 years old). This game helps children learn the English alphabet (A-Z) by dragging and dropping colorful letter blocks onto their corresponding outlines on a wooden-themed board.

## Features

*   **Interactive Gameplay**: Drag and drop uppercase letters (A-Z) to their matching slots.
*   **Kid-Friendly UI**: Colorful, large letter blocks and a visually appealing wooden board theme, built with HTML, Tailwind CSS, and JavaScript.
*   **Responsive Design**: Works on desktops, tablets, and phones.
*   **Audio Feedback (Setup Required)**:
    *   Letter pronunciations when a letter is clicked or dragged.
    *   Sound effects for correct matches (success chime, wooden block drop).
    *   Sound effect for incorrect matches (gentle "try again" sound).
*   **Completion Animation**: A "Well Done!" message appears when all letters are matched, with an option to "Play Again".

## How to Play

1.  Open the `index.html` file in a web browser, or visit the live demo.
2.  The game board will display outlines for all letters from A to Z.
3.  A tray at the bottom of the screen will contain all 26 letter blocks in a shuffled order.
4.  Click and drag a letter block from the tray.
5.  Drop the letter block onto its matching outline on the board.
    *   **Correct Match**: The letter will lock into place, and a success sound will play.
    *   **Incorrect Match**: The letter will return to its original spot in the tray, and a "try again" sound will play.
6.  Continue until all letters are correctly placed.
7.  A congratulatory message will appear. Click "Play Again?" to restart the game.

## Sound Effect Setup

The game includes a framework for sound effects. To enable them, you need to:

1.  **Provide Sound Files**: Obtain or create sound files (e.g., `.mp3`, `.wav`) for:
    *   A success chime/sound.
    *   A failure/try-again sound.
    *   A wooden block drop sound.
    *   A subtle drag sound (optional).
    *   Pronunciations for each letter of the alphabet (A-Z).
2.  **Update HTML**:
    *   In the `index.html` file, locate the `<audio>` tags near the end of the `<body>`.
    *   For each `<audio>` tag (e.g., `<audio id="audio-success" src="#">`), replace the `src="#"` with the actual URL or relative path to your sound file.
    *   Ensure you add `<audio>` tags for letters B through Z, similar to the example provided for `audio-A`:
        ```html
        <!-- ... other audio tags ... -->
        <audio id="audio-A" src="path/to/your/A_sound.mp3"></audio>
        <audio id="audio-B" src="path/to/your/B_sound.mp3"></audio>
        <!-- ... and so on for C through Z ... -->
        ```

## Live Demo

You can play the game live on GitHub Pages: [https://biswatma.github.io/abcd-game/](https://biswatma.github.io/abcd-game/)

*(Note: Sound effects in the live demo will only work if placeholder `src` attributes have been updated with valid URLs in the deployed code.)*
