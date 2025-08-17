# Mage Arena Modding Class Catalog

This repository documents decompiled Mage Arena classes and organizes them into categories useful for modding.

## Version
These classes were extracted from Mage Arena Version 0.7.6 ROCK. Please note that they may change in future versions and would need to be updated.

## Why this exists
- This list was made to help with creating mods for Mage Arena.

## How to use
- Start with the Categories section below to find candidate classes to patch or extend.
- Use the Ignore section to avoid patching compiler-generated iterator classes.

### Core Game Flow
- BootstrapManager, BootstrapNetworkManager, MainMenuManager, MainMenuManagerNetworked, ResourceManager, SettingsHolder
- FindPublicLobbies, LobbyDataEntry, ShowLobbyCode
- EnableMeshRenderers, ToggleDungeonMeshRenders, SceneHDRPSettingsSetter, SetUpModelProvider

### Player Systems
- PlayerMovement, PlayerRespawnManager, PlayerInventory, PlayerInteract, PlayerMapIconController
- PlayerAudioPlayer, PlayerVolumeSettingsController, PushtoTalk, NameTagDistanceCulling
- VoiceControlListener, RenableCursorOnMenus

### Progression and Items
- ItemSpawner, SpawnNetworkedItem, ChestInteract, ChestInteract1, ChestNetController, ChestNetController1
- PageLootTable, PageController, PaperInteract, PaperMover, LogItem
- CraftingForge, CraftInteracter, CraftHammerController, WardController
- PoofController, PoofSpell, PullExcalibur, ExcaliburController, ExcaliberBlade, ExcaliberHilt

### Networking and Multiplayer
- NetInteractionManager, NetworkedFireballController, FindPublicLobbies, MainMenuManagerNetworked
- ShowLobbyCode, KickPlayersHolder, SetChatMessage

### Combat and Spells
- BlinkSpellController, MagicMissleController, FireballController, FireballFireController
- DartController, DartGunController, DarkBlastController, FrostBoltController
- LightningBoltSpellController, LightningBoltDamage, LightningLookAt, HolyLightSpell
- RockSpellController, RockController, RockCheckSphere, ExplosionController
- SmokeCloud, SmokeRingController, SwordController, TorchController
- TorchHitDetection, WeaponHitDetection, WormholeTele, RespawnWormhole
- FreezeHitController, ShrinkRay

### AI and NPCs
- ShadowWizardAI, ShadowWizardAnimationController, SkelemageController, SkelemageAniController
- SkeletoneController, SkeletoneBodyPart, GolemController, GolemGuyAdder
- BoneDogController, BoneDogTargets, BogFrogController, BogFrogSingleController, BogFrogInteractor, SporeFrog
- SoupManController, SoupManInteractor, DuendeManager, DuendeController, DuendeInteractor, DuendeRagdollAudio
- MushroomGuyController, MushroomManTrigger, FallenKnight, FallenKnightNet, CastleWraithController
- RavenController, RavenSpawner, NpcOpenDoor, MonsterHitScript
- AINodes, DungeonPathfinder2D, GetHexAiNodes, GetShadowWizardController

### World and Environment
- DungeonGenerator, Generator2D, Grid, Grid2D, Delaunay2D
- WeatherCycle, NightAudioSwap, RoomEnabler, RoomPrefabEnabler
- DoorOpen, DoorInteract, DoorInteract1, PortcullisController, PortcullisNetController
- BrazierInteract, BrazzerInteract, CastleFlagCapturedNotifier, FlagController, FlagPositionLerper
- ColoseumManager, ColoseumPots
- BounceMushroomManager, BouncePad, BounceShroomTrigger
- CaveDrip, LavaAudio, FireAudioPlayer, OceanTriggershit, RiverPitchRandomizer
- MoutainWind, MountainWindTrigger, HatSpin, Levitator, WindZome

### Interactables and Props
- ActivateSwizards, BookController, cinemamode, CleetedWalkingStickController
- CrystalReactor, CrystalShard, CrystalSoup, FrogItem, FungalWalkingStick
- GetEntrancePoint, GetMap, GetPlayerGameobject, GetRespPortal, GetRockPlayerOwner, GetSoupFromGuy
- LookatCam, LookatCamera, MagicMirrorController, OrbController
- PerfectedCrystal, PicSwapper, PipeItem, Prim, RoomPrefabEnabler
- SetLabelMic, SetSenseText, SpikeGrower, SpikedRootController, SyncHandPos
- ThrummingStoneController, TitleLetterShake, ToggleDungeonMeshRenders, WalkingStickController, WispController

### UI and UX
- NetHudCanvasHider, MapCGFader, MenuThemeVolumeUpper, HealthBarLerper, KillFeedMessage
- SetChatMessage, ShowLobbyCode, showcheckmark, NameTagDistanceCulling

### Samples and Editor/Demo
- SamplesShowcase, SampleShowcase, FullscreenSamplesEffectSelection
- FitToWaterSurface, FitToWaterSurfaceBurst, ProjectCaustics, FoamBuffer, FoamShore, FloatingIceberg, ShoreDecalTrigger, LinkDirectionalToCustomNightSky, AlignSceneView
- DrawPixels_Done.DrawPixels, DrawPixels_Done.DrawPixelsUI, DrawPixels_Done.DrawPixelsVisual

### Pathfinding / Geometry Utils
- Delaunay2D, Delaunay2D.Triangle, Delaunay2D.Edge
- DungeonPathfinder2D, DungeonPathfinder2D.Node, Generator2D.Room
- Prim, Prim.Edge, CurvedLinePoint, CurvedLineRenderer, LineSmoother
- Graphs.Vertex, Graphs.Edge
- BlueRaja.FastPriorityQueue, BlueRaja.FastPriorityQueueNode
- BlueRaja.GenericPriorityQueue, BlueRaja.GenericPriorityQueueNode
- BlueRaja.SimplePriorityQueue, BlueRaja.SimplePriorityQueue.SimpleNode
- BlueRaja.StablePriorityQueue, BlueRaja.StablePriorityQueueNode

### Networking Internals and Generated
- FishNet.Serializing.Generated_DeltaWriters, FishNet.Serializing.Generated_DeltaReaders
- FishNet.Serializing.Generated.GeneratedComparers___Internal, GeneratedWriters___Internal, GeneratedReaders___Internal
- FishySteamworks.BidirectionalDictionary, CommonSocket, FishySteamworks, ServerSocket, ClientHostSocket, ClientSocket
- UnitySourceGeneratedAssemblyMonoScriptTypes_v1, <PrivateImplementationDetails>

### Tutorial and Docs
- Readme, Readme.Section, TutorialScript, TutorialFlagController, TutorialBrazzier, TutorialGoblin

### Voice and Audio Integration
- DissonanceMicSource, DissonanceProcessAudio, DissonanceSource, DissonanceSpeechSource
- Recognissimo sample scenes: VoiceControlExample, VoiceActivityDetectorExample, SpeechRecognizerExample
- Gameplay.VoiceChat.CustomDissonancePlayer

## Ignore: Compiler-Generated Types
Do not patch compiler-generated iterator/state-machine classes. Match with these glob-like patterns:

```text
*.<>c
*.*<>c
*.<*>d__*
```

Examples: `PlayerMovement.<TelePlayer>d__154`, `SettingsHolder.<>c`.

## Contributions
- CheekyEntity - Initial Catalog

## License
MIT
