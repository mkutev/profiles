##Additional Credit:

Furok and Grim Age mod team created the original models and textures used in this mod, I just re-rigged the model and did some other tweaks for use in Valheim. Grim Age is a mod based on Warhammer Fantasy, and as such should be considered a Derivative Work to which Games Workshop holds copyright to. Games Workshop's copyright thus extends to the models and textures used in this mod.

GoldenJude for Blacksmith's Tools and significant rigging help

zarboz for some help with some rigging adjustments

blaxxun for ItemManager/ServerSync

##Description:

Adds Chaos Warrior Armor as a new standalone set of armor to the game. Armor names and descriptions are kept fairly vague and don't outright refer to anything from Warhammer lore, if that matters to you. 

Low-res texture version available in optional files on Nexus. 

Recipes can be viewed and adjusted in ReepusDeepusDelmeepus4902761.ChaosArmor.cfg.

(Low Res)
![](https://staticdelivery.nexusmods.com/mods/3667/images/1215/1215-1657432122-358647393.png)

(Default)
![](https://staticdelivery.nexusmods.com/mods/3667/images/1215/1215-1654743586-673230531.png)

##Full Equipment List

(T0, 4 quality levels)

Scrap breastplate (Prefab name T0ChaosPlateArmor)

Scrap helm (Prefab name T0ChaosPlateArmor)

Scrap greaves (Prefab name T0ChaosPlateLegs)

(T1, 4 quality levels)

Half plate harness (Prefab name T1ChaosPlateArmor)
  
Tusk plate helm (Prefab name T1ChaosPlateHelm)
  
Battered plate leggings (Prefab name T1ChaosPlateLegs)

(T2, 4 quality levels)

Three quarters plate harness (Prefab name T2ChaosPlateArmor)

Fanged plate helm (Prefab name T2ChaosPlateHelm)

Refurbished plate leggings (Prefab name T2ChaosPlateLegs)


(T3, 4 quality levels - only armor before V5)

Uncanny plate harness (Prefab name ChaosPlateArmorBody)

Uncanny plate helm (Prefab name ChaosPlateHelm)

Uncanny plate leggings (Prefab name ChaosPlateLegs)

(T4, 4 quality levels)

Stygian plate harness (Prefab name EliteChaosPlateArmor)

Abyssal plate helm (Prefab name EliteChaosPlateHelm)

Tenebrous plate helm (Prefab name ChaosPlateHelmAlt)

Umbral greaves (Prefab name EliteChaosPlateLegs)


##Changelog:

10.0.2
- reverted non-metal textures, were too sharp in 10.0.0

10.0.1
- added neck cover to bronze tier helm

10.0.0
- added early bronze tier set
	- updated default recipes for iron tier set to be crafted from bronze tier pieces
- upped brightness on all textures
- localization file should finally be read from the dll's directory

9.0.17
- updated serversync to version which should work with crossplay

9.0.16
- updated serversync

9.0.15
- reduced total movement penalty of T1 and T2 sets to that of T3 (-12%)
	- distributed penalty more evenly between chest and leg pieces
- slightly increased total movement penalty of T4 full set (-13%)
- updated serversync and itemmanager

9.0.14
- sealed up gaps in T4 chest piece between arms and breastplate

9.0.13
- added MS-paint-tier bodymat that doesn't black out the face

9.0.12
- removed blackout bodymat, did not realize it affected face as well
- re-rigged boots across all tiers
- made some minor visual adjustments to T2 and T3 boots to have some small distinction
- sealed up a small seam between the breastplate and right arm for T1 to T3 armors

9.0.11
- added blackout bodymat to chest armors as a fallback in case blacksmith's tools ever stops working

9.0.10
- rigging adjustments on all tiers
- now using zarboz's ShaderReplacer
- I am fucking exhausted

9.0.8
- fixed thumb rigging issue introduced in 9.0.7 for T1 to T3 armors

9.0.7
- visual adjustments to all tiers of armor
	- breastplates/lower body positions adjusted to fit more closely with player position and reduce clipping with capes
	- added redundant chainmail neck cover to all tiers of breastplates for players who forgo the helmet (no longer neckless)
	- replaced left arm plating on T2 and T3 armor models with T4 arm plating

9.0.6
- long overdue update to latest ServerSync and ItemManager versions

9.0.5
- changed armor shader

9.0.4
- added Localization support via YAML file in plugins folder
	- new language localizations can be added by following the format in the template sample included in the file

9.0.3
- reduced bloat in breastplate, slightly slimmer now
- extended right arm bracer/gauntlet to cover up some very visible rigging ugliness when in the 2h sledge pose
- hopefully moved fixed cfg from 9.0.2 to right folder this time

9.0.2
- fixed more fuckups
	- T3 helmet and legs still had 8 max quality, reduced down to 4 as intended
	- dumbass issues with T4 legs and alternate helmet default recipe caused NRE spam when selecting their recipes in-game

9.0.1
- fixed fuckup in recipe registration causing no recipes to be registered
- added default cfg to configs for anyone who already loaded in with borked cfg

9.0.0
- added new armor set port
	- upped saturation on existing armor textures as well to mesh better with new set
	- new armor is T4, requires Flametal and many other rare trophies to craft
	- extra edgy names and descriptions featuring words from at least 5 different thesaurus sources
		- I understand that Stygian has literary roots in an entirely different mythology, don't @ me
- shuffled around default tiers and armor stats
	- Uncanny set now requires Black Metal instead of Flametal
	- all armor sets now follow the vanilla 4 quality level standard
- Warped plate helm moved to T4 and renamed to Tenebrous plate helm
	- same armor level as T3 helm but has a damage type immunity as trade off with the other T4 helm

8.0.0
- removed JVL dependency, switched to blaxxun's ItemManager and ServerSync
	- stamina and health regen related bonus effects on final tier of armor have been removed
	- some config settings are no longer available - delete your old cfg and json files
- slightly reduced texture quality to slim down file size

7.1.0
- unload assetbundle after mod initialization, should no longer cause Unity crash on game exit

7.0.0
- added alternate final tier helm with mostly same stats as Uncanny plate helm
	- just an altered version of the mesh with a face grill attached
- translations moved from being hardcoded to a json file, side-loaded via Jotunn

6.0.5
- removed dependency on BoneReorder function from JVL/Blacksmith's Tools - model was re-rigged onto the correct armature

6.0.4
- plugin ver. still 6.0.2, version bump just for dependency updates
- adding Thunderstore version of Blacksmith's Tools as dependency

6.0.3
- plugin ver. still 6.0.2, version bump from before was purely for dependency string updates
- removed blacksmith's tools config files; body hiding configuration is handled in-code now
- fixed minor issue with easter egg Reepus/Deepus/Delmeepus set regarding damage modifiers list; set to empty instead of null
- removed equip message for final tier chaos armor, just a personal judgement call
- updated bepinex dependency version
- some minor tweaks to config options and upper limits

6.0.2
- just updating dependency versions to latest; verified basic functionality still works with H&H 

6.0.1
- minor tweak made to ensure armor renders properly in Vulkan (was previously translucent)

6.0.0
- moved recipe configuration to its own json file, ReepusDeepusDelmeepus4902761.ChaosArmor.recipes.json
- max quality of each tier of Chaos Armor made configurable through ReepusDeepusDelmeepus4902761.ChaosArmor.cfg
- reduced default max quality of tier 3 Chaos Armor to 7, since it is currently impossible to get to forge level 8
- bundled cfg file with this release to replace the old one and its outdated fields

5.0.2
- removed jump/run stamina use modifiers on chest entirely as they did not seem to be working as intended

5.0.1
- changed eye color of T1 and T2 helmets on a suggestion
  - T1 has blue eyes
  - T2 has green eyes
  - Final tier retains original red eyes
- fixed issue in high res textures where they were accidentally left with no filter

5.0.0
- added two lower tiers of stripped-down armor, beginning at bronze
- new crafting recipes requires beginning with the bronze tier armor and reforging it up to the final tier
- final tier upgrade/craft recipes adjusted slightly, but existing crafted sets from previous versions will remain at their quality level

4.0.2
- not an actual update, just adding a very important note about copyright in the description and readme
- actual file contents are the same as 4.0.1, the .dll version is also still 4.0.1 for network compatibility purposes

4.0.1
- added cold resist to chestpiece
- rebuilt assembly from new project yet again
- low res texture version available on Nexus, just overwrite ChaosArmor.dll with the .dll provided in that optional file; texture replacement should be client-side and the rest of the code is up-to-date with main file

4.0.0
- added frost resist to chestpiece
- added new config options
- rebuilt dll from new project, praying to god this stamps out any assembly loading issues; will retain loose assetbundle version on Nexus for some time in case not
- low res texture version available on Nexus, just overwrite ChaosArmor.dll with the .dll provided in that optional file; texture replacement should be client-side and the rest of the code is up-to-date with main file

3.0.2
- changed AssemblyTitle of compiled assembly, was using non-unique name previously

3.0.1
- changed to GetExecutingAssembly in code for loading assetbundle
- fixed minor bug from last version where status effects on chest and legs were not applying

3.0.0
- bumped major version for stricter compatibility enforcement (should've done so last update already tbh)
- changed code class name to hopefully fix assembly loading issues
- added icons for status effects

2.2.4
- added configuration file allowing for adjustment of crafting/upgrade amounts

2.2.3
- added rigging for fingers; still a little rough around the edges, but seems fine in most cases

2.2.2
- added normal and metallic maps for models
- small tweaks to recipe requirements
- made the eyes of helmet faintly emissive
- changed casing on in-game item names to be consistent with vanilla item names
- made some very minor rigging tweaks to the neck parts of model

2.2.1
- fixed bug where equipping chest piece would wipe out player model textures (face, skin, eyes etc.)

2.2.0
- adjusted recipe/upgrade amounts to be more varied
- small mesh adjustments:
  - covered up a small gap between the right arm and breastplate with filler material
  - positioned helmet further forward to closer match player character posture (no longer clips with head in character select screen)
- bunch of cool changes courtesy of zarboz
  - mesh rigging of body matches player posture much better now - unfortunately not enough to prevent clipping, hence Blacksmith's tools remains a requirements
  - on-equip status effects with a special cheesy message for each armor piece, see Gear Stats Breakdown for more details

2.0.1:
- assetbundle now in .dll as an embedded resource, should work when running from mod managers now