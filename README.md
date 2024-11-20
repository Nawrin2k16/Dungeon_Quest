# Dungeon-Quest: A Turn-Based Grid Adventure

## Overview
**Dungeon Quest Game** is an interactive grid-based survival game that blends strategy, adventure, and AI-driven challenges. The player navigates a dynamic dungeon to reach a treasure while avoiding a pursuing monster. Each level increases in complexity, with grid size doubling and gameplay becoming progressively more challenging. 

## Features
1. **Grid-Based Gameplay:**
   - The dungeon is represented as a grid, with cells containing obstacles, the player, the monster, or the treasure.
   - Players move up (`u`), down (`d`), left (`l`), or right (`r`) to navigate the dungeon.

2. **Dynamic Environment:**
   - Obstacles randomly shift periodically, altering the dungeon layout and requiring players to adapt their strategy.
   - Treasures periodically disappear and reappear in random locations, adding a time-pressure element.

3. **Levels & Progression:**
   - Players advance through levels by reaching the treasure.
   - Grid size doubles with each level, increasing the complexity of navigation and survival.

4. **Challenging Monster AI:**
   - The monster uses different pathfinding algorithms (BFS, A*, or reinforcement learning) to track the player or treasure.
   - The AI adapts as levels progress, becoming smarter and harder to evade.

5. **Game Over Conditions:**
   - The player is caught by the monster or fails to reach the treasure in time.
   - The monster reaches the treasure before the player.

6. **Treasure Mechanics:**
   - Treasure disappears after a certain number of moves, leaving the player to survive until it reappears.
   - When reappearing, the treasure spawns in a new, random, empty cell.

## Technical Highlights
- **Algorithms:** Implements BFS, A*, and reinforcement learning for the monster's movement.
- **Randomized Obstacles:** Ensures every game session feels unique by adding randomized walls and dynamic dungeon shifts.
- **Scalable Levels:** Provides increasing difficulty by doubling grid size and employing smarter AI logic.

## How to Play
1. Enter the dungeon size and start navigating using keyboard inputs (`u`, `d`, `l`, `r`).
2. Avoid the monster and obstacles while aiming to reach the treasure.
3. Survive through shifting obstacles and disappearing treasures to progress to higher levels.

## Requirements
- Python 3.x
- NumPy (for grid representation and calculations)

## How to Run
1. Clone the repository.
2. Install dependencies:
   ```
   pip install numpy
   ```
3. Run the game:
   ```
   python dungeon_escape.py
   ```

## Future Improvements
- Add graphical interface using libraries like `pygame`.
- Introduce multiple difficulty modes.
- Add new AI behaviors and power-ups for the player.
- Include a multiplayer mode for cooperative gameplay.

Enjoy the thrilling challenge of **Dungeon Escape Game**, where wit and strategy determine survival!
