# Third-party notices

This site includes or loads the following third-party software. Each component keeps its own copyright and licence.

## Bundled inside `index.html`

### Bible Strong Avatar Lab (mascot engine)

- Packages: `@bible-strong/avatar-web` 0.1.0 and `@bible-strong/avatar-core` 0.1.0
- Copyright (C) 2026 Stéphane Montlouis-Calixte
- Licence: GNU Affero General Public License v3.0 ([LICENSE](./LICENSE))
- Source: https://github.com/smontlouis/bible-strong-avatar-lab
- Use here: the packages are bundled unmodified into the `<script id="avatar-engine">` block.
- Changes made: the mascot definition in `<script id="mascot-def">` is adapted from the project's `strobi.avatar.json` example. The body was changed to a rounded cube with a graduation cap, the colours were changed, and the set of expressions and animations was reduced.

### Ajv and its dependencies (bundled with the mascot engine)

| Package | Version | Licence | Licence text |
| --- | --- | --- | --- |
| ajv | 8.20.0 | MIT | [licenses/ajv-MIT.txt](./licenses/ajv-MIT.txt) |
| fast-uri | 3.1.9 | BSD-3-Clause | [licenses/fast-uri-BSD-3-Clause.txt](./licenses/fast-uri-BSD-3-Clause.txt) |
| fast-deep-equal | 3.1.3 | MIT | [licenses/fast-deep-equal-MIT.txt](./licenses/fast-deep-equal-MIT.txt) |
| json-schema-traverse | 1.0.0 | MIT | [licenses/json-schema-traverse-MIT.txt](./licenses/json-schema-traverse-MIT.txt) |

## Loaded from a CDN at runtime (not stored in this repository)

- [three.js](https://github.com/mrdoob/three.js) r128, MIT licence, from cdnjs. Draws the network animation in the header.
- [Google Fonts](https://fonts.google.com): Cormorant Garamond, Lora and DM Sans, SIL Open Font License 1.1.
