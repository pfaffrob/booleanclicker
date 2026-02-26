BooleanClicker

BooleanClicker is a QGIS plugin that adds points with a boolean value by mouse click:

* Left click adds a point with the selected field set to True
* Right click adds a point with the selected field set to False

How to use

1. Load at least one point vector layer in QGIS.
2. Ensure the layer has a boolean field (type: Bool).
3. Click the BooleanClicker toolbar button or menu item.
4. Select the target point layer and boolean field.
5. Click OK to activate the map tool.
6. Left or right click on the map canvas to create points.

Notes

* The plugin starts editing on the selected layer automatically if needed.
* Save edits from QGIS when you are done digitizing.

Sharing with other users

Option 1 (quick internal sharing):
* Zip the entire plugin folder `booleanclicker`.
* Other users extract it into their QGIS plugins folder:
  * Windows: `%APPDATA%/QGIS/QGIS3/profiles/default/python/plugins`
  * Linux: `~/.local/share/QGIS/QGIS3/profiles/default/python/plugins`
  * macOS: `~/Library/Application Support/QGIS/QGIS3/profiles/default/python/plugins`
* Restart QGIS and enable the plugin in Plugin Manager.

Option 2 (official distribution):
* Upload the plugin package to the QGIS Plugin Repository.
* Keep `metadata.txt` up to date for each release.
