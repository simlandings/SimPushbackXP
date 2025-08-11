# SimPushbackXP Changelog

## [0.0.13-dev] - 2025-08-10
### Added
- **Default X-Plane 12 tug model support** — no more bundled OBJ file; the plugin now uses built-in library tug objects such as:
  - `lib/airport/vehicles/pushback/tug.obj`
  - `lib/airport/vehicles/pushback/tug_lrg.obj`
  - `lib/airport/vehicles/ground_handling/tug.obj`
  - `lib/airport/vehicles/ground_handling/towtractor.obj`
- **Improved turning behavior** — aircraft now begins rotation earlier in the pushback for a smoother and more visible curve.
- **Parking brake auto-release** — brake is released when pushback starts to avoid drag or incomplete movement.
- **Detailed logging** — log file now records which library object was resolved and loaded, plus optional per-frame debug lines.
- **Compatibility fallback** — tries multiple object lookup signatures to work across different XPPython3 versions.

### Changed
- Removed dependency on `objects/tug_default.obj` to prevent the “IDX count is out of range” startup error.
- Slightly increased turn rate limits for tighter ground maneuvering.

### Fixed
- Startup crash when selecting a tug type with no corresponding model loaded.
- Pushback always moving straight back — now direction choices (90°, 180°, compass headings) are properly applied.

### Download
📦 **Patch download:** [SimPushbackXP_patch_0.0.13-dev.zip](sandbox:/mnt/data/SimPushbackXP_patch_0.0.13-dev.zip)

### Installation
1. Extract the zip.
2. Copy `PI_SimPushbackXP.py` into:
   ```
   X-Plane 12/Resources/plugins/PythonPlugins/
   ```
3. Delete any old bundled tug objects from:
   ```
   X-Plane 12/Resources/plugins/PythonPlugins/objects/tug_default.obj
   ```
4. Reload scripts in-sim: **Plugins → XPPython3 → Reload Scripts**, or restart X-Plane.

---
## [0.0.12] - 2025-08-09
- Added SimLandings branding in code and menus.
- Included `simlandings.com`, YouTube, and Instagram links in plugin metadata.

## [0.0.11] - 2025-08-08
- Direction menu implemented (Left 90°, Right 90°, Opposite, compass points).
- Logging system added with toggle.
- Auto distance fallback added.

## [0.0.10] - 2025-08-07
- Initial working pushback implementation.
- Menu structure created for tug selection, distance, and start/stop control.

## [0.0.0] - 2025-08-06
- Initial commit: project structure, XPPython3 framework setup, tug data table.
