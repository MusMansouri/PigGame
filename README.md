# Pig Game

This project is an interactive dice game called "Pig Game," created as part of a JavaScript training. It is a two-player game where each player rolls a die and accumulates points until reaching a predefined score to win the game. If a player rolls a 1, they lose all points accumulated during their turn, and it's the other player's turn.

## Features

- **Roll Dice**: Players can roll a die and accumulate points.
- **Hold Points**: Players can choose to hold their accumulated points to secure their score.
- **New Game**: Players can start a new game at any time.
- **Active Player Indication**: The active player is highlighted with a style change.

## Technologies Used

- HTML
- CSS
- JavaScript

## Project Structure

The project consists of the following files:

- `index.html`: Contains the structure of the web page.
- `style.css`: Contains the styles for the layout and appearance of the game.
- `script.js`: Contains the JavaScript logic for the game's functionality.

## Usage

1. Clone the repository or download the project files.
2. Open `index.html` in your web browser.
3. Start playing by clicking the "Roll dice" and "Hold" buttons.

## Code Details

### index.html

This file contains the HTML structure of the page, including sections for each player, buttons for game actions, and the element to display the die.

### style.css

This file contains the CSS styles for the game's appearance, including styles for the players, buttons, and the die. It uses the 'Nunito' font from Google Fonts and applies styles for a modern and attractive look.

### script.js

This file contains the JavaScript logic for the game. Here are some key features:

- Selection of necessary HTML elements for the game.
- Initialization of starting conditions.
- Handling of click events on buttons to roll the die, hold points, and start a new game.
- Features for switching the active player and checking the winner.

![Game Flowchart](/img/pig-game-flowchart.png)

```javascript
// Example code from script.js

// Selecting elements
const player0El = document.querySelector('.player--0');
const player1El = document.querySelector('.player--1');

const score0El = document.querySelector('#score--0');
const score1El = document.getElementById('score--1');

const current0El = document.querySelector('#current--0');
const current1El = document.getElementById('current--1');

const diceEl = document.querySelector('.dice');
const btnNew = document.querySelector('.btn--new');
const btnRoll = document.querySelector('.btn--roll');
const btnHold = document.querySelector('.btn--hold');

// Starting conditions
score0El.textContent = 0;
score1El.textContent = 0;
diceEl.classList.add('hidden');

let scores = [0, 0];
let currentScore = 0;
let activePlayer = 0;

// Function to roll the die
btnRoll.addEventListener('click', function () {
  // Game logic
});

// Function to hold points
btnHold.addEventListener('click', function () {
  // Game logic
});

// Function to start a new game
btnNew.addEventListener('click', function () {
  // Game logic
});
```

### Screenshot

![Game Screenshot](img/screenshot.png)
