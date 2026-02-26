# Tic-Tac-Toe
A collection of my coding projects and learning journey,


Gemini said
This project is a classic Tic-Tac-Toe web application built using the fundamental "holy trinity" of web development: HTML5, CSS3, and Vanilla JavaScript. It provides a clean, interactive user interface where two players can compete locally on the same screen.

## Project Overview
The application features a standard 3×3 grid where players take turns marking spaces with "O" and "X". The game logic automatically detects winning patterns and handles game resets.

### Key Features
* Interactive Gameplay: Users can click on any empty grid box to place their mark.
* Win Detection: The script evaluates the grid after every move against eight predefined winning combinations (horizontal, vertical, and diagonal).
* Visual Feedback: When a player wins, a congratulatory message appears, and the game board is temporarily locked to prevent further moves.
* Game Management: * Reset Button: Allows players to clear the current board and start over.
* New Game Button: Appeared specifically after a win to restart the match.
* Responsive Design: Uses vmin units in CSS to ensure the game board scales appropriately across different screen sizes

## Technical Breakdown
* Component,Responsibility
* HTML (index.html),"Defines the structure, including the game title, the 9-button grid, and the message container for winners."
* CSS (style.css),"Handles the visual styling, using Flexbox for centering, a dark-themed color palette (black and greenyellow), and a .hide class to toggle UI elements."
* JavaScript (app.js),"Manages the state (turn tracking), event listeners for clicks, and the logic to check if a pattern like [0, 1, 2] or [0, 4, 8] has been met."

## How It Works (Logic)
* Turn Tracking: A boolean variable turno tracks whether it is player "O"'s turn (true) or player "X"'s turn (false).
* Pattern Matching: The checkWinner function iterates through an array of arrays containing index positions. If the inner text of three boxes at those positions matches and is not empty, a winner is declared.
* State Management: The disableboxes and enableboxes functions control the interactivity of the buttons to ensure the game flow is followed correctly.
