# JumpLoot Plugin Configuration Guide

## Overview

The JumpLoot plugin for Rust enhances gameplay by allowing players to receive loot when they jump. This guide provides detailed instructions on configuring the items that can be dropped using the `JumpLoot` plugin.

## Configuration File

The configuration for the items is located within the `oxide/config/JumpLoot.json` file. This section focuses on how to customize the `Items` array.

## Item Configuration

The `Items` array in the configuration file specifies the items that players can receive as loot when they jump. Each item in the array has the following attributes:

### Name (`string`)
- **Description**: The internal name of the item.
- **Example**: `"Name": "hat.wolf"`

### MinAmount (`int`)
- **Description**: The minimum amount of this item that can be dropped.
- **Example**: `"MinAmount": 1`

### MaxAmount (`int`)
- **Description**: The maximum amount of this item that can be dropped.
- **Example**: `"MaxAmount": 3`

## Example Configuration

Here is an example configuration for the `Items` array:

```json
{
  "Items": [
    {
      "Name": "hat.wolf",
      "MinAmount": 1,
      "MaxAmount": 3
    },
    {
      "Name": "pistol.semiauto",
      "MinAmount": 1,
      "MaxAmount": 1
    },
    {
      "Name": "ammo.pistol",
      "MinAmount": 10,
      "MaxAmount": 50
    },
    {
      "Name": "medkit",
      "MinAmount": 1,
      "MaxAmount": 2
    }
  ]
}

For further assistance or to report issues, please visit the JumpLoot Plugin page.
