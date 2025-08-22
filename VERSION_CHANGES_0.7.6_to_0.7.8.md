# Version Changes: 0.7.6 ROCK to 0.7.8

This document outlines the changes between Mage Arena versions 0.7.6 ROCK and 0.7.8, focusing on class additions, removals, and modifications that are relevant for modding.

## New Classes in 0.7.8

### Core Game Systems
- `AiMAgeBook` - New AI behavior system for the mage book
- `BlockEditorEntry` & `BlockListEditor` - New block editing functionality
- `Colorblindness` - New accessibility feature
- `CustomizeHighlightColor` - New visual customization option
- `DethRobeRaycaster` - New robe interaction system
- `ForceFieldTeam` - New team-based force field system
- `IHitableMonster`, `IInteractable`, `IInteractableNetworkObj`, `IItemInteraction`, `ISpell`, `ISpellCommand`, `ITimedInteractable` - New interfaces for game systems
- `PixelArtDrawingSystem` & `PixelArtDrawingSystemVisual` - New drawing system
- `RaycastAudioDamper` - New audio spatialization system
- `SpineSyncer` - New animation synchronization system

### Gameplay Elements
- `FrogBalloon` - New interactive object
- `FrogBladeController` - New weapon type
- `FrogSpear` - New weapon type
- `KnightDong` - New character component
- `LackyController` - New NPC type
- `MushroomSword` - New weapon type
- `PotInteract` - New interaction type
- `SpellDarkBlast`, `SpellHolyLight`, `SpellRock`, `SpellWisp` - New spell implementations

### UI/UX
- `debugmush` - New debugging utility

## Modified Classes

### Major Changes
- `MageBookController` (previously `MageBook`?) - Significantly expanded functionality
- `PlayerInventory` - Major updates to item handling
- `PlayerMovement` - Significant movement system updates
- `ShadowWizardAI` - Major AI behavior updates
- `SkelemageController` - Updated AI and behavior

### Minor Changes
- `BogFrogController` - Added new interactions
- `ChestNetController` - Updated networking
- `CraftingForge` - New crafting recipes/interactions
- `Dissonance` integration files - Updated voice chat implementation
- `DungeonGenerator` - New generation features
- `FishNet` related files - Updated networking code
- `PlayerAudioPlayer` - New audio features
- `ResourceManager` - New resource handling
- `SettingsHolder` - New settings and options

## Removed Classes
- `ExampleSpellLightningBolt` - Moved/renamed
- `ManBlinls` - Removed or renamed
- `Serverchecksiguess` - Removed or consolidated

## New Namespaces and Folders
- `BlueRaja/` - Updated priority queue implementations
- `Dissonance.Integrations.Offline/` - Updated voice chat
- `DrawPixels_Done/` - New drawing system components
- `FishNet.*/` - Updated networking namespaces
- `Gameplay.VoiceChat/` - New voice chat implementation
- `Recognissimo.Samples/` - New voice recognition samples

## Modified Systems
1. **Networking**
   - Updated FishNet integration
   - New network behaviors and sync systems

2. **Combat**
   - New spell implementations
   - Updated weapon systems
   - New AI behaviors

3. **UI/UX**
   - New accessibility options
   - Updated HUD elements
   - New visual feedback systems

4. **Audio**
   - New spatial audio features
   - Updated voice chat
   - New sound effects

## Notes for Modders
- Several interfaces have been formalized (`IHitableMonster`, `IInteractable`, etc.)
- New event systems for interactions
- Updated networking requires attention to new sync behaviors
- Many existing mods may need updates for compatibility
- New hook points available for mod integration

## Breaking Changes
- Some class names have changed
- Method signatures in core systems have been updated
- Network behavior modifications may affect existing multiplayer mods
- Resource loading has been updated, affecting asset bundle handling
