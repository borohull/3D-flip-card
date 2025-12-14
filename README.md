# Retro 3D Game Flip Cards
A pure CSS project featuring 3D rotating product cards designed with a 90s arcade aesthetic. The cards mimic physical game boxes that flip over to reveal statistics, using pixel-art fonts, neon colors, and CRT scanline effects.

## Features
* **Pure CSS Interactivity:** Uses the "Checkbox Hack" to handle click states without JavaScript.
* **3D Transformations:** Smooth CSS animations with perspective depth.
* **Retro Aesthetic:** Uses the "Press Start 2P" font, sharp corners, and high-contrast neon colors.
* **Responsive Layout:** Built with Flexbox and CSS Grid.

## How it Works (The Checkbox Hack)
This project does not use JavaScript for the click interaction. Instead, it links a label to a hidden checkbox.

1. The **Insert Coin** button is a HTML `<label>`.
2. This label is linked to a hidden `<input type="checkbox">`.
3. When the label is clicked, the checkbox state changes to `checked`.
4. CSS detects this change and rotates the card using the sibling selector `~`.
