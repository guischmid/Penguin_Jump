# Penguin Jump

## Overview

This project is a 2D vertical platformer game developed in Unity. It showcases gameplay mechanics such as movement, power ups, and weapon use, and was created as part of an exam project.

## 🐧 Play in the Browser — Rebuilt Edition

The game has been rebuilt from scratch as a single self-contained HTML5 file: **[`docs/index.html`](docs/index.html)**. No Unity, no build step, no assets to download — just open the file in any modern browser (double-click it, or serve the repo and visit `/docs/`). To host it online, enable GitHub Pages for this repository (Settings → Pages → Deploy from branch → `/docs` folder).

The remake keeps the original's design — climb procedurally generated platforms, grab power-ups, dodge or shoot monsters, and stay ahead of the rising lava — and improves on it:

- **Better jump feel** — coyote time, jump buffering, and variable jump height replace the original's "press the space bar harder and longer" workaround
- **Fair generation** — every platform is mathematically guaranteed to be reachable, including moving platforms at their travel extremes
- **Stomp attack** — land on monsters to defeat them (in addition to throwing snowballs with <kbd>E</kbd>)
- **Invulnerability frames** after taking damage, instead of monsters self-destructing on first contact
- **High score** persisted in the browser, pause menu, auto-pause when the tab loses focus
- **Procedural audio** (WebAudio) with a mute toggle — no sound files needed
- **Altitude-reactive sky** — day fades through dusk into a starfield as you climb, with parallax glacial mountains and snowfall
- **Touch controls** on mobile devices
- All five platform types (static, disappearing, crumbling, and both movers), all four power-ups (trampoline, wings, double jump, extra life), rising lava with score-based speed-up, hearts UI, and the grayscale game-over fade — faithfully recreated

**Controls:** ← → / A D to move · Space / W / ↑ to jump · E to throw snowballs · P to pause · M to mute

## Features

- Smooth character movement
- Jumping mechanics
- Weapon usage
- Custom shaders and visual effects
- Developed with Unity using C#, ShaderLab, and HLSL

## Setup

To use the repository and access all its contents, it is **necessary** to install and set up Git LFS (Large File Storage).  
Follow the instructions here: [GitHub - Installing Git Large File Storage](https://docs.github.com/en/repositories/working-with-files/managing-large-files/installing-git-large-file-storage)

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/guischmid/Penguin_Jump.git
    ```
2. Open the project in [Unity Editor](https://unity.com/).
3. Select the MainMenu scene at Assets/Scenes.
4. Press the **Play** button in the Unity Editor to start the game.

## Requirements

- Unity (specify version, e.g., 2021.3 or later)
- Git LFS extention

## How to Execute the Built File on MacOS that was created on Windows

> **Note:** The built file for Mac cannot be compressed as a ZIP file. If you do, the game will no longer be executable. Therefor, a TAR file is the best solution. 

1. Decompress the TAR file.
2. Open a terminal and enter:
    ```bash
    cd built.app/Contents/MacOS
    ```
    You may need to adjust the command to navigate to the “MacOS” directory, depending on where you saved the TAR file.
3. Enter:
    ```bash
    chmod -R 755 game
    ```
4. Now you can double-click on the built application and the game should run. Force execute the file if your anti-virus program blocks the execution.

## How to Play
- **Move Left:** Press the **Left Arrow** key
- **Move Right:** Press the **Right Arrow** key
- **Jump:** Press the **Space Bar**
  > **Note:** The space bar should be pressed harder and longer to reach other objects properly. 
- **Use Weapon:** Press the **E** key

## Project Structure

```
...
├── Assets
│   ├── Animated effects
│   ├── Art
│   ├── Buttons
│   ├── Chibi Monster Free (Unique Skill Animated Prefab with SFX)
│   ├── DefaultVolumeProfile.asset
│   ├── Editor
│   ├── Fonts
│   ├── MainMenuBG.png
│   ├── Materials
│   ├── Nine Pines Animation
│   ├── Prefabs
│   ├── Presets
│   ├── Resources
│   ├── Scenes
│   ├── Scripts
│   ├── Settings
│   ├── Settings.meta
│   ├── test_scene.unity
│   ├── TextMesh Pro
│   ├── UI
│   ├── UI pack
│   ├── UniversalRenderPipelineGlobalSettings.asset
│   ├── Warped Shooting Fx
...
```

## Credits

- Developed by [lea10k](https://github.com/lea10k)
- Developt by [EfusRyuga](https://github.com/EfusRyuga)
