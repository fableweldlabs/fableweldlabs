# Workflow examples

[Home](README.md) · [Getting started](GETTING-STARTED.md) · [Website](https://fableweld-labs.itch.io/)

These are written authoring recipes, not downloadable sample projects or claims that every edition includes every feature. Follow the released product's feature list and version-specific instructions when implementing them.

## A seasonal shop

Goal: a market opens at noon in Spring and Summer and closes during Autumn and Winter.

- Keep the clock and shop availability rules tied to the same game-time state.
- Give the player a readable open/closed indicator and an explanation of the current season or hours.
- Check the exact opening and closing boundaries, both included seasons and both excluded seasons.
- Save while open, advance into a closed state, then restore. The visible date and shop availability should agree after restoring.

## Sleeping until morning

Goal: sleeping advances game time to the next intended morning.

- Define the wake-up time and what should happen if the player sleeps before or after it.
- Decide how the game handles skipped events; a time jump should not silently create unlimited rewards or spawns.
- Test crossing midnight, a season boundary and a saved/restored state.
- Display the new time after waking so the result is understandable.

## Day/night lighting with readable UI

Goal: the world changes from day to night while the player's clock and controls remain readable.

- Let the game's clock drive the lighting response.
- Keep text contrast and focus indicators readable at both bright and dark times.
- Review the smallest supported viewport and the project's actual renderer.
- Treat 2D and 3D lighting as separate visual checks; success in one does not establish the other.

## Sharing a reproduction

Reduce a problem to the smallest scene that demonstrates it, using only files you may share. State the clock's starting date/time, pause/speed settings, rules and exact action sequence. Never upload Paid source or private project assets to a public issue. See [Support](SUPPORT.md).
