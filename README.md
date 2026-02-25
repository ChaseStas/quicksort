# Quicksort

## Features
* **Lightweight item sorting.** Keep your workshop organized quickly and easily.
* **Vanilla-friendly**.         Does not add any new blocks to your server.
* **Serverside-only**.          Does not have to be installed on clients.
* **Fully customizable.**       Define your own quicksort chest types.

## Usage
* Place an emerald or diamond block in the center of your storage area.
* Create a **Quicksorter** by putting regular chest on top of that block.
* Items placed in the Quicksorter will automatically be distributed to nearby chests that contain matching items.

![](https://github.com/pcal43/quicksort/raw/main/etc/quicksort-demo2.gif)


## Fine Points
* The Quicksorter must have a clear line-of-sight to the receiving chests (unless `rangeThroughWalls` is enabled in config)
* The receiving chests must be within a cube-shaped area centered on the Quicksorter.
* The Quicksorter's range depends on the type of block used:
  * Emerald: 5 blocks away
  * Diamond: 10 blocks away
* Items are transferred regardless of whether the item appears to not make it to the chest

## Build & Run

**Requirements:** Java 17+ (Java 21 recommended for Minecraft 1.21+)

**Compile:**
```bash
./gradlew build
```

The mod JAR will be in `build/libs/` (e.g. `quicksort-0.21.1+1.21.11-prerelease.jar`).

**Install in Minecraft:**
1. Install [Fabric Loader](https://fabricmc.net/use/installer/) for your Minecraft version
2. Install [Fabric API](https://modrinth.com/mod/fabric-api) (required dependency)
3. Copy the built JAR into your Minecraft `mods/` folder
4. Launch Minecraft with the Fabric profile

**Development / Run in-game:**
```bash
./gradlew runServer   # Run a Minecraft server with the mod
./gradlew runClient   # Run a Minecraft client with the mod
```

## Configuration

To configure the mod, follow the instructions in the default config file:

https://github.com/pcal43/quicksort/blob/main/src/main/resources/quicksort-default-config.json5

**`rangeThroughWalls`** — When `true`, the Quicksorter will find and sort to all valid chests within `range` blocks, regardless of walls, blocks, or other obstacles. Useful when you want to sort within a radius (e.g. "around N blocks") without worrying about line-of-sight.

## Credits

#### Icon components courtesy of
* [Minecraft Toolbox - Minecraft Chest PNG](https://flyclipart.com/minecraft-toolbox-minecraft-chest-png-50783)
* [transparentpng.com](https://www.transparentpng.com/download/circle-vector-2_15270.html)
* [freesvg.org](https://freesvg.org/8-directions-arrows)

## Legal

This mod is published under the [MIT License](LICENSE).

You're free to include this mod in your modpack provided you attribute it to pcal.net.

## Questions?

If you have questions about this mod, please join the Discord server:

[https://discord.pcal.net](https://discord.pcal.net)

Comments have been disabled and I will **not** reply to private messages on Curseforge.