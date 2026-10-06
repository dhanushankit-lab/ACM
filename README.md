# 2D Pong Game

A single-player 2D Pong game built in a standalone HTML file using pure JavaScript and the HTML5 Canvas API.

## Features
- **Player Paddle:** Smooth movement with `W` / `S` and `Up` / `Down` arrow keys, with strict boundary clamping.
- **Physics & Ball Movement:** Explicit velocity increments per frame with position-corrected wall bouncing.
- **Manual Collision Detection:** Custom circle-to-rectangle (AABB) overlap testing with front-face deflection and sticking/tunneling prevention.
- **Beatable AI Opponent:** Tracks the ball's Y-position with a dead zone to eliminate jitter and a capped max speed lower than the ball's vertical velocity.
- **Scoring & Reset:** Live score tracking on canvas, serve pause/countdown, and serve direction toward the scoring side with randomized angles.
- **Angle-Based Bounce:** Deflection angles up to ±60° depending on paddle contact point, with progressive speed acceleration up to a cap.

## How to Play
Open `index.html` in any modern web browser.
- Move paddle up: `W` or `↑`
- Move paddle down: `S` or `↓`
