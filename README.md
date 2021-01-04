# BraindanceProtocol

A collection of LUA scripts to modify your Cyberpunk 2077 experience

## Available Tweaks

- Prevent _V_ from being knocked over by NPC vehicles
- Disable AutoSaves
- Increase AutoSaves increments
- Decrease AutoSaves increments
- Activate GodMode
- Give Player Johnny's Items
- Give Player lots of money
- Set Player to Max Level, Streetcred, Perk level, and Attribute level
- Give Player all Legendary recipies
- Make all equipped items Legendary with max stats
- Give player all ownable vehicles

## Requirements

Latest version of [CyberEngineTweaks](https://github.com/yamashi/CyberEngineTweaks#usage-and-configuration)

## Installation

Drop `mods` folder into `bin\x64\plugins\cyber_engine_tweaks\`

## Using In-Game

You must call the GetMod command to register commands for the mod.

```lua
BD = GetMod("braindance_protocol")
```

Following that, all below commands will be available.

## Manually Activate Protocols

```lua
-- Cheats
BD.Cheats.Player.MaxOut() -- Max Level, Attributes, Skill Points, Money,
BD.Cheats.Player.GodMode() -- Gives you pseudo "god mode". Permanent to your SaveFile
BD.Cheats.Player.AddMoney(amount) -- Gives the player specified amount of money. If no amount is specified, gives you 999999 money.
BD.Cheats.Crafting.AddAll() -- Add all Recipes & Materials
BD.Cheats.Johnny.AddItems() -- Adds Johnny's Legendary Items
BD.Cheats.Legend.Create() -- Makes all equipped items legendary with max stats.

-- Saves
BD.Saves.DisableAutosave() -- Disables auto saving.
BD.Saves.DecreaseAutosaves() -- Decreases time between auto saves.
BD.Saves.IncreaseAutosaves() -- Increases time between auto saves.

-- Vehicles
BD.Vehicles.GetAll() -- Grants you all ownable player vehicles.
```
