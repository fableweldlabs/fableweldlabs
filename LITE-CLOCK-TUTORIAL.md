# Lite clock signal tutorial

[Full illustrated guide](https://fableweld-labs.itch.io/time-seasons-free-lite/devlog/1725172/tutorial-open-a-shop-with-godot-clock-signals) · [24-second demonstration with original audio](https://x.com/FableweldLabs/status/2114771823728685482)

## Run the small sample

1. From the [free product page](https://fableweld-labs.itch.io/time-seasons-free-lite#download), download **Time & Seasons Lite 2.1.0 — Addon Only** and **Clock Signal Tutorial — Optional**. No payment is required. Skip the large Lumen Vale downloads.
2. Extract the tutorial into a new folder. Extract the addon ZIP, then copy its `addons` folder beside the tutorial’s `project.godot`.
3. Import that project in Godot 4.7.2 and press F5. Keep your own project.godot unchanged.
4. Watch 05:50 cross 06:00: the sample shop opens. Try Next evening to close it, Skip 1 day to reach Summer, and Next morning to reopen.

## Why this works

The separate shop controller listens to `period_changed` and opens for Morning or Day. It also reads `clock.period_at()` when binding, so a scene beginning at noon starts open. Parent the clock before binding: its profile applies in `_ready()`. Read `shop.is_open` once for the initial display, then listen for `shop_state_changed`.

```gdscript
func _on_period_changed(period: String) -> void:
    _set_open(period in ["Morning", "Day"])
```

Default boundaries are 06:00, 12:00, 18:00 and 22:00. Adapt the allowed names if you customize periods. A time skip reports the destination state; it does not replay every missed morning or transaction. Do not advance the clock again inside its signal callback.

## Scope and verification

The shop, buttons and display are separate MIT example code, not built-in addon features. This sample does not provide inventory, buying/selling, persistence, weather or lighting. The addon supplies clock, periods, seasons and signals.

Fresh actual Godot viewport rendering confirmed morning opening, evening closing, the summer transition and reopening against the exact itch.io Lite 2.1.0 package, SHA-256 `bf78a1501e7b1358bb6eebb2dce169a34e2acfedf4749eb672dce45003fe4923`. Verified Godot 4.7.2 Windows x64; other targets are unverified. This is a deterministic runtime demonstration, not a recording of manual installation.

As checked October 26, 2026, the [Lite source repository](https://github.com/fableweldlabs/time-seasons-lite) and accepted legacy Godot listing remain at 1.4.0. Use the current itch.io addon for this updated sample. The earlier source tutorial remains available in that repository.

Copyright 2026 Gordon Hinchen; Fableweld Labs branding. Tutorial source includes its MIT license. Code and documentation were developed with Codex assistance. [Report a bug](https://github.com/fableweldlabs/time-seasons-lite/issues) with product version, engine version, OS and reproduction steps.
