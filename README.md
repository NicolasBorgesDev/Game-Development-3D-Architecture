# 🎮 Game Development & 3D Architecture (Portfolio Showcase)

> **Note:** The complete source code and raw project files for these systems are private due to commercial NDAs and proprietary mechanics. This repository serves as a comprehensive technical portfolio showcasing my expertise in gameplay engineering, multiplayer architecture, and 3D asset pipelines across industry-standard engines.

![Unreal Engine](https://img.shields.io/badge/Unreal_Engine-5.3-0E1128?style=for-the-badge&logo=unrealengine&logoColor=white)
![UEFN](https://img.shields.io/badge/UEFN-Verse-000000?style=for-the-badge&logo=epicgames&logoColor=white)
![Unity](https://img.shields.io/badge/Unity-2022.3-000000?style=for-the-badge&logo=unity&logoColor=white)
![Blender](https://img.shields.io/badge/Blender-3D_Modeling-F5792A?style=for-the-badge&logo=blender&logoColor=white)
![C++](https://img.shields.io/badge/C++-System_Architecture-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![C#](https://img.shields.io/badge/C%23-Scripting-239120?style=for-the-badge&logo=c-sharp&logoColor=white)

---

## 📌 Executive Summary

This portfolio highlights my end-to-end capabilities as a Technical Game Developer. My focus lies at the intersection of **Systems Engineering** (building scalable match flows, tactical mechanics, and multiplayer replication) and **Technical Art** (3D modeling, material setups, and asset optimization). 

The showcase is divided into three core pillars:
1. **Unreal Engine & UEFN (Verse/C++):** Multiplayer match architecture, tactical FPS mechanics, and dynamic HUDs.
2. **Unity (C#):** Cross-platform mechanics, state machines, and physics-based gameplay.
3. **3D Asset Pipeline (Blender):** Character concepting, modeling, texturing, and engine integration.

---

## 🕹️ Pillar 1: Unreal Engine & UEFN (Multiplayer Systems)

Developing for the Fortnite ecosystem and standalone Unreal projects requires strict adherence to memory limits and network replication standards.

<p align="center">
  *<img width="1891" height="1031" alt="Captura de tela 2026-01-17 233821" src="https://github.com/user-attachments/assets/2474dd3e-802f-470a-b98f-603807e8e181" />
  *
  <img width="1642" height="948" alt="Captura de tela 2026-06-09 132154" src="https://github.com/user-attachments/assets/948c1a2c-99ac-4eec-8577-46c92c7d603c" />
  <img width="1908" height="1074" alt="Captura de tela 2026-01-17 233553" src="https://github.com/user-attachments/assets/89bd349b-2823-49b9-ac69-a76e64f95d25" />

</p>

### Key Technical Implementations:
- **Match Flow Architecture:** Built robust state machines using Verse to handle pre-game lobbies, round transitions, objective spawning, and end-game score calculation without server desync.
- **Tactical Multiplayer Mechanics:** Implemented team-based round management, custom loadout granters, and zone-control logic.
- **Dynamic HUD & UI Systems:** Engineered responsive user interfaces that react to in-game events (e.g., health states, objective captures, match timers) using UMG and Verse UI integrations.
- **Gameplay Event Systems:** Created modular event dispatchers allowing environment hazards and cinematic sequences to trigger seamlessly during live gameplay.

---

## 🧊 Pillar 2: 3D Modeling & Technical Art (Blender)

A game is only as good as its visual optimization. This section highlights my pipeline for creating game-ready assets, focusing on a custom series of "Elemental" characters (Ice, Nature, Magma, etc.).

<p align="center">
  *  <img width="1621" height="917" alt="Captura de tela 2026-07-03 103103" src="https://github.com/user-attachments/assets/49eefa68-da5b-4cca-8265-ffc05be4f19b" />
*
  <img width="1903" height="1008" alt="Captura de tela 2026-10-25 094743" src="https://github.com/user-attachments/assets/af9cc747-cf6b-429d-82d9-036264e0af65" />

<img width="1607" height="924" alt="Captura de tela 2026-07-03 103039" src="https://github.com/user-attachments/assets/27187c0d-ab1a-4573-b983-afcee9782f75" />

</p>

### Workflow & Pipeline:
- **Character Concepting & Modeling:** Designed distinct "pill-shaped" elemental base meshes with varied thematic accessories (translucent ice, emissive magma, mossy rocks) while maintaining a unified skeletal structure.
- **Material & Shader Setup:** Configured complex materials including sub-surface scattering for organic elements, dynamic emissive nodes for glowing eyes/runes, and translucent shaders for water/ghost elementals.
- **Rigging & Engine Import:** Ensured all topology is animation-ready, bound to efficient rigs, and correctly imported into the engine with optimized LODs (Level of Detail) to prevent draw-call bottlenecks.

---

## ⚙️ Pillar 3: Unity Engineering (C# Scripting)

<p align="center">
  *    <img width="1501" height="902" alt="Captura de tela 2026-05-15 041122" src="https://github.com/user-attachments/assets/43c52b2a-e96b-4446-afac-d5462bc8c2b3" />
*
  <img width="1675" height="1074" alt="Captura de tela 2026-01-17 234003" src="https://github.com/user-attachments/assets/c7af6d53-ec72-4f5b-baa3-b20bb66d9809" />

</p>

### System Highlights:
- **Component-Based Architecture:** Developed decoupled, reusable C# scripts for player controllers, enemy AI behaviors, and inventory management.
- **Physics & Collision Matrices:** Optimized Rigidbody physics and collision layers to ensure smooth movement and accurate hit-detection in fast-paced scenarios.
- **Data Persistence:** Implemented robust save/load systems using JSON/Binary serialization to manage player progression and settings across sessions.

---

## 🧠 Engineering Challenges & Solutions

### Challenge 1: Multiplayer State Synchronization
- **Scenario:** In fast-paced tactical rounds, late-joining players or temporary network drops caused desyncs in match timers and team scores.
- **Solution:** Shifted the source of truth entirely to the server-side logic (using Verse/C++). Implemented state-replication variables that force the client UI to rebuild its state based on the server payload upon reconnection, ensuring 100% consistency.

### Challenge 2: 3D Asset Performance Overhead
- **Scenario:** Using highly detailed models with emissive and translucent materials caused frame drops on lower-end hardware.
- **Solution:** Established a strict polycount budget in Blender. Baked high-poly details into Normal maps and consolidated material IDs to reduce engine draw calls.

---

## 👨‍💻 Let's Connect

- **LinkedIn:** [Nicolas Borges](https://www.linkedin.com/in/nicolas-borges-a1b941191/)
- **GitHub:** [@NicolasBorgesDev](https://github.com/NicolasBorgesDev)
- **E-mail:** [niicolasrodriigues2@outlook.com](mailto:niicolasrodriigues2@outlook.com)
