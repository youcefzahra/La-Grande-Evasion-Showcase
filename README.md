# 🧟 La Grande Évasion - 3D Multiplayer Escape Game

> **Showcase Repository:** To comply with EPITA's anti-plagiarism regulations, the raw source code of this project is kept private. This repository serves as an architectural showcase documenting the game mechanics, the AI behavior, and the multiplayer network logic.

## 📖 Project Context

**La Grande Évasion** is a 3D cooperative escape game (1 to 4 players) developed in Unity as a first-year final project at EPITA. Players are trapped in a medical prison and must collaborate to solve puzzles while evading a guard controlled by artificial intelligence.

**My Role:** In this 4-person team project, I was personally responsible for two major pillars of the game: the antagonist's Artificial Intelligence ("The Plague") and the multiplayer network synchronization logic via Photon PUN 2.

## 🏗️ Technical Architecture & Features

### 1. Enemy AI & Network Logic (My Core Contributions)
* **Tracking System & Vision Cone:** Developed the enemy's autonomous behavior using a State Machine. The AI patrols and triggers a chase upon detecting players through a dynamic red-light vision cone emitting from its eyes and lantern.
* **Combat & Penalties:** Programmed the damage system (4 hits to eliminate a player) and the respawn logic (automatic player teleportation to their initial cell).
* **Real-Time Synchronization:** Managed the network lobby, player spawn system, and synchronized state variables (health points, positions, actions) across all clients via RPC (Remote Procedure Call) requests to ensure a fluid co-op experience.

### 2. Mechanics & Level Design (Team Contributions)
* **Custom Character Controller:** A physics-safe C# movement system with continuous raycasting to prevent wall-clipping and handle dynamic animation blending.
* **Synchronized Puzzles & Environment:** Networked inventory preventing item duplication, state-driven cooperative puzzles, and a fully lit 3D medical prison utilizing Unity's NavMesh for complex AI navigation.

## 🎯 Installation & Playable Demo

A pre-compiled Windows installer and its instruction manual are available for testing.

1. Go to the **[Releases](../../releases)** tab of this repository.
2. Download `La Grande Evasion 1.1 Setup (x64).exe` and the installation manual.
3. Run the setup and follow the manual's instructions to connect to the multiplayer server and play.

### Gameplay Overview

https://github.com/user-attachments/assets/8685f126-00c0-49c2-bbe8-20ad76577cee

## 👥 The Team
* **[Youcef Zahra](https://github.com/youcefzahra)**
* **[Wael Akhdar](https://github.com/Wael-Akhdar)**
* **[Jessim Ziani](https://github.com/jessim-ziani)**
* **[Ilann Oller]()**
