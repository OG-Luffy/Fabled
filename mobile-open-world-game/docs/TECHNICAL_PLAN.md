# Technical Plan

## Unity architecture

### Systems
- GameBootstrap
- InputSystem
- PlayerController
- VehicleController
- InteractionSystem
- MissionSystem
- NPCSystem
- WantedSystem
- SaveSystem
- WorldStreamingSystem
- AudioSystem
- UI/HUD

### Data
Use ScriptableObjects for static gameplay definitions:
- MissionDefinition
- VehicleDefinition
- WeaponDefinition
- ItemDefinition
- NPCArchetype

Use JSON/local storage for player save state.

## Mobile optimization
- Object pooling for NPCs, vehicles, VFX
- Addressables for large assets
- Scene additive loading / world chunks
- GPU instancing
- LOD and occlusion culling
- Reduced shadow distance on low presets
- Quality profiles: Low / Medium / High / Ultra
