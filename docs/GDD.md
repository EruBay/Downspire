# Game Design Document - Downspire

> Last Updated: January 2025  
> Version: 1.0.0

## Table of Contents

1. [Game Overview](#game-overview)
2. [Core Gameplay Loop](#core-gameplay-loop)
3. [Game Mechanics](#game-mechanics)
4. [Visual Design](#visual-design)
5. [Level Design](#level-design)
6. [Systems Design](#systems-design)
7. [Narrative](#narrative)
8. [Monetization](#monetization)
9. [Technical Requirements](#technical-requirements)

## Game Overview

### Concept Statement
Downspire is a top-down roguelite where players descend from floor 100 to floor 1 of a mysterious tower. Each death returns you to the top, but collected "Echoes" persist for permanent character upgrades.

### Core Pillars
1. **Meaningful Death** - Every run teaches you something
2. **Environmental Storytelling** - Each floor tells a story
3. **Satisfying Progression** - Both skill and stats improve
4. **Atmospheric Immersion** - Dark, mysterious, compelling

### Target Audience
- Primary: Roguelite fans (Hades, Gungeon players)
- Secondary: RPG enthusiasts who enjoy progression
- Tertiary: Souls-like fans who appreciate challenge

### Unique Selling Points
- Inverted tower progression (top to bottom)
- Themed floors with unique bosses and key items
- Environmental storytelling through level design
- 2.5D perspective combining depth with clarity

## Core Gameplay Loop

### Macro Loop (Run)
```mermaid
graph LR
    A[Start Floor 100] --> B[Explore Floor]
    B --> C[Combat Enemies]
    C --> D[Find Boss]
    D --> E[Defeat Boss]
    E --> F[Collect Key Item]
    F --> G[Unlock Door]
    G --> H[Descend]
    H --> I{Death?}
    I -->|Yes| J[Collect Echoes]
    I -->|No| B
    J --> K[Upgrade Character]
    K --> A
Micro Loop (Floor)

Enter floor
Explore rooms
Fight enemies
Collect loot/echoes
Find boss room
Boss battle
Claim key item
Find and unlock exit

Game Mechanics
Movement

8-directional movement with analog stick support
Base speed: 5 units/second
Dodge roll: 8 units distance, 0.5s duration, 0.2s i-frames
Environmental interaction: Push objects, activate switches

Combat
See detailed documentation: Combat System
Progression
See detailed documentation: Meta Progression
Visual Design
Camera System

Type: 2.5D top-down perspective
Angle: 45-60 degrees
Features:

Smooth follow with lookahead
Combat zoom-out
Dramatic moment zoom-in
Screen shake for impact



Art Direction

Style: Dark fantasy with environmental decay
Palette: Varies by floor theme
Lighting: Dynamic shadows, ambient glow
Effects: Particle systems for atmosphere

Level Design
Floor Structure

Size: 15-20 rooms per floor
Layout: Procedural with handcrafted rooms
Secrets: 1-3 per floor
Pacing: Combat -> Exploration -> Boss

Example Floors
See detailed documentation: Floor Themes
Systems Design
Enemy AI

Behavior Trees for complex enemies
State Machines for simple enemies
Aggro System with sight/sound detection
Coordinated Attacks for group encounters

Loot System

Echoes: Meta-currency (persistent)
Coins: Floor currency (lost on death)
Items: Temporary power-ups
Artifacts: Permanent collection items

Narrative
See detailed documentation: Narrative
Monetization
Business Model

Premium Game: $19.99 USD
No Microtransactions
Potential DLC: New character classes, floor packs

Platform Strategy

Steam Early Access
Full Steam Release
Console Ports (Switch, PlayStation, Xbox)

Technical Requirements
Minimum Specs

OS: Windows 10
CPU: Intel i3 or equivalent
RAM: 4GB
GPU: GTX 750 or equivalent
Storage: 2GB

Performance Targets

Resolution: 1920x1080
Framerate: 60 FPS stable
Load Times: <3 seconds between floors


Back to Documentation

---

## /docs/CHANGELOG.md

```markdown
# Changelog

All notable changes to Downspire will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- Initial project setup
- Basic movement system
- Camera controller
- Project documentation

### Changed
- Switched from 3D to 2D implementation
- Refined camera angle to 45 degrees

### Fixed
- N/A

## [0.1.0] - 2025-01-XX

### Added
- Unity project initialization
- Basic folder structure
- Core documentation
- GitHub repository setup

---

[Unreleased]: https://github.com/yourusername/downspire/compare/v0.1.0...HEAD
[0.1.0]: https://github.com/yourusername/downspire/releases/tag/v0.1.0
