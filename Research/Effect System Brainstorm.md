
# What is an effect system
Generally, an effect system is an API for game state to alter stats of an entity.
- Taking damage can be an effect

# Potential Issues
- Orphaned Effects
	Effects must have something to remove them, or else they will be permanent. Dying while inside a slow AOE can cause you to stay slowed down forever after respawn.
- Order of operations
	Upgrades need to be applied in a specific order so that the same configuration always results in the same stats
- Effect copies
	When an effect is not intended to be stackable, such as slowness, we must ensure that we do not apply duplicates of that effect.
- Corrupt Immunity
	If you are already on fire, an effect that says 'be immune to fire', when it is applied may not be programmed to first check if you are already on fire.

# Potential Features
- Proc Chain
	Effects that proc from events such as killing an enemy may cascade uncontrollably. For instance an effect that says 'when you kill an enemy, they explode' can kill another enemy and continue the explosions
- Proc Drop
	Effects that proc from events such as killing an enemy cannot cascade uncontrollably. For instance we would change the definition of the effect to, 'when you kill an enemy with your primary weapon directly, they explode'
- Stackable Effects
	Effects can be configured to be stackable.


# Types of Effects
- Skill tree effects
	Stat bonuses, level ups
	Passive effects, conditional passive effects
- Gear effects
	Stat bonuses
- Gear set bonuses
- Area Effects
	Tar traps
	Brimstone
	Poison smoke
- Limited Time Effects
	Potions, enchantments, burning, poisoned

### All Effects Have in Common
- They must all be kept track of, they must all be able to be removed

# Deconstruction of Stats
There really is two different states of stats
- Base Stats
	The default starting stats of all characters.
- 
- Enhanced Stats
