# The Last Survivor
The Last Survivor is a top-down 2D shooter built with Python + Pygame.

You control a rotating character who must survive waves of enemies coming from different sides of the map. Shoot, dodge, reload, and stay alive as long as you can.

<img width="1112" height="1140" alt="image" src="https://github.com/user-attachments/assets/3a77e7fb-64ad-45da-bfe4-c12c2b8dde70" />


## Features

### Player
- 360° rotation
- Smooth movement with vector direction
- Health bar with color indicators (green → yellow → red)

### Shooting System
- Bullets fly in the direction of the player's current rotation
- Magazine system (10 bullets by default)
- Reload mechanic (`R` adds 15 bullets)
- Explosion animation on grenade hit
- Shooting sound effects

### Enemy Types
- **Left-side grenadier**  
  - Throws/acts like a rotating grenade  
  - Explodes on contact  
- **Top zombies**  
  - Animated  
  - HP bar  
- **Right-side fast zombies**

### Collision System
- Player takes damage on enemy/grenade hit
- Enemies take bullet damage
- Dead enemies play death sounds and disappear

### Sound System
- Background music  
- Shooting sound  
- Attack / death sounds  
- Explosion sound

## Controls

| Key | Action |
|-----|--------|
| ← / → | Rotate left / right |
| ↑ / ↓ | Move forward / backward |
| **SPACE** | Shoot |
| **R** | Reload (+15 bullets) |
| **ESC** / Window Close | Quit the game |

## Project Structure
```
TheLastSurvivor
│  main.py
│  calibry]i.ttf
│  README.md
│
├─ media
│  ├─ img
│  │   ├─ player/
│  │   ├─ enemy1/
│  │   ├─ enemy2/
│  │   ├─ enemy5/
│  │   ├─ explosion/
│  │   ├─ shell.png
│  │   └─ bg2.jpg
│  └─ snd
│      ├─ Music.wav
│      ├─ shoot.wav
│      ├─ blow.wav
│      ├─ zombie_attack.wav
│      └─ zombie_death1.wav

```

## Requirements

- Python **3.8+**
- **Pygame**

Install dependencies:

```
pip install pygame
```

## Running

From the project root:
```
python main.py
```
