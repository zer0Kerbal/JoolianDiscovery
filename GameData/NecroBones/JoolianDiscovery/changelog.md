# Changelog  
  
| modName    | Joolian Discovery (JOOL)                                         |
| ---------- | ---------------------------------------------------------------- |
| license    | CC-BY-NC-SA-4.0                                                  |
| author     | NecroBones and zer0Kerbal                                        |
| forum      | (https://forum.kerbalspaceprogram.com/index.php?/topic/206954-*) |
| github     | (https://github.com/zer0Kerbal/zer0Kerbal/JoolianDiscovery)      |
| curseforge | (https://www.curseforge.com/kerbal/ksp-mods/JoolianDiscovery)    |
| spacedock  | (https://spacedock.info/mod/95)                                  |
| ckan       | JoolianDiscovery                                                 |

## 0.9.0.0 - Adoption - I can do that Dave

* 17 Feb 2022
* For Kerbal Space Program 1.12.3

### Parts

* lint and reorganize
* updated pointer in model.mu from .dds/.tga/.png --> .dds
* rename part.cfg --> name
* rename model.mu --> `name.mu`
* moved .mu and .dds to Assets\
* mesh --> model

* [KAL.cfg]
  * Command Pod - Polished Menancing Glowing Red Sphere
  * [ModuleCommand]
    * added
      * [Hibernation]
      * [defaultControlPointDisplayName]
      * [CONTROLPOINT] reverse
  * Added:
    * [ModuleKerbNetAccess]
      * Biome
      * Terrain
      * Resources
      * FoV: 5-90
      * Detection %: 2.0
    * [ModuleResourceScanner]
    * [ModuleGPS]
    * [ModuleProbeControlPoint]
      * [minimumCrew] = 0
      * [multiHop] = false
    * [crewReport]
      * [usageReqMaskInternal] = 5
      * [usageReqMaskExternal] = -1
  * asset move
  * lint pass
  * light pass
  * formatting pass
  * localization pass
    * [ModuleSAS]
    * [ModuleScienceContainer]
    * [ModuleKerbNetAccess]
  * drag cubes
* [JoolianBoomTank1.cfg]
  * Fuel Tank
  * asset move
  * lint pass
  * light pass
  * formatting pass
  * localization pass
  * drag cubes
  * ModuleCargoPart pass
* [JoolianBoomTank2.cfg]
  * Fuel Tank
  * asset move
  * lint pass
  * light pass
  * formatting pass
  * localization pass
  * drag cubes
  * ModuleCargoPart pass
* [JoolianBoomTank3.cfg]
  * Fuel Tank
  * asset move
  * lint pass
  * light pass
  * formatting pass
  * localization pass
  * drag cubes
  * ModuleCargoPart pass
* [JoolianCommBox.cfg]
  * Fuel Tank
  * asset move
  * lint pass
  * light pass
  * formatting pass
  * localization pass
  * drag cubes
  * ModuleCargoPart pass
* [JoolianCommTower.cfg]
  * Relay Antenna
  * [category] from Science to Communication
  * [antennaPower] to 200M from 100M
  * [antennaCombinable] is true was false
  * [packetResourceCost] was 10.0 now 24.0
  * [antennaType] set to RELAY
  * asset move
  * lint pass
  * light pass
  * formatting pass
  * localization pass
  * drag cubes
  * ModuleCargoPart pass
* [JoolianEngine.cfg]
  * Engine
  * asset move
  * lint pass
  * light pass
  * formatting pass
  * localization pass
  * drag cubes
  * ModuleCargoPart pass
* [JoolianMainTank.cfg]
  * Fuel Tank
  * asset move
  * lint pass
  * light pass
  * formatting pass
  * localization pass
  * drag cubes
  * ModuleCargoPart pass
* [JoolianMonolith.cfg]
  * Space Object
  * [ModuleCommand]
    * added
      * [Hibernation]
      * [defaultControlPointDisplayName]
      * [CONTROLPOINT] reverse
    * changed [ElectricCharge] from 0.0001 to 0.005
  * [ModuleReactionWheel]
    * changed [ElectricCharge] from 0.01 to 0.0003
  * [ModuleGenerator]
    * changed [ElectricCharge] from 0.01 to 0.0003
  * [ModuleDecouple]
    * added localization
  * add [ModuleCoreHeat]
    * this will need adjustment
    * this part should always be warm to the touch
  * asset move
  * lint pass
  * light pass
  * formatting pass
  * localization pass
  * drag cubes
  * ModuleCargoPart pass
* [JoolianPod.cfg]
  * Command Pod
    * Review needed (versus mk3Cockpit_Shuttle):
      * [mass] = 16 // 3.5
      * [crashTolerance] = 45 // 50
    * Adjusted:
      * [maxTemp] now 2500 was 1500
    * Add
      * [skinMaxTemp] = 2700 // ??
      * [emissiveConstant] = 0.9 // ??
      * [breakingForce] = 300 // ??
      * [breakingTorque] = 300 // ??
      * [fuelCrossFeed] = True
  * [ModuleCommand]
    * added
      * [Hibernation]
      * [defaultControlPointDisplayName]
      * [CONTROLPOINT] reverse
    * changed [ElectricCharge] from 0.0001 to 0.005
  * [ModuleReactionWheel]
    * [PitchTorque] now 40 was 30
    * [YawTorque] now 40 was 30
    * [RollTorque] now 40 was 30
    * [ElectricCharge] rate now 1.0, was 2.4 vs 2.7 of mk3Cockpit
  * Added:
    * [ModuleDataTransmitter]
      * internal
    * [ModuleKerbNetAccess]
      * Biome
      * Terrain
      * FoV: 5-90
      * Detection %: 1.0
    * [ModuleProbeControlPoint]
      * [minimumCrew] = 2
      * [multiHop] = True
    * [crewReport]
      * [usageReqMaskInternal] = 5
      * [usageReqMaskExternal] = -1
  * asset move
  * lint pass
  * light pass
  * formatting pass
  * localization pass
    * [crewReport]
    * [ModuleReactionWheel]
    * [ModuleScienceContainer]
    * [ModuleKerbNetAccess]
  * drag cubes
  * [ModuleInventoryPart] pass
    * [InventorySlots] = 10
    * [packedVolumeLimit] = 1200
* [JoolianSystems.cfg]
  * Control
  * [ModuleReactionWheel]
    * [ElectricCharge] rate now 2.25, was 1
    * [SASServiceLevel] now 3, was 0
  * asset move
  * lint pass
  * light pass
  * formatting pass
  * localization pass
  * drag cubes
  * [ModuleCargoPart] pass
    * [packedVolume] = -1

### Add Compatibility Patches

* MechJeb
* Kerbal Engineer
* kOS compatibility
* closes #58 - [Request]: MechJeb compatibility
* closes #57 - [Request]: Kerbal Engineer compatibility
* closes #56 - [Request]: kOS compatibility

### Update

* lint and reorganize
* updated pointer in model.mu from .dds/.tga/.png --> .dds
* rename part.cfg --> name
* rename model.mu --> `name.mu`
* moved .mu and .dds to Assets\
* mesh --> model
* Compatibility Patches
  * move TweakScale into separate compatibility patch
  * move RemoteTech into separate compatibility patch
  * move Snacks into separate compatibility patch
  * move UNK life support mod into separate compatibility patch
* [maxTemp] = 2000 from 2500
* [crashTolerance] = 6 from 12

### Add

* [tags]
* indent

### Part Thumbnail Images

* @thumbs list 
  * [x] [KAL.cfg]
  * [x] [JoolianBoomTank1.cfg]
  * [x] [JoolianBoomTank2.cfg]
  * [x] [JoolianBoomTank3.cfg]
  * [x] [JoolianCommBox.cfg]
  * [x] [JoolianCommTower.cfg]
  * [x] [JoolianEngine.cfg]
  * [x] [JoolianMainTank.cfg]
  * [x] [JoolianMonolith.cfg]
  * [x] [JoolianPod.cfg]
  * [x] [JoolianSystems.cfg]
* create docs/PartInvoice.md
* closes #55 - Part Thumbnail Images

### Patch linting and file maintenance

* minor housekeeping  
* patch dusting (mostly removing construction dust (comments)) 

### Status

* closes #2 - Release 0.8.9.9-adoption
* closes #3 - Adoption - social media
* closes #4 - Adoption Legal MumboJumbo
* closes #5 - Adoption Documentation
* closes #6 - Previous Releases
* closes #42 - Update Joolian Discovery (JOOL)
* closes #41 - Adoption - GitHub
* closes #25 -   Localization - English (United States) <en-us.cfg>
* closes #44 -  KAL.cfg
* closes #45 -  JoolianBoomTank2.cfg
* closes #46 -  JoolianBoomTank3.cfg
* closes #47 -  JoolianCommBox.cfg
* closes #48 -  JoolianCommTower.cfg
* closes #49 -  JoolianEngine.cfg
* closes #50 -  JoolianMainTank.cfg
* closes #51 -  JoolianMonolith.cfg
* closes #52 -  JoolianPod.cfg
* closes #53 -  Part Localization
* closes #54 -  JoolianBoomTank1.cfg
* closes #55 -  Part Thumbnail Images
* updates #24 -   Localization - Master

## Version 0.8.9.9 - for KSP 1.12.3 [17-Feb-2022]

* #43 - upstream from master - contributed by zer0Kerbal

## 0.8 (2015-08-14) - Tweaks

* Added Community Tech Tree support, moving parts to more advanced tech nodes.
* Added a radially-attachable KAL-9999 probe core, using existing art assets.

## 0.7 (2015-08-11) - Monolith tweaks

* Monolith scaled up 85% to give it dimensions close to the TMA-1 monolith from 2001.
* Monolith given a probe core, small reaction wheel, battery, internal generator.
* Monolith classified as a "Space Object" instead of debris.
* Monolith mass drasitcally reduced, to give it air-density, as mentioned in the 2010 book.
* Monolith texture problem fixed. Should be black again.
* Monolith now has top and bottom stack nodes, in addition to its surface attachment node.

## 0.6 (2015-05-01) - KSP 1.0.1 corrections

* Adjusted engine heat & thrust for KSP 1.0.1 compatability.
* Converted textures to DDS format.

## 0.5 (2015-04-30) - Beta Release

* Added more advanced SAS functions to the command pod
* KSP 1.0 compatability updates
* Re-assigned tech-tree locations.
* Now uses LiquidFuel instead of NuclearPropellant.

## 0.4 (2014-10-30) - Beta Release

* Tiny bit more progress on IVA
* Fixed IVA seat orientations
* Slightly brightened exterior textures.
* Switched textures back to MBM format for best performance and memory usage.

## 0.3 (2014-10-07) - Beta Release

* Fixed texture problem in the neck-adapter part.

## 0.2 (2014-10-07) - Beta Release

* Added a starter IVA (work in progress)
* Changed version file to not be as picky about KSP version

## 0.1 (2014-10-03) - Inital Beta Test
