

> **Role:** You are an expert game developer specializing in HTML5 Canvas and vanilla JavaScript.
>
> **Task:** Develop a complete, highly refined web-based 2D arcade defense game inspired by the classic "Missile Command." The game should be contained within a single `index.html` file containing HTML, inline CSS, and JavaScript.
>
> **Theme & Context:** > The player controls Israel's defense system (like the Iron Dome/Arrow), intercepting incoming missile barrages originating from Iran. The objective is strictly defensive: protect the city buildings at the bottom of the screen from being destroyed.
>
> **Visual Style (Crucial):**
>
> * **Aesthetic:** 8-bit retro pixel-art arcade look.
> * **Palette:** Deep black sky for contrast. Buildings should be blocky, cyan or gray pixelated silhouettes. Enemy missiles leave bright red pixel trails. Player interceptors leave blue or yellow pixel trails.
> * **Effects:** Explosions should be expanding, blocky pixelated circles that flash white and yellow before fading. If possible, add a subtle CSS CRT scanline overlay to the canvas for a true retro arcade feel.
>
> **Core Game Mechanics:**
>
> 1. **The City:** Render 6 distinct, blocky pixel-art buildings spaced evenly across the bottom of the canvas.
> 2. **Enemy Missiles:** >     \* Spawn randomly at the top of the canvas and travel downwards at varying angles, targeting the buildings.
>    * Start with a manageable speed and spawn rate.
> 3. **Player Interceptors (Defense):**
>    * The player clicks anywhere on the canvas to launch an interceptor.
>    * Interceptors launch from a central base at the bottom of the screen.
>    * They travel at a fast, fixed speed to the exact X/Y coordinates of the click.
>    * Upon reaching the target coordinates, the interceptor detonates, creating an expanding "blast radius" (an expanding circle that lasts for 1-2 seconds).
> 4. **Collision Detection:**
>    * If an enemy missile's coordinates fall within the active blast radius of an interceptor's explosion, the enemy missile is destroyed, adding to the player's score.
>    * If an enemy missile reaches a building's bounding box, both the missile and the building are destroyed. Play a specific, larger, ground-level explosion effect.
>
> **Game Progression & Logic:**
>
> * **Waves:** Group incoming missiles into waves. Each wave increases the speed, spawn rate, and number of enemy missiles.
> * **Ammo/Cooldown:** To prevent click-spamming, give the player a maximum of 3 active interceptors in the air at one time, or implement a rapid reload system (e.g., 20 shots per wave).
> * **Game States:**
>   * *Start Screen:* Large retro pixel font displaying the game title and "Click to Start."
>   * *Active Play:* HUD showing Score, Current Wave, and remaining buildings.
>   * *Game Over:* Triggered when all 6 buildings are destroyed. Display "GAME OVER" in red pixel font, final score, and "Click to Restart."
>
> **Technical Requirements:**
>
> * Use `requestAnimationFrame` for a smooth game loop.
> * Use object-oriented programming (ES6 Classes) for Game Entities (Missile, Interceptor, Explosion, Building, Particle) to keep the code clean and scalable.
> * Handle window resizing gracefully, or lock the canvas to a classic arcade aspect ratio (e.g., 800x600) centered on the screen.
>
> Please output the complete, runnable code within a single HTML code block.

***



