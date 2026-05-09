Final Game Specification: Project Mosaic – Avengers Assemble
Role: You are a Senior Game Developer specializing in HTML5 Canvas, JavaScript (ES6+), and CSS3. Your goal is to build a high-performance, polished web game based on the following specs.
1. Visual & Theme Identity

* Theme: "Modern Spacy Neon" meets "Stark Industries Tech."
* Background: Solid black (`#000000`).
* Bubbles: 3 colors: Neon Red, Neon Blue, Neon Green. All bubbles must have a `shadowBlur` glow effect to look like neon lights.
* Start Page: Deep space gradient with animated stars. Features a "Start" button with neon glassmorphism and a "Mission Briefing" feel.
* UI Components:
   * Pause/Close: Top-right corner. Pause uses a "Time Stone" (Green) glow; Close is "Red" and resets the session.
   * Jarvis Commentary Box: A sleek text area that updates with Gen Z / Avenger-themed banter based on gameplay.
2. Core Game Mechanics

* Grid System: 8 Columns x 15 Rows.
* The Shooter: Centered at the bottom. Displays the current random bubble color and a trajectory guide.
* Objective (The "Hologram"):
   * Display a small 2D target figure (the "Mosaic") in a side-panel on the right.
   * The user must replicate this pattern anywhere on the main 8x15 grid.
   * Once a cluster of bubbles matches the target pattern (color and shape), those bubbles vanish.
* Gravity Logic: If a figure is cleared and other bubbles are left floating in the middle of the screen, they must fall down the columns until they hit another bubble or the bottom row (Row 15).
* Game Over: If any bubble occupies Row 15 without completing a figure, the game ends.
3. Scaling Difficulty

* Level 1 (0-100 pts): Small 2x2 or 3x1 shapes, single colors.
* Level 2 (101-500 pts): 3x3 shapes with two colors.
* Level 3 (500+ pts): 4x4+ complex shapes using all three colors.
4. Scoring & The "Jarvis" Social System

* Scoring: +10 points per completed figure.
* Milestones & User Titles:
   * 0-490 pts: Winter Soldier Fanboy ("Vibe check passed.")
   * 500-990 pts: Low-Key Loki ("The glorious purpose is giving... everything.")
   * 1000-1490 pts: Vibe-Ranium Soldier ("That's America's Aim right there.")
   * 1500+ pts: The Main Character ("I love you 3000, bestie. Pure GOAT energy.")
* Banter & Logic:
   * Good Shot: "No cap, your aim is fire," "Stark would be jealous."
   * Miss/Mistake: "That's not very 'Strongest Avenger' of you," "Is this your first time in the Multiverse?"
   * Losing Comment: "L + Ratio + You should have gone for the head," "You're embarrassing us in front of the Wizards," "Dread it, run from it, the bottom of the screen arrives all the same."
5. Technical Requirements

* Logic: Implement a 2D array to track the grid. Use a pattern-matching algorithm to scan for the "Hologram" shape within the main array.
* Physics: Use `requestAnimationFrame` for smooth bubble travel. Ensure falling bubbles stop correctly upon collision.
* Clean Code: Modular functions for `checkMatch()`, `applyGravity()`, and `generateNewMission()`.
Instruction to AI: "Please generate the HTML, CSS, and JavaScript files to make this game fully playable in a single browser window."
