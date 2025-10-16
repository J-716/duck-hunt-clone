# Duck Hunt Clone

A modern recreation of the classic Duck Hunt game built with TypeScript and Kaplay.

## Features

- **Classic Gameplay**: Hunt ducks across multiple rounds with limited bullets
- **Animated Characters**: Detailed sprite animations for the dog and duck
- **Sound Effects**: Immersive audio including quacking, flapping, gunshots, and more
- **Score System**: Track your performance with persistent high score
- **Round Progression**: Increasing difficulty with faster duck movement
- **Retro Aesthetics**: Nintendo NES-inspired pixel art and fonts

## Game Mechanics

- **3 bullets per duck** - Use them wisely!
- **10 ducks per round** - Hunt them all to advance
- **Progressive difficulty** - Ducks get faster each round
- **Smart AI** - Dog reacts to your performance with different animations
- **Score tracking** - Earn points for each successful hit

## Controls

- **Click** - Shoot at ducks
- **P** - Pause/Resume game

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd duck-hunt-clone
```

2. Install dependencies:
```bash
pnpm install
```

3. Start the development server:
```bash
pnpm dev
```

4. Open your browser and navigate to the local development URL (typically `http://localhost:5173`)

## Building for Production

```bash
pnpm build
```

The built files will be in the `dist` directory.

## Project Structure

```
duck-hunt-clone/
├── src/
│   ├── entities/          # Game entities (duck, dog)
│   ├── constants.ts       # Game constants and colors
│   ├── gameManager.ts     # Game state management
│   ├── kaplay.Ctx.ts     # Kaplay context setup
│   ├── main.ts           # Main game entry point
│   └── utils.ts          # Utility functions
├── public/
│   ├── graphics/         # Sprite assets
│   ├── sounds/          # Audio files
│   └── fonts/           # Custom fonts
└── index.html           # HTML entry point
```

## Technologies Used

- **Kaplay** - 2D game framework
- **TypeScript** - Type-safe JavaScript
- **Vite** - Build tool and dev server
- **PNPM** - Package manager

## Assets

- **Graphics**: Custom pixel art sprites
- **Audio**: Retro-style sound effects
- **Fonts**: Nintendo NES font for authentic feel

## Development

The game uses a state machine pattern for managing game flow and entity behavior. Key systems include:

- **Game Manager**: Handles rounds, scoring, and state transitions
- **Duck Entity**: Manages flight patterns, collision detection, and animations
- **Dog Entity**: Controls search behavior, reactions, and animations

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Credits

- **Developer**: JDesigns
- **Framework**: [Kaplay](https://github.com/kaplayjs/kaplay)
- **Font**: Nintendo NES Font
- **Inspiration**: Original Duck Hunt (Nintendo, 1984)
