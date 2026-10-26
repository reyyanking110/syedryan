<div align="center">

  # 🍎 Catch an Apple - Scratch Game

  <img src="https://readme-typing-svc.herokuapp.com?font=Fira+Code&weight=600&size=24&pause=1000&color=FF4B4B&center=true&vcenter=true&width=500&lines=Interactive+Scratch+2D+Game;Catch+Apples+%2B+Score+Points!;Simple+%26+Fun+Block+Coding" alt="Typing SVG" />

  <p align="center">
    <b>A fun and interactive Scratch game where players control a bowl to catch falling apples and score points! 🎮</b>
  </p>

  <p align="center">
    <img src="https://img.shields.io/badge/Platform-Scratch-orange?style=for-the-badge&logo=scratch&logoColor=white" alt="Scratch Badge"/>
    <img src="https://img.shields.io/badge/Language-Block--Based-blue?style=for-the-badge" alt="Block Coding Badge"/>
    <img src="https://img.shields.io/badge/Genre-2D%20Arcade-green?style=for-the-badge" alt="Genre Badge"/>
  </p>

</div>

---

## 🌟 Features

*  bowl **Mouse Control**: Bowl moves smoothly horizontally following the mouse cursor.
* 🍎 **Random Apple Spawning**: Apples drop randomly from the top of the screen.
* 🔊 **Audio Effects**: Plays a fun `Chomp` sound whenever an apple is caught.
* 💯 **Dynamic Score System**: Score resets to `0` at start and increments by `1` with every catch.

---

## 📜 Scratch Code Logic Breakdown

### 🥣 1. Bowl Movement Script
Sets the bowl at the bottom-center and locks its Y-axis while allowing it to follow the mouse X-position.

```scratch
when green flag clicked
go to x: 0 y: -150
forever
  go to x: (mouse x) y: -150
