# RRR Core

- Core library required by all of my other mods.

## Setup

Extract the zip file to your `Valheim\BepInEx` folder. Config files should end up in `Valheim\BepInEx\config`, everything else should end up in `Valheim\BepInEx\plugins`. Config files will also be generated automatically if missing.

## Help!

If you need further assistance, feel free to bug me in the Valheim Modding Discord at https://discord.gg/RBq2mzeu4z


## Changelog

### 2.12
- To Character, added bStaggerWhenBlocked.
- To CustomAttack, added fAIAttackRange, fAIAttackRangeMin, fAIAttackMaxAngle, bBlockable, bDodgeable, bForceAttackChainZero, bUseCharacterFacing, fAttackRange, fAttackHeight, fAttackRayWidth.

### 2.11
- Updated for Valheim 207.20. IronGate removed "NoiseRangeScale" from MonsterAI so that field is now deprecated and will not do anything for custom monsters.

### 2.10 
- Updated for Valheim H&H. IronGate removed "ConsumeHeal" from MonsterAI so that field is now deprecated and will not do anything for custom monsters.

### 2.9
- Updated ServerSync, which should hopefully fix the sync issues some users have on dedicated servers.
- Add sAITargetType and sAttackStatusEffect to custom attack definitions.