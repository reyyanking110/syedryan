<div align="center">

  <h1>🍎 Catch an Apple — Scratch 2D Game 🎮</h1>

  <p align="center">
    <b>A fun and interactive Scratch game where players control a bowl to catch falling apples and score points!</b>
  </p>

  <p align="center">
    <img src="https://img.shields.io/badge/Platform-Scratch_3.0-orange?style=for-the-badge&logo=scratch&logoColor=white" alt="Scratch Badge"/>
    <img src="https://img.shields.io/badge/Language-Block--Based-blue?style=for-the-badge" alt="Block Coding Badge"/>
    <img src="https://img.shields.io/badge/Category-2D_Arcade-brightgreen?style=for-the-badge" alt="Genre Badge"/>
    <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" alt="Status Badge"/>
  </p>

</div>

---

## 🌟 Game Highlights

* 🥣 **Smooth Mouse Tracking**: The bowl glides horizontally along the bottom following the mouse pointer.
* 🍎 **Random Apple Spawning**: Apples fall continuously from random X-positions at the top of the screen.
* 🔊 **Chomp Sound Effects**: Plays an audio effect (`Chomp`) instantly when an apple is caught.
* 💯 **Score System**: Resets to `0` on launch and increases by `1` point for each successful catch.

---

## 📜 Scratch Code Implementation

### 🥣 1. Bowl Movement
Locks the Y-coordinate to `-150` while updating the X-coordinate continuously to match `mouse x`[cite: 1, 2].

```scratch
when green flag clicked
go to x: 0 y: -150
forever
  go to x: (mouse x) y: -150
