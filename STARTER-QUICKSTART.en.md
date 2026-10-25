# Time & Seasons Starter — Quick start

1. Back up your project. Extract Addon Only into it: the only installed folder is addons/rpg_time. In Project Settings > Plugins enable Fableweld Time & Seasons Starter. Install one edition at a time.
2. Choose your language in the Time Starter dock. Clock: set the starting day/time, pace, pause and HUD options. Periods: edit and apply daily periods. Lighting: choose midnight/noon tint and ambient brightness, then Apply lighting.
3. Files: choose a profile location outside addons, then Save profile. Choose a new scene location outside addons. Create a 2D or 3D rig, or a playable 2D test scene. Add the saved rig to your world, or open the test scene and press F6.
4. Rules: name an availability rule, choose hours and seasons, then Apply and save the profile. The next-day scan samples every 15 minutes and may miss shorter conflicts. Conditions do not create shops or move NPCs.
5. Preview is isolated: save edits, reset it and try advancing or sleeping without changing your game. Language switching preserves unsaved values and customer names.
6. Optional Lumen Vale: extract its separate editable project into a new folder, import project.godot and press F5. Choose any of the seven languages; dialogue, signs and help follow it. Save clock and Restore clock demonstrate clock persistence only. Godot 4.7.2 Windows x64 is verified; other targets are unverified.

Updates: keep profiles, generated scenes and your code outside addons. Back up, disable the plugin, replace only addons/rpg_time, then re-enable. Convert a COPY of a Lite profile and preserve the original. Inspect .writing and .previous recovery files before retrying a failed save. Never overwrite your project's project.godot with the example's.

Addon Only is required. Both example downloads are optional. Full commercial source is included for private use; do not publish paid source. MIT core rights are unchanged. See LICENSE and LICENSE-COMPONENTS.txt. No weather, growth, custom calendar, NPC pathfinding, inventory, quests or whole-game saves are included. Support: fableweldlabs@gmail.com. Translations are AI-assisted and have not received independent native-speaker review.


The generated rig now includes a glossy reusable clock HUD, matching sleep control and a language selector. The selector translates built-in HUD text, interaction prompts and generated instructions without changing your game’s TranslationServer or custom names. For a custom HUD, use its language_code field or set_language("ja"). FWHUDStyle controls colors, font, padding, corners and clock size; the clock caches its appearance instead of rebuilding it on every tick. Existing custom sleep captions are preserved. Lumen Vale uses this actual reusable HUD, not a separate imitation.
