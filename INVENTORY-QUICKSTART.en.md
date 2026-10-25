# Inventory & Equipment — quick start

Inventory & Equipment 1.0.0. Godot 4.7.2, Windows x64. See the included license and component notices.

1. Preserve your project and saves. Copy `addons/fableweld_inventory` into your
   game. Compare versions and preserve customizations before replacing files.
   No clock or NPC addon is required.
2. Enable Fableweld Inventory & Equipment under Project Settings > Plugins.
   Choose the dock's language. This does not change the game's global locale.
3. Create items or add starter items. Edit them in the Inspector and validate the
   catalog. Save a `.tres` outside `addons`. Load an existing destination before
   updating it; loading requires confirmation. Keep stable item IDs.
4. In the example project, open `demo/inventory_quick_start.tscn` and press F6.
   Its top language selector coordinates tabs and panels. Equip the starter
   blade, assign a potion to the hotbar, split a stack and transfer to the chest.
5. For your own scenes, bind panel `controller_path` values to a
   `FWSlotInventoryController`. Grids that exchange items need the same catalog
   resource and nonempty `transfer_group`. Your game supplies item effects and
   base character stats.
6. Register slot controllers in `FWInventorySession.controllers` with stable save
   IDs and NodePaths. Bind `FWInventorySavePanel.session_path` to that session.
   Choose a distinct `user://...json` save path for each slot or world.
7. Save and load the inventory session. This includes registered bags, equipment
   and shortcuts; it does not save the whole game. The older checkpoint demo
   keeps data only until it closes. Preserve an existing `.fw-writing` file
   before retrying a blocked save. Concurrent writers are unsupported.
8. Upgrade a copy first. Keep authored catalogs, scenes and saves outside vendor
   folders. Before removal, replace dependent references, disable the plugin,
   then remove its addon folder. Deleting scripts while referenced breaks scenes.

Language changes preserve IDs and custom text. Example category/stat translation
is opt-in through `translate_example_names`; it is off by default on reusable
views. Unknown custom text falls back unchanged. Native-speaker review, arbitrary
project compatibility and final exported-package acceptance are not claimed.
