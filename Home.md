# MarrowSDK
Welcome to the MarrowSDK Wiki.  This is a public resource containing usage documentation for the MarrowSDK.

## Creating Marrow Content
- [Requirements](#requirements)
- [Project Setup](ProjectSetup.md)
- [Getting Started](#getting-started)
- [Creating a Pallet / Crates / Datacards](PalletsAndCrates.md)
  - [Spawnable Crate](Spawnables.md) - Spawn vanilla Bonelab items with the Bonelab Spawnable Pallet, spawn custom items into levels
  - [Avatar Crate](Avatars.md) - Create and play as a custom avatar
  - [Level Crate](Levels.md) - Design a custom Bonelab level
  - [Bone Tag Data Card](BoneTags.md) - Digital data used to reference the Player and other items, used to organize crates, etc.
  - [Mono Disc Data Card](MonoDiscs.md) - Reference digital audio data
- [Zones](Zones.md)
  - [Zone Links](ZoneLinks.md)
  - [Zone Events](ZoneEvents.md)
  - [Zone Load Level](ZoneLoadLevel.md)
- [ZoneLinkItems](ZoneLinkItems.md)
  - [Zone Music](ZoneMusic.md)
  - [Zone Ambience](ZoneAmbience.md)
- [Pallet Packing / Mod Installation](BuildPallet.md)
- [Mod Repositories](ModRepositories.md)
- [Developer Mode](DeveloperMode.md)
- [UltEvents](UltEvents.md)
- [Sharing Packed Content](SharingPackedContent.md)


Project Setup
---
Watch the step-by-step <b>MarrowSDK [Project Setup Guide](https://www.youtube.com/watch?v=U5jynJcDjvo)</b>, the <b>[Getting Started Guide](https://www.youtube.com/watch?v=M4B0TOG-b94)</b> on YouTube or follow the written <b>[Project Setup](ProjectSetup.md)</b> guide.


Getting Started
---

- On first launch, until you've created a Pallet, the editor will display a <i>Getting Started</i> window that will guide you through ensuring the SDK has <i>automatically</i> detected your game installation folder.  If not, the Game Install Locator will provide several options to find it.

![gettingstarted](./Images/UnityProjectModules/getting_started.png)

- Setting your game install will add the External BONELAB Content Pallet, which gives you access to all Bonelab vanilla content, like spawnables, avatars, the full game soundtrack and several ambient sounds that can be used when making your own content.

![assetwarehouse](./Images/UnityProjectModules/asset_warehouse.png)

- Use the Asset Warehouse button in the upper left of the Unity window to display the Asset Warehouse whenever you need it. 

- Create a Working Pallet, select it in the Asset Warehouse and add a new Level Crate.
- The Default Marrow Scene will create a basic template that includes the essential components of a level, so you can focus being creative!

