# Open and use Calendar & Growth Pro

This guide targets Calendar & Growth Pro review builds. Commercial license wording and the $29.99 price are approved for packaging. Publication remains separately authorized.

## Choose your download

The required addon contains addons/rpg_time and no root project.godot. Copy only that folder into your existing project as described below. Do not import the demo folder in Project Manager.

The separate optional Lumen Vale editable example contains project.godot at its root. Extract it into a new folder, import that file, wait for scanning, then press F5. The village opens; Calendar shows the real Pro calendar, two growth durations and harvest/snapshot controls. Existing internal workshop projects are engineering fixtures, not the same download.

The optional Windows x64 demo runs without Godot installed: extract the entire ZIP, keep Lumen-Vale-Pro.exe and its matching PCK together, then run the executable. Its clock save controls persist time; garden snapshots are in-memory demonstrations.

## Add it to your own game

1. Close your game project in Godot.
2. Copy only the package's `addons/rpg_time` folder into your game's `addons` folder.
3. Open your game, let import finish, then enable RPG Time & Seasons under Project > Project Settings > Plugins.
4. Open the Time & Seasons dock. On Setup, configure and Apply the starting settings.
5. Save the profile outside addons, for example `res://time_seasons/world.tres`.
6. Create a clock scene at a new path outside addons and add that scene to your world. The Paid lighting rig option includes a linked clock, HUD and sleep button; avoid adding a second authoritative clock accidentally.

Do not copy the demo's project.godot over your game's project.godot. Lite and Paid use the same addon folder and class names: replace an edition using docs/INSTALL-UPGRADE.md, never install both alongside one another.

## What each screen does

- Godot dock: configure reusable profiles and generate clock/rig scenes.
- Dock Preview: simulate the profile in isolation. It does not run or change your game world or write game saves.
- Runnable showcase: try the reusable UI and example workflows.
- Your game: receives time behavior through the generated clock and documented connections. Saving time is not the same as saving your entire game.

## If something looks wrong

| Symptom | Next step |
| --- | --- |
| Import dialog shows an empty demo folder | Go up to the package root and select project.godot. |
| The editor shows an empty scene | Press F5 to run the configured project; an empty editor tab is not the demo. |
| An older interface opens | Check the project's full path in Project Manager and import the reviewed project path above. |
| Time & Seasons dock is missing | Wait for import, then check that the plugin is enabled. Inspect the Output/Debugger errors if enabling fails. |
| The clock does not advance | Check whether it is paused and whether its day duration is zero. The showcase starts paused intentionally. |
| Generated clock is not affecting the world | Confirm the generated scene is instanced in the running world. Creating its file does not add it automatically. |
| A 3D lighting rig has no visible world | It requires your world's camera and geometry. The supplied 3D example provides those. |

Tested support target: Godot 4.7.2 on Windows x64. The editable example has a root manifest; addon and Windows package hashes are recorded in their engineering handoff. See docs/RELEASE-GATES.md for engineering and owner acceptance boundaries.
## Upgrade from Starter

Close Godot and replace only addons/rpg_time. Keep authored profiles, scenes and saves outside that folder. Pro accepts compatible advanced Paid v2 JSON clock saves and writes v3 JSON saves. Focused Starter binary saves require the explicit conversion described in Focused-Starter-Upgrade.txt. Keep a copy of your old saves: Starter cannot load the new v3 format. See INSTALL-UPGRADE.md and CLOCK-PRECISION.md.


## Atmosphere and local development tools

On Lighting, choose and explicitly apply an atmosphere preset; effect switches preserve manually edited curves. Save the profile and generate a new rig. In the optional Lumen Vale example, open Calendar and scroll to Atmosphere. No atmosphere preserves the baseline. Preview presets and fog, advance time and restore registered state; the saved profile remains unchanged. Removing the preview restores baseline lighting.

Setup can include local development tools in newly generated rigs. This choice is off by default and links the bridge automatically when selected. The discovery bridge stays disabled in an actual release executable. See DEVELOPMENT-BRIDGE.md for the local consumer contract; it has no network transport or competitor protocol compatibility claim.
