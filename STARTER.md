# Time & Seasons Starter

[Product and purchase](https://fableweld-labs.itch.io/time-seasons-starter) · [Free Lite](https://fableweld-labs.itch.io/time-seasons-free-lite) · [Bug reports](https://github.com/fableweldlabs/fableweldlabs/issues)

Starter includes the Lite clock, four seasons, editable day periods, signals, guided UI and isolated preview. It adds basic 2D/3D lighting, clock HUD options, sleep interactions, availability rules and clock-state save/restore. It does not include weather, custom calendars, growth, NPC pathfinding, inventory, quests or whole-game saves.

Download **Addon Only** for your own game. Lumen Vale's editable project and playable Windows demo are separate **optional** downloads. The demo can be tried for free; the editable project includes commercial dependencies for purchasers. Scenery and reflections are shared example work, not addon APIs.

## Quick starts

- [English](STARTER-QUICKSTART.en.md)
- [Español](STARTER-QUICKSTART.es.md)
- [Português (Brasil)](STARTER-QUICKSTART.pt_BR.md)
- [简体中文](STARTER-QUICKSTART.zh_CN.md)
- [日本語](STARTER-QUICKSTART.ja.md)
- [Français](STARTER-QUICKSTART.fr.md)
- [Deutsch](STARTER-QUICKSTART.de.md)
- [Polski](STARTER-QUICKSTART.pl.md)
- [한국어](STARTER-QUICKSTART.ko.md)
- [繁體中文](STARTER-QUICKSTART.zh_TW.md)
- [Türkçe](STARTER-QUICKSTART.tr.md)
- [Українська](STARTER-QUICKSTART.uk.md)

The dock and optional Lumen Vale example support the same twelve languages. Dialogue, controls, help, signs and localized place names follow the selection. Customer names, API identifiers and saved data remain stable. Translations are AI-assisted, without independent native-speaker review.

## Requirements and safe updates

Verified target: Godot 4.7.2, Windows x64. Other targets are unverified. Back up your project. Keep profiles, generated scenes and your code outside addons. Disable the plugin, replace only addons/rpg_time, then re-enable. Install one edition at a time. Open a copy of a Lite profile when converting; preserve the original. Inspect recovery files before retrying a failed save.

The optional editable example is a standalone project. Do not copy its project.godot over your own. Its save buttons store clock state only, not the player or an entire game.

## License and support

Commercial additions permit one purchasing person/entity, private project-team access and use in integrated exported games/apps. Paid source must remain private. MIT core and shared MIT scenery retain their rights; see the component map and license included with the purchase. This public hub supplies documentation and issues, not paid source archives.

[Report a reproducible bug](https://github.com/fableweldlabs/fableweldlabs/issues/new) without posting paid source, private saves or purchase details. Purchase support: fableweldlabs@gmail.com. No perpetual update or response-time promise is made. Copyright (c) 2026 Gordon Hinchen; Fableweld Labs branding.

## Runtime HUD and extended controls
The generated rig now includes a glossy reusable clock HUD, matching sleep control and a language selector. The selector translates built-in HUD text, interaction prompts and generated instructions without changing your game’s TranslationServer or custom names. For a custom HUD, use its language_code field or set_language("ja"). FWHUDStyle controls colors, font, padding, corners and clock size; the clock caches its appearance instead of rebuilding it on every tick. Existing custom sleep captions are preserved. Lumen Vale uses this actual reusable HUD, not a separate imitation.
The generated language controller is scoped to its own rig and explicitly marked built-in text. It leaves arbitrary customer labels alone. The smaller 2D/3D examples also localize their paid action buttons, save feedback and availability explanations.

## Update 2.2.0

Polish, Korean, Traditional Chinese, Turkish and Ukrainian join the existing seven languages. Interface text, quick starts and the optional example's dialogue, signs and controls are included.

The reusable clock card formats its date only when the date or language changes. Set `compact_mode` in the card Inspector to hide secondary labels while keeping date, time and day progress; its tooltip retains full context. The translation helper caches formatted-message patterns per language and now handles padded times, precision and literal percent signs.

Only Addon Only is required. Both example downloads remain optional; the Windows demo remains free. Prices and the active launch sale are unchanged.

