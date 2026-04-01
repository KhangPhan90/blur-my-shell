# Blur my Shell

Fork of [aunetx/blur-my-shell](https://github.com/aunetx/blur-my-shell).

This fork is focused on keeping the extension working on newer GNOME Shell
releases with a small, targeted compatibility patch.

## What this fork fixes

- Improves application blur handling when compositor actors are missing or
  change shape, avoiding crashes and broken opacity updates.
- Stops relying on the last child actor for overview blur-on-overview logic,
  which makes the content actor selection more robust.
- Adds null-safe handling during workspace switch preparation and cleanup.
- Restores patched workspace-switch methods more safely to avoid prototype
  conflicts.
- Updates extension metadata to advertise GNOME Shell 50 support.
