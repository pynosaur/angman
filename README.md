# angman

Terminal Pac-Man with authentic arcade mechanics, rendered entirely in curses.

Based on the original PAC-MAN (1980) by Toru Iwatani, published by Namco.
Game mechanics derived from "The Pac-Man Dossier" by Jamey Pittman.

## Install

```
pget install angman
```

## Usage

```
angman          # start the game
angman --help   # show help
```

## Controls

| Key | Action |
|-----|--------|
| Arrow keys / WASD | Move |
| Space | Pause |
| R | Restart |
| Q / Esc | Quit |

## Ghosts

| Char | Name | Behavior |
|------|------|----------|
| B | Blinky (red) | Chases you directly |
| P | Pinky (pink) | Targets 4 tiles ahead |
| I | Inky (cyan) | Flanks using Blinky |
| K | Clyde (orange) | Chases far, retreats close |

## Fruits

Spawn at random tiles after eating dots. Expire if not collected.

| Char | Points | Time |
|------|--------|------|
| % | 100 | 50s |
| $ | 200 | 40s |
| @ | 300 | 30s |
| & | 1000 | 20s |

## Credits

PAC-MAN is a registered trademark of Bandai Namco Entertainment Inc.
This is an independent fan tribute for educational purposes and is not
affiliated with or endorsed by Bandai Namco.
