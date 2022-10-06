# Useful Trophies

Has this ever happened to you?

Chests filling up with trophies you don't know what to do with,
Your bonfire is already filled to the brim with "sacrifices" to your favorite god,
You are running out of places to store these heads!

All the while, you wish your stats were a bit higher...

Well look no further!

---

This mod gives you the ability to consume the heads of your enemies!
Each Trophy consumed will increase a random skill by how rare the trophy is!
The amount varies by trophy head, and can be configured.

Boss Trophies now also have an extended use.
When a boss trophy is consumed, your current guardian power cooldown is reset and made ready again.
Or you can enable an alternative in the config to have the specific Boss Trophy just give you their buff
(eg. Eikthyr Trophies would give you the Eikthyr buff)

You could even enable both if you want, I'm not going to stop you.


## Installation (manual)

If you are installing this manually, do the following

1. Extract the archive into a folder. **Do not extract into the game folder.**
2. Move the contents of `plugins` folder into `<GameDirectory>\BepInEx\plugins`.
3. Run the game.

### Configuration

EXPScaling: You can set the amount of exp each trophy will give you (up to a max of 1 level at a time)
A 1 here is equivalent to one club/axe swing or 1 second of running.

TrophyEXPMultiplier: Global modifier for exp gained from each trophy 

BossConsumption: This is on by default, however you may consider disabling it if you don't want to be careless when handing in a boss trophy to the alter.
(It will still work, just don't accidently consume the trophy by accident)

BossesResetGuardianCooldown: On by default, resets your guardian CD when any boss trophy is consumed.

BossesApplyGuardianPower: Off by default, applies boss specific buffs instead of resetting your CD. (may be harder to farm specific buffs)

```
## Settings file was created by plugin Useful Trophies Mod v1.1.0
## Plugin GUID: gg.khairex.usefultrophies

[BossConsumption]

# Setting type: Boolean
# Default value: true
CanConsumeBosses = true

## This will reset your CURRENT guardian cooldown when consuming ANY boss trophy
## You should probably use either this OR ApplyGuardianPower and not both
# Setting type: Boolean
# Default value: true
BossesResetGuardianCooldown = true

## This will give you the guardian buff when consuming a guardian head.
## eg. Eikthyr Trophies will give you the Eikthyr Buff
## You should probably use either this OR ResetGuardianCooldown and not both
# Setting type: Boolean
# Default value: false
BossesApplyGuardianPower = false

[ExpScaling]

## Multiplier for all trophies
## 0.5 would half all incoming trophy exp
# Setting type: Single
# Default value: 1
TrophyEXPMultiplier = 1

# Setting type: Single
# Default value: 4
deer = 4

# Setting type: Single
# Default value: 4
boar = 4

# Setting type: Single
# Default value: 5
neck = 5

# Setting type: Single
# Default value: 5
greydwarf = 5

# Setting type: Single
# Default value: 10
greydwarfbrute = 10

# Setting type: Single
# Default value: 10
greydwarfshaman = 10

# Setting type: Single
# Default value: 6
skeleton = 6

# Setting type: Single
# Default value: 15
skeletonpoison = 15

# Setting type: Single
# Default value: 15
troll = 15

# Setting type: Single
# Default value: 10
surtling = 10

# Setting type: Single
# Default value: 7
leech = 7

# Setting type: Single
# Default value: 8
draugr = 8

# Setting type: Single
# Default value: 15
draugrelite = 15

# Setting type: Single
# Default value: 12
blob = 12

# Setting type: Single
# Default value: 30
wraith = 30

# Setting type: Single
# Default value: 12
wolf = 12

# Setting type: Single
# Default value: 35
fenring = 35

# Setting type: Single
# Default value: 12
hatchling = 12

# Setting type: Single
# Default value: 25
sgolem = 25

# Setting type: Single
# Default value: 15
goblin = 15

# Setting type: Single
# Default value: 30
goblinbrute = 30

# Setting type: Single
# Default value: 20
goblinshaman = 20

# Setting type: Single
# Default value: 20
lox = 20

# Setting type: Single
# Default value: 20
deathsquito = 20

# Setting type: Single
# Default value: 60
serpent = 60

# Setting type: Single
# Default value: 25
eikthyr = 25

# Setting type: Single
# Default value: 35
elder = 35

# Setting type: Single
# Default value: 50
bonemass = 50

# Setting type: Single
# Default value: 50
dragonqueen = 50

# Setting type: Single
# Default value: 50
goblinking = 50
```