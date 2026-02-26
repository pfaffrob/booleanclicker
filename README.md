# BooleanClicker

BooleanClicker is a QGIS plugin for fast point digitizing into a boolean field.  
Left click writes **True**, right click writes **False**.

## Features

- Target layer list only shows point layers with at least one boolean field.
- Snapping-aware point placement (uses current QGIS snapping settings).
- Live preview marker while moving the mouse.
- Optional map recentering after insertion with configurable horizontal and vertical target position.
- Remembers last selected layer, field, and recenter settings.

## How to Use

1. Enable the plugin in QGIS Plugin Manager.
2. Click the BooleanClicker toolbar button.
3. Select a target point layer and boolean field.
4. (Optional) Enable recentering and choose horizontal/vertical target position.
5. Click **OK** to activate the tool.
6. Left click to add `True`, right click to add `False`.

## Notes

- The plugin starts an edit session automatically when needed.
- Save layer edits from QGIS when you finish digitizing.
- For icon/resource updates, rebuild `resources.py` from `resources.qrc`.