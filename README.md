# Carnage Karts

A voxel-space kart racer that runs in the browser. Six cute animal racers, three laps, weapon pickups, and a very messy finish (gore can be set to Off, On or Extra on the menu).

**Play:** https://corysyx.github.io/critter-carnage-karts/

## Controls

**Keyboard:** arrows / WASD to drive · Shift to drift (hold for a mini-boost) · Space to use an item · R back to track · P pause · M mute

**Phone:** play in landscape. Choose **Buttons** or **Tilt** steering on the menu. Tilt uses the phone's motion sensor (on iPhone, Safari asks for permission the first time). Auto-gas is on by default.

## Items

| Item | What it does |
|---|---|
| Carrot Rocket | Homes in on the racer ahead (gory) |
| Buzz Saw | Fires straight forward (gory) |
| Spike Mine | Dropped behind you (gory) |
| Slime Puddle | Spins out whoever drives into it |
| Sugar Rush | Speed boost |
| Bubble Shield | Blocks one hit |

## Tech

Everything is in `index.html`: no build step and no dependencies. Terrain is drawn with a column-by-column ray-cast voxel heightmap renderer (Comanche-style) into a 2D canvas; racers, items and particles are depth-tested 2D sprites.
