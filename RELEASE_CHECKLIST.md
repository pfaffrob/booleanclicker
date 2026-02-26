# BooleanClicker Release Checklist

Use this checklist before publishing to the QGIS Plugin Repository.

## 1) Metadata

- [ ] Update `metadata.txt` URLs:
  - `homepage`
  - `repository`
  - `tracker`
- [ ] Confirm `version` is correct for this release
- [ ] Keep `changelog` aligned with release changes
- [ ] Verify `category`, `tags`, `description`, and `about`

## 2) Build generated files

From plugin folder:

```powershell
& 'C:\Program Files\QGIS 3.40.15\bin\python-qgis-ltr.bat' -m PyQt5.pyrcc_main -o resources.py resources.qrc
```

- [ ] `resources.py` regenerated after icon/resource updates

## 3) Manual QA in QGIS

- [ ] Plugin loads with no startup errors
- [ ] Target layer dropdown only shows point layers with boolean fields
- [ ] Left click inserts `True`, right click inserts `False`
- [ ] Snapping (magnet) affects placement when enabled
- [ ] Preview marker is visible and updates during map pan
- [ ] Recenter option works (including custom horizontal/vertical positions)
- [ ] Dialog remembers last layer/field/recenter settings after reopen

## 4) Package

- [ ] Create clean plugin ZIP named `BooleanClicker.zip`
- [ ] ZIP root contains plugin folder `BooleanClicker/` with all required files
- [ ] Exclude caches/temp files (e.g., `__pycache__`, local IDE files)

## 5) Publish

- [ ] Log in to plugins.qgis.org
- [ ] Upload ZIP
- [ ] Fill/update release notes
- [ ] Confirm listing icon, description, and version are correct

## 6) After publish

- [ ] Install/update from repository in a clean QGIS profile
- [ ] Smoke test main workflow
