![Unreal Engine Blueprints](https://img.shields.io/badge/Unreal%20Engine-Blueprints-313131?style=for-the-badge&logo=unrealengine&logoColor=white)

# Unreal Engine 5 - Advanced AI & Combat System

https://github.com/user-attachments/assets/fd868a09-2731-46b0-962d-b9fb525530ba

https://github.com/user-attachments/assets/7c5aa5f3-445d-4c23-9dfb-d8ce98ac8584

A modular Third-Person Combat and Enemy AI system built in Unreal Engine. This project demonstrates core gameplay mechanics, AI perception state machines, custom line-trace combat logic, and real-time UI integration.

> Engine Version Requirement:  
> This project requires Unreal Engine 5.8 to open and run properly without asset/blueprint version conflicts.

---

## Key Features

### Enemy AI & Behavior System
* Perception & Field of View: AI detects the player upon entering its Line of Sight (LoS).
* State Machine Transitions: Dynamic movement switching (Walking on patrol -> Running in pursuit -> Searching).
* Last Known Location Tracking: When LoS is broken, the AI moves to the last recorded player position using debug traces and executes a perimeter search animation.
* Combat AI: Automated attack logic upon entering close range.

### Player Combat & Defense Mechanics
* Target Lock-On: Fixed camera lock system centered on the active target for precise movement.
* Sword Combat & Line Traces: Weapon hit detection calculated via precise debug line traces.
* Blocking Logic: Defensive guard stance that interacts directly with health logic to mitigate incoming damage (75% damage reduction).

### UI & Feedback Systems
* Real-time Health Logic: Direct link between incoming hit events and UI health bar updates.
* Visual Screen Feedback: Screen-edge color overlays for damage feedback and pickup healing events.

---

## Prerequisites & Setup

1. Unreal Engine 5.8 installed via Epic Games Launcher.
2. Clone this repository:
   git clone https://github.com/SbcInteractive/UE-Combat-AI-Framework.git
3. Open Unreal-AI-Combat-System.uproject using Unreal Engine 5.8.
