# Pond Snake

A compact browser Snake game built as a single HTML file. Pond Snake combines classic grid movement with escalating difficulty, collectible bonuses, cosmetic unlocks, and a custom gradient skin editor.

## Game Review

Pond Snake is easy to start and gradually becomes more demanding. The three difficulty modes make it approachable for new players while still giving experienced players a faster, more dangerous challenge. The progression loop gives each run a clear goal: collect points, reach higher levels, unlock skins, and improve your best score.

The shop adds a useful long-term layer without changing the core Snake rules. Players can unlock Black, Grey, Green Gradient, Blue Gradient, and Custom Gradient skins. The Custom Gradient skin includes a 15-level editor so players can choose how many colors appear across the snake.

## Features

- Classic Snake movement on a 20 x 20 canvas grid
- Easy, Normal, and Hard difficulty modes
- Wraparound walls in Easy mode
- Deadly walls and stone obstacles in Normal and Hard modes
- Red berries, Gold bonus berries, and Blue slow-time pickups
- Combo multiplier for quick pickups
- Level progression every 100 score points
- Maximum level: 100
- Faster movement and additional obstacles at higher levels
- Persistent best scores and unlocked skins using `localStorage`
- Shop with point-based cosmetic unlocks
- Custom gradient editor with 15 levels
- Keyboard, touch swipe, and on-screen mobile controls
- Space to pause and Escape to exit the current game

## Skin Unlocks

| Skin | Cost |
| --- | ---: |
| Black | 23 points |
| Grey | 50 points |
| Green Gradient | 60 points |
| Blue Gradient | 70 points |
| Custom Gradient | 1000 points |

## Difficulty Modes

| Mode | Starting Speed | Walls | Stones |
| --- | ---: | --- | ---: |
| Very Easy | Relaxed | Wrap around | None |
| Normal | Faster | Deadly | Yes |
| Spedrun.exe | Fastest | Deadly | More stones |

Every 100 score points increases the level. Progression stops at level 100. As the level rises, the snake moves faster; Normal and Hard modes also add more stone obstacles.

## Controls

- Arrow keys or `WASD`: steer
- `Space`: pause or resume
- `Escape`: exit the current game
- Touch swipe: steer on phones and tablets
- On-screen arrow buttons: mobile fallback controls

## Run Locally

No build step or installation is required.

1. Download or clone this repository.
2. Open `snake.html` in a modern web browser.
3. Press **Play the game**.

The game is designed to work as a standalone static page and can be hosted with GitHub Pages.

## Project Structure

```text
snake.html   The complete game: HTML, CSS, and JavaScript
README.md    Public project review and documentation
```

## Data and Privacy

The game stores best scores and progression locally in the browser. It uses these local storage keys:

- `pondsnake`: best scores by difficulty
- `pondsnake_profile`: points, unlocked skins, equipped skin, and custom gradient level

No account or server is required.

## Technology

- HTML5
- CSS3
- JavaScript
- Canvas 2D API
- Browser `localStorage`

## Public Release Review

Pond Snake is a good fit for a small public GitHub project because it is self-contained, immediately playable, and easy to inspect. The single-file structure keeps hosting simple and makes the game accessible to beginners learning browser game development.

The main future improvement would be separating the HTML, CSS, and JavaScript once the project grows. A separate test layer, sound settings, a reset-progress button, and optional online leaderboards could also improve the public release without changing the simple core experience.

## License

Add the license you want to use before publishing, such as MIT, if you want other people to reuse and modify the project.
