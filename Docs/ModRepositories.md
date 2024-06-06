## Q: What is a Mod Repository?

A: A mod repository is a name, a description, and a list of mods.

## Q: What is a Mod Listing?

A: An entry in the mod list, including its name, description, author, and a lookup-table of Mod Targets from their platform identifier ("pc" or "oculus-quest").

> :pencil: A Mod Listing holds metadata on a mod, so it shares many similarities with the Pallet data structure in the mod SDK, but it also contains URLs pointing to the pallet manifest and a thumbnail image for display.

## Q: How do I make a Mod Repository?

A: The SDK includes a basic editor which can be found in the menu "Stress Level Zero/Marrow/Mod Repository Editor".

> :pencil: Technically advanced users may be interested in creating their own tools to produce compatible Mod Repository or Pallet files. Our implementation of the serialization format can be found here: https://github.com/StressLevelZero/SLZ.Serialize

## Q: How do I add a Mod Repository?

A: Repositories are loaded from `repositories.txt` in the game directory, one URL per line. You can update them by adding to this file, or, if you are in developer mode, via the WebSocket console.

### File Method

- On PC, this file is located at `%appdata%\..\LocalLow\Stress Level Zero\BONELAB\repositories.txt`.
- On Quest, this file is located at `Internal shared storage\Android\data\com.StressLevelZero.BONELAB\files\repositories.txt`. If you have a PC, you can connect your Quest to it, accept the permission dialog, and upload your `repositories.txt` there.

### Websocket Console Method

> :warning: This is a bit technical, and intended to streamline developer workflows and involves enabling a server on your device.
>
> :warning: Your Quest (and BONELAB) may need to be foregrounded to register the repository add.

1. Enable Developer Mode (see below).
2. Connect to your device (typically, `ws://127.0.0.1:50152/console` on your PC, or your headset's IP in place of `127.0.0.1` otherwise).
3. Send `repo.add http://example.com/path/to/your/repository.json` (with the URL replaced, obviously) to the WebSocket console.
4. Return to the main menu and reopen the mod menu to refresh your repositories.
5. Check that your repo is now listed in Mods -> Settings -> Repos.

## Q: What is Developer Mode?
A: Developer Mode is a flag to enable functionality used by the Marrow SDK to interface with BONELAB. It enables a local WebSocket server, against which text commands can be issued. Enabling Developer Mode does not connect to an external server.

Enabling Developer Mode can be toggled from menu in Mods -> Settings.