<div align="center">

  <!-- Header Banner -->
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:FF4B4B,100:FF8C00&height=220&section=header&text=🍎%20Catch%20An%20Apple&fontSize=48&fontColor=ffffff&animation=fadeIn&fontAlignY=38" width="100%" alt="Header Banner" />

  <br/>

  <!-- Badges -->
  <p align="center">
    <a href="https://scratch.mit.edu/"><img src="https://img.shields.io/badge/ENGINE-SCRATCH_3.0-FF6B6B?style=for-the-badge&logo=scratch&logoColor=white" alt="Scratch 3.0" /></a>
    <a href="https://github.com/reyyanking110/syedryan"><img src="https://img.shields.io/badge/GENRE-2D_ARCADE-4ECDC4?style=for-the-badge&logo=gamepad&logoColor=white" alt="Genre" /></a>
    <a href="https://github.com/reyyanking110/syedryan"><img src="https://img.shields.io/badge/LANGUAGE-BLOCK_BASED-FFE66D?style=for-the-badge&logo=codefactor&logoColor=black" alt="Language" /></a>
    <a href="https://github.com/reyyanking110/syedryan/stargazers"><img src="https://img.shields.io/github/stars/reyyanking110/syedryan?style=for-the-badge&color=FFD166" alt="Stars" /></a>
  </p>

  <p align="center">
    <b>An interactive, fun 2D arcade game built in Scratch! Control the bowl with smooth mouse movement to catch falling apples and score points.</b>
  </p>

</div>

---

## ⚡ Key Highlights

| Component | Technical Implementation |
| :--- | :--- |
| **🥣 Bowl Control** | Lock Y at `-150` & continuously track cursor X via `mouse x`[cite: 1, 2] |
| **🍎 Apple Physics** | Spawn at top (`y: 150`, random `x`), continuous downward movement (`change y by -5`)[cite: 2] |
| **🔊 Collision Handling** | Detect `touching Bowl`, trigger `Chomp` audio effect, hide sprite & reset[cite: 3, 4] |
| **💯 Dynamic Scoring** | Reset score to `0` at start, increment by `+1` per caught apple[cite: 3, 4] |

---

## 🎮 Game Code Implementation

<details open>
<summary><b>🥣 1. Bowl Movement System</b></summary>

<br/>

```scratch
when green flag clicked
go to x: (0) y: (-150)
forever
    go to x: (mouse x) y: (-150)
end
