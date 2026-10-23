# Bulk Properties

> **This plugin is now part of [Vault Management](https://github.com/VeryRandomness/obsidian-vault-management)**, which combines bullet variants, color swatches, bulk property editing and theme updates in one plugin. This repo is archived and no longer updated.

An [Obsidian](https://obsidian.md) plugin to change properties across every note at once.

Run **Bulk edit properties** from the command palette, or click the list-checks icon in the ribbon.

1. **Pick a property.** Type to filter your property names; each shows how many notes use it.
2. **Tick values.** Search its values and tick one or more. Ticking several lets you merge them, for example `Inprogress` and `In progress` into `In Progress`. `(empty)` covers notes where the property is blank.
3. **Choose an action:** change the ticked values to a new one, remove them, or delete the property from those notes. In a list property, only the ticked items change.
4. **Check the list of notes, then apply.**

There is also **Rename...** on step 2, to rename a property or merge it into one that already exists. Lists are combined; if both properties hold different single values, the existing one is kept and the plugin tells you which notes.

Changes are made with Obsidian's own property editing. They can't be undone with Ctrl+Z, so check the list of notes first.

## Install

Copy `main.js`, `manifest.json` and `styles.css` into `<vault>/.obsidian/plugins/cb-bulk-properties/` (the folder name must match the plugin ID), then enable **Bulk Properties** under Settings → Community plugins.

## Updates

The plugin updates itself. On startup it compares the version in this repo's `manifest.json` with the installed one and, if the repo's is newer, installs the new files and reloads. The command **Check for update now** does the same on demand. To ship a change, raise `version` in `manifest.json` and push.

The ID `cb-bulk-properties` is deliberately not `bulk-properties`, which belongs to a different plugin in Obsidian's community store.
