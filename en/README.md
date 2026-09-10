# Dishwasher simulator

This English project builds a Scratch dishwasher simulator in the Raspberry Pi Code Editor.

## Project files

- `landing.md` introduces the game and embeds the published Scratch player.
- `step_1.md` to `step_29.md` contain 28 build steps and a final challenge.
- `meta.yml` defines the step titles, order, completion markers, and landing-page setting.
- `code/editor-dishwasher-sim-starter/` contains `editor-dishwasher-sim-starter.sb3`, with sprites, costumes, and sounds but no scripts, variables, or lists.
- `code/editor-dishwasher-sim-complete/` contains `editor-dishwasher-sim-complete.sb3`, copied from the source project's completed reference.
- Both code folders have a `project_config.yml` with the matching editor identifier, `type: 'code_editor_scratch'`, and `build: true`.
- `solutions/` contains the completed Scratch project for download.
- `images/` contains the source screenshots and supporting images.

The Scratch archives and assets are copied unchanged from `dishwasher-sim`. The instructions retain the source's incremental code examples, including its list-length-based random dish selection. The supplied completed reference uses a fixed maximum of eight dishes, so extending that reference with a ninth dish also requires updating its random-selection blocks.
