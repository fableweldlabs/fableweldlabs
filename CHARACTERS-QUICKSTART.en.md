# Characters, Stats & Abilities — Quick start

Verified: Godot 4.7.2 Windows.


1. Copy `addons/fableweld_characters` into your Godot project's `addons/` folder.
2. Enable **Fableweld Characters, Stats & Abilities** in **Project Settings → Plugins**.
3. Open the **Fableweld Characters** dock, add classes before characters, then add abilities and status effects as needed.
4. Enter a project-relative catalog path such as `res://data/characters.tres`, then choose **Save catalog**. The dock will not save a catalog with unresolved references or invalid IDs.
5. Use **Open catalog** only after entering its path. An unreadable, unrelated, or invalid resource leaves the active catalog unchanged.

The dock and quick-start support English, Spanish, Brazilian Portuguese, Simplified Chinese, Japanese, French, and German. Unknown built-in locales fall back to English. Resource identifiers, authored display names, and customer content remain yours; this add-on does not translate or rewrite them.

Use the language selector at the top of the dock. **Add Lumen starter** creates a localized example in an empty catalog; it does not overwrite existing work. Select an entry to edit it in Godot's Inspector. **Undo last change** reverses catalog creation/open/starter actions; Inspector property edits use Godot's own undo history. Tab moves through the dock controls, and a short dock scrolls to follow focus. The optional shared-world example opens the same runtime summary through its Characters button.


Keep catalogs outside the addon folder and preserve IDs. Your game owns save storage, migration decisions and combat execution.

## Updating and saved data

Catalogs are ordinary Godot `.tres` resources. Keep them outside the replaceable `addons/fableweld_characters` folder, and back up project data before replacing the add-on. Version 1.0.0 uses version-1 party save dictionaries. Treat a failed `from_dictionary()` result as incompatible or malformed data and keep the prior in-memory state; it is intentionally atomic.

The optional `demo/character_quick_start.tscn` is an editable/playable sample, while `tests/` is package-validation material. Neither is required by your shipped game.
