Le Mot Caché: A Word Search Game
Description
Le Mot Caché (The Hidden Word) is an interactive, browser-based word search game with an educational twist. The game challenges players to find the names of all 26 Premier Cru vineyards from the Gevrey-Chambertin appellation in Burgundy, France.

When a player successfully finds a vineyard's name in the grid, a modal window appears, providing interesting facts about that specific climat, including its size, major producers, and the origin of its name.

The game is built with vanilla JavaScript, styled with Tailwind CSS, and designed to be fully responsive, offering a seamless experience on both desktop and mobile devices.

Features
Dynamic Grid Generation: The word search grid and word placement are dynamically generated on each page load, ensuring a new puzzle every time.

Multiple Selection Methods: Players can select words using two intuitive methods:

Click-and-Drag: Click on the first letter of a word and drag the cursor to the last letter.

Click-Click: Click on the first letter and then click on the last letter.

Advanced Touch Controls: The game is optimized for touch devices with robust gesture handling:

Single-Finger Drag: For word selection.

Two-Finger Pan: Allows users to easily move around the grid on smaller screens without accidentally selecting a word.

Click-Pan-Click: Users can start a selection, pan the grid to find the end of the word, and complete the selection.

Educational Content: After finding each word, a modal provides detailed information about the vineyard, enriching the player's knowledge of Burgundian wine terroir.

Responsive Design: The interface is designed to adapt to various screen sizes, from mobile phones to large desktop monitors.

User-Friendly Interface: The game includes a clear list of words to find, a "New Game" button, and congratulatory messages upon completion.

How to Play
Start the Game: Open the index.html file in any modern web browser. A "How to Play" modal will greet you.

Find the Words: The list on the right side of the screen shows all the vineyard names hidden in the grid. Words can be oriented horizontally, vertically, or diagonally, in any direction (forwards or backwards).

Select a Word:

Method 1 (Drag): Click and hold the first letter, then drag your mouse or finger to the last letter and release.

Method 2 (Click): Click the first letter, then click the last letter.

Learn and Continue: When you find a word correctly, its name will be struck through in the list, and a pop-up will appear with more information about it. Close the pop-up to continue playing.

Win the Game: Find all the words in the list to complete the puzzle. A "Félicitations!" (Congratulations!) message will appear.

Play Again: Click the "New Game" or "Play Again" button to generate a new grid and start over.

Technical Stack
HTML5: For the basic structure of the game.

CSS3 & Tailwind CSS: For modern, responsive styling and layout.

JavaScript (ES6+): For all game logic, including grid generation, user interaction, and DOM manipulation.

File Structure
The entire game is self-contained within a single index.html file. This includes:

The HTML structure.

CSS styles within the <style> tags.

All JavaScript logic within the <script> tags.

This single-file architecture makes the game easy to share and deploy.

Key JavaScript Functions
initializeGame(): Resets and sets up a new game board.

placeWordsInGrid(): The core algorithm that intelligently places words onto the grid, allowing for overlaps.

renderGrid() & renderWordList(): Functions responsible for displaying the game state in the DOM.

handleTouchStart(), handleTouchMove(), handleTouchEnd(): A suite of robust event handlers that differentiate between single-touch selections and two-finger panning gestures.

checkSelection(): Validates if a player's selection matches a word from the list.

showDefinitionModal(): Displays the informational pop-up when a word is found.
