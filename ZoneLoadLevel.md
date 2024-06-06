# <img src="./Images/zone-icon.png" valign="middle" style="padding-bottom: 4px"> Zone Load Level

<img src="./Images/icon_marrow_video.png" valign="middle" style="margin: 0px 5px 5px 0px"/> <a href="https://www.youtube.com/watch?v=mckRH8cNSRU"><font size="5">Zone Events and Level Loading Tutorial Video</font></a> 

## Zones with Zone Load Level

<img src="./Images/Zones/zoneloadlevel_to_hub.png" width="400">

Zone Load Level triggers a level change when a valid activator (usually the player) enters the collider volume.  

- The Load Screen Level field specifies the "loading screen" area the player will see during the level loading process.  This is recommended to be a very visually simple, small, low-asset, walled-in area that prevents the player from falling.  It should display some form of loading progress status or a simple image or animation to convey the level load process.  The External BONELAB Core Pallet (available once your game install has been set in the Marrow SDK) includes the "Load Mod" and "Load Default" Level Crates for this purpose.

- The Level field accepts any Level Crate found in the Asset Warehouse.

<img src="./Images/Zones/zoneloadlevel_inspector.png" >