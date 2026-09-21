# Neon District — Game Design

## Premise
A fictional coastal city is divided into neighborhoods controlled by competing crews, private security, and local businesses. The player builds a reputation by taking jobs, exploring the city, and improving mobility and equipment.

## Player
- Movement: walk, sprint, crouch
- Traversal: vehicles and climbable world props
- Combat prototype: non-graphic, arcade-style ranged and melee interactions
- Progression: reputation, cash, vehicle collection, equipment upgrades

## World
Initial vertical slice:
- Downtown
- Industrial yard
- Residential block
- Gas station / convenience store
- Vehicle garage
- Safehouse

## Mission framework
Each mission is data-driven:
- id
- title
- briefing
- start location
- objectives
- completion conditions
- reward
- failure conditions

## Mobile controls
Left side:
- virtual movement stick

Right side:
- interact
- sprint
- vehicle brake/handbrake
- primary action

Contextual buttons appear only when relevant.

## Performance budget
Target 30 FPS on lower-end supported Android devices and 60 FPS on higher-end devices.
Prefer baked lighting where possible, pooled NPC/vehicle entities, LOD groups, occlusion culling, texture compression, and streamed world chunks.
