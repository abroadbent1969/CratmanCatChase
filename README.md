Cartman Cat Chase
Overview
Cartman Cat Chase is a browser-based game inspired by classic arcade maze games. You control Cartman, navigating a maze to collect pellets, power-ups, and special prizes while avoiding cats and interacting with a turtle. The game features increasing difficulty, sound effects, and animated overlays for an engaging experience.
Features
Player Control: Use arrow keys to move Cartman through the maze.

Objective: Collect pellets (10 points), power-ups (100 points), prizes (100 points), and special prizes (100 points per cat + 1 extra life).

Enemies: Four cats chase Cartman. When a power-up is active, cats become vulnerable, and colliding with them earns 100 points.

Turtle: A turtle roams the maze. Collecting it grants 100 points.

Lives and Scoring: Start with 3 lives. Lose a life when hitting a cat (unless powered up). Game over when lives reach 0.

Levels: Clear all pellets and power-ups to advance. Each level increases cat speed.

Audio: Sound effects for actions like collecting items, collisions, and level-ups.

Visuals: Animated overlays for points, game over, and level transitions.

Installation
Clone or Download: Obtain the game files (HTML, images, and sounds).

Directory Structure:
Place the HTML file in your project root.

Ensure the images/ folder contains:
eric_cartman.png (player)

cat.png (enemy)

cat-sleep.png (vulnerable enemy)

turtle.png (turtle)

pie.png (power-up)

polly.png (prize)

flower-pot.png (special prize)

points-100.png (points overlay)

poof.png (collision overlay)

GameOver.png (game over screen)

StartGame.png (start screen)

cartman_cop.png (level-up overlay)

Ensure the sounds/ folder contains:
start.wav, pellet.wav, powerup.wav, specialPrize.wav, no_kitty.wav, meow.wav, pie.wav, alright-voice-cartoon.wav, dead.wav, hey.wav, home.wav, balls.wav, respect.wav, hippy.wav, crash.wav

Host or Open:
Use a local server (e.g., python -m http.server or VS Code Live Server) to avoid CORS issues with audio/image loading.

Alternatively, open the HTML file directly in a browser (note: some browsers may block local audio).

How to Play
Start the Game:
Open the HTML file in a browser.

Press any arrow key to start. The start screen displays "Use The Arrow Keys".

Controls:
Arrow Keys: Move Cartman up, down, left, or right.

Gameplay:
Navigate the maze to collect yellow pellets, power-ups (pies), prizes (Polly), and special prizes (flower pots).

Avoid cats unless powered up (after eating a pie), when you can "eat" them for points.

Collect the turtle for bonus points.

Clear all pellets and power-ups to advance to the next level.

Power-Ups and Prizes:
Power-Up (Pie): Makes cats vulnerable for 10 seconds, allowing you to eat them for 100 points each.

Prize (Polly): Appears periodically for 10 seconds, worth 100 points.

Special Prize (Flower Pot): Appears periodically, "eats" all active cats (100 points each) and grants an extra life.

Game Over:
Lose a life when hitting a cat (unless powered up).

The game ends when lives reach 0, displaying a "Game Over" screen.

Level Progression:
Each level increases cat speed, making the game harder.

A "Cartman Cop" overlay appears when starting a new level.

Technical Details
Tech Stack: HTML5, CSS3, JavaScript, Canvas API.

Canvas: Used for rendering the maze, pellets, power-ups, and prizes (608x608 pixels).

Assets:
Images for sprites and overlays.

Audio files for sound effects.

Game Loop: Uses requestAnimationFrame for smooth updates.

Collision Detection: Pixel-based checks for player-enemy and player-item interactions.

Map: 19x19 grid with tiles (32x32 pixels). Values:
0: Path

1: Wall

2: Pellet

3: Power-Up

4: Prize

5: Special Prize

Development Notes
Error Handling: The game logs errors for failed image/audio loads to the console.

Performance: Optimized for smooth rendering with minimal DOM updates.

Extensibility: The map and enemy behaviors can be modified by editing the map array and ghostSpeed settings.

Troubleshooting
No Sound/Images:
Ensure images/ and sounds/ folders are in the correct directory.

Use a local server to avoid CORS restrictions.

Game Not Starting:
Check the console for errors (Ctrl+Shift+J in browsers).

Verify all asset files are present and correctly named.

Performance Issues:
Reduce browser load by closing tabs or using a modern browser (Chrome, Firefox recommended).

Credits
Inspired by: Classic arcade maze games.

Assets: Custom images and sounds (ensure you have rights to use or replace with your own).

License
This project is for personal use and demonstration. Ensure all assets (images, sounds) are licensed appropriately for your use case.
Enjoy playing Cartman Cat Chase! For feedback or issues, check the console logs or modify the code to suit your needs.

