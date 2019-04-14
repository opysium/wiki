---
title: ForceClassSelection
description: Forces a player to go back to class selection.
tags: []
---

# ForceClassSelection

<TagLinks />

## Description

Forces a player to go back to class selection.

| Name     | Description                                 |
| -------- | ------------------------------------------- |
| playerid | The player to send back to class selection. |

## Returns

This function does not return any specific values.

## Examples

```c
if(!strcmp(cmdtext, "/class", true))
{
    ForceClassSelection(playerid);
    TogglePlayerSpectating(playerid, true);
    TogglePlayerSpectating(playerid, false);
    return 1;
}
```

## Notes

::: warning

This function does not perform a state change to PLAYER_STATE_WASTED when combined with TogglePlayerSpectating (see example below), as is listed here.

:::

## Related Functions

- AddPlayerClass: Add a class.
- SetPlayerSkin: Set a player's skin.
- GetPlayerSkin: Get a player's current skin.
- OnPlayerRequestClass: Called when a player changes class at class selection.