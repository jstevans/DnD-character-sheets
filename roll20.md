# Helpful macros for Roll20
Here are some awesome examples of macros for Roll20. Below are all examples of ones that you might use for a Level 5 Bard from 5E.

## Attribute modifiers

### Strength
```
2
```

### Dexterity
```
3
```

### Constitution
```
3
```

### Intelligence
```
1
```

### Wisdom
```
0
```

### Charisma
```
4
```

## Traits

### Proficiency Bonus
```
3
```

### Jack of all Trades
```
floor(#prof_bonus / 2)
```

## Skill Checks

### Acrobatics
```
**Acrobatics check**
/roll d20 + #dex_mod + #jack_of_all_trades
```

### Animal Handling
```
**Animal handling check**
/roll d20 + #wis_mod + #jack_of_all_trades
```

### Arcana
```
**Arcana check**
/roll d20 + #int_mod + #jack_of_all_trades
```

### Athletics
```
**Athletics check**
/roll d20 + #str_mod + #jack_of_all_trades
```

### Deception
```
**Deception check**
/roll d20 + #chr_mod + #prof_bonus
```

### History
```
**History check**
/roll d20 + #int_mod + #prof_bonus
```

### Insight
```
**Insight check**
/roll d20 + #wis_mod + #prof_bonus
```

### Intimidation
```
**Intimidation check**
/roll d20 + #chr_mod + #jack_of_all_trades
```

### Investigation
```
**Investigation check**
/roll d20 + #int_mod + #jack_of_all_trades
```

### Medicine
```
**Medicine check**
/roll d20 + #wis_mod + #jack_of_all_trades
```

### Nature
```
**Nature check**
/roll d20 + #int_mod + #jack_of_all_trades
```

### Perception
```
**Perception check**
/roll d20 + #wis_mod + #prof_bonus
```

### Performance
```
**Performance check**
/roll d20 + #chr_mod + #jack_of_all_trades
```

### Persuasion
```
**Persuasion check**
/roll d20 + #chr_mod + #prof_bonus
```

### Religion
```
**Religion check**
/roll d20 + #int_mod + #jack_of_all_trades
```

### Sleight of Hand
```
**Sleight of hand check**
/roll d20 + #dex_mod + #prof_bonus
```

### Stealth
```
**Stealth check**
/roll d20 + #dex_mod + #jack_of_all_trades
```

### Survival
```
**Survival check**
/roll d20 + #wis_mod + #prof_bonus
```

## Spells

### Save DC
```
**Spell save DC**
/roll 8 + #prof_bonus + #chr_mod
```

### Cure light wounds
```
/roll ?{Cast Cure Wounds at what level?}d8 + #spell_mod
```

### Shatter
```
**Casting shatter**
/roll (?{Casted at level} + 1)d8

*Make targets make a constitution saving throw*
#spell_save_dc
```

### Thunder Wave
```
**Casting Thunder Wave**
/roll (?{Casted at level} + 1)d8

*Make targets make a constitution saving throw*
#spell_save_dc
```

## Saving throws

### Strength
```
**Strength saving throw**
/roll d20 + #str_mod + #jack_of_all_trades
```

### Dexterity
```
**Dexterity saving throw**
/roll d20 + #dex_mod + #prof_bonus
```

### Constitution
```
**Constitution saving throw**
/roll d20 + #const_mod + #jack_of_all_trades
```

### Intelligence
```
**Intelligence saving throw**
/roll d20 + #int_mod + #jack_of_all_trades
```

### Wisdom
```
**Wisdom saving throw**
/roll d20 + #wis_mod + #jack_of_all_trades
```

### Charisma
```
**Charisma saving throw**
/roll d20 + #chr_mod + #jack_of_all_trades
```

## Misc.

### Initiative
```
**Initiative**
/roll d20 + #dex_mod + #jack_of_all_trades
```

### Hit Die
```
**Taking a hit die for points of health**
/roll d8 + #const_mod + #jack_of_all_trades
```

### Healing Potions
This macro prompts the user what kind of cure wounds potion that would like to use, and then rolls the appropriate die.

```
?{Health Potion|
   Potion of Healing, **Potion of Healing** I regain [[2d4+2]] HP. |
   Greater Potion of Healing, **Greater Potion of Healing** I regain [[4d4+4]] HP. |
   Superior Potion of Healing, **Superior Potion of Healing** I regain [[8d4+8]] HP.
}
```
