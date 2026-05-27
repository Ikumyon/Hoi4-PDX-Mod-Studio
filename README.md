# HOI4 Syntax Plugin

This plugin is a data-only sample for Hearts of Iron IV grammar assets.

- No executable code is included.
- All assets are UTF-8 text files.
- The manifest is the plugin entrypoint metadata and may also declare `files.toml`.
- Manifest display text may use `name_key` and `desc_key`.
- Asset paths and element definitions are declared in `files.toml`.
- `files.toml` may declare `[i18n]`, and each locale may point to a JSON file or a directory of JSON files.
- `[[files]]` entries declare `name_key` for translatable UI labels.
- Translation resources are stored as locale files such as `translations/en-US.json`.
- `format` is intentionally not included because output formatting belongs to each custom tab or plugin-local asset.

Included assets:

- `files.toml`
- `translations/en-US.json`
- `grammar/syntax.toml`
- `grammar/values.toml`
- `grammar/schemas/decision_category.schema.json`
- `grammar/schemas/decision.schema.json`
- `grammar/statements/triggers.json`
- `grammar/statements/effects.json`

Current sample coverage:

- decision categories
- decisions
- trigger/effect rule placeholders

This plugin is meant to define syntax resources only. If the host later wires data-only grammar plugins into diagnostics, these assets are ready to be consumed without changing their file layout.
