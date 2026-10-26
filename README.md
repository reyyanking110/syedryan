<div align="center">

  <!-- Animated Header Banner -->
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:FF4B4B,100:FF8C00&height=220&section=header&text=🍎%20Catch%20An%20Apple&fontSize=48&fontColor=ffffff&animation=fadeIn&fontAlignY=38" width="100%" alt="Header Banner" />

  <br/>

  <!-- Animated Badges -->
  <p align="center">
    <a href="https://scratch.mit.edu/"><img src="https://img.shields.io/badge/Engine-Scratch_3.0-FFAB19?style=for-the-badge&logo=scratch&logoColor=white" alt="Scratch 3.0" /></a>
    <a href="https://github.com/reyyanking110/syedryan"><img src="https://img.shields.io/badge/Type-2D_Arcade_Game-00C853?style=for-the-badge&logo=gamepad&logoColor=white" alt="Game Type" /></a>
    <a href="https://github.com/reyyanking110/syedryan"><img src="https://img.shields.io/badge/Language-Block--Based-00B0FF?style=for-the-badge&logo=codefactor&logoColor=white" alt="Block Coding" /></a>
    <a href="https://github.com/reyyanking110/syedryan/stargazers"><img src="https://img.shields.io/github/stars/reyyanking110/syedryan?style=for-the-badge&color=FFD700" alt="Stars" /></a>
  </p>

  <p align="center">
    <b>An engaging, interactive 2D arcade game built in Scratch! Players control a bowl using real-time mouse movement to catch falling apples and score points.</b>
  </p>

</div>

---

## ⚡ Quick Overview

| Feature | Description |
| :--- | :--- |
| **🎮 Controls** | Real-time horizontal Mouse Tracking (`mouse x`)[cite: 1, 2] |
| **🍎 Mechanics** | Random X-Spawning & Continuous Downward Y-Velocity (`-5`)[cite: 2] |
| **🔊 Audio** | Instant collision sound effect (`Chomp`)[cite: 3, 4] |
| **💯 Scoring System** | Auto-resets to `0` at start and increments by `+1` per catch[cite: 3, 4] |

---

## 🎮 Game Architecture & Code Blocks

### 1️⃣ Bowl Controller Script
Moves the bowl horizontally while keeping its vertical position fixed at the bottom of the screen[cite: 1, 2].

```scratch
when green flag clicked
go to x: (0) y: (-150)
forever
    go to x: (mouse x) y: (-150)
end
