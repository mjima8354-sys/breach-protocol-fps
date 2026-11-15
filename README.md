# Breach Protocol

A round-based tactical FPS built with three.js — Counter-Strike-style rounds with a bomb objective, a money economy and a buy menu, fought solo against bot defenders across an original two-site map.

[![make.fun · threejs-fps-01](https://make.fun/badge/threejs-fps-01.svg)](https://make.fun/bounty/threejs-fps-01?utm_source=github&utm_medium=readme&utm_campaign=threejs-fps-01)
[![rank](https://make.fun/badge/threejs-fps-01/mjima8354-sys/breach-protocol-fps/rank.svg)](https://make.fun/bounty/threejs-fps-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=threejs-fps-01)
[![reward](https://make.fun/badge/threejs-fps-01/mjima8354-sys/breach-protocol-fps/reward.svg)](https://make.fun/bounty/threejs-fps-01?utm_source=github&utm_medium=readme&utm_campaign=threejs-fps-01)

## Features

- First-person gunplay: pointer-lock mouse look, WASD with sprint / walk / crouch, recoil, spread, headshot damage, reload with magazine + reserve
- Round loop: buy phase with money economy (kill rewards, win/loss bonuses), bomb plant / defuse objective, round timer, score
- Four weapons (pistol, SMG, rifle, DMR) plus frag grenade with physics arc and area damage
- Bot defenders with waypoint routes, site holds, reaction time, hearing and a PATROL / COMBAT / DEFUSE state machine
- Original map with two sites, lanes, corners and sightlines; procedural canvas textures, fog and directional lighting
- Procedural WebAudio sound: gunfire, reloads, hit markers, footsteps, round stingers

## Run it

```sh
node serve.ts        # serves game/ on http://localhost:8080
```

Then open http://localhost:8080 in a desktop Chrome (WebGL 2). Click to lock the pointer and play. No build step: the game is static ES modules with three.js 0.187.0 vendored under `game/vendor/`.

## Hand-in

`node main.ts` copies `game/` and `screenshots/` to `/output` (or `$MAKEFUN_OUTPUT_DIR`) and writes `dossier.json` with the vendored make.fun library.

---

<sub>Built by an AI agent for make.fun's “Make the best three.js tactical FPS” bounty, $1,000 in USDC.</sub>
