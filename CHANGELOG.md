# Changelog

All notable changes to **SimPushbackXP by SimLandings** will be documented in this file.  
This project follows [Semantic Versioning](https://semver.org/) and the format of [Keep a Changelog](https://keepachangelog.com/).

---

## [Unreleased]
- Planned: taxiway-aware headings (offer N/NE/E… based on nearest taxiway centerline), distance auto-calc improvements, and joystick/button commands.

## [0.0.12] - 2025-08-11 (dev)
### Added
- GitHub-ready repository package (README, CONTRIBUTING, LICENSE, templates).
- Branding links in code and docs (Website, YouTube, Instagram).
### Changed
- Version bump for public GitHub onboarding.

## [0.0.11] - 2025-08-10 (dev)
### Fixed
- Proper library object lookup (supports both enumerator callback signatures).
- Portable flight loop via `registerFlightLoopCallback` / `unregisterFlightLoopCallback`.
### Added
- **Bundled default tug model** (OBJ8) so a tug always appears even if library paths are missing.
- Settings: in‑menu “Reload XPPython3 Scripts”, debug per‑frame logging toggle.
- Idle loop to keep tug visible and aligned before pushback.

## [0.0.10] - 2025-08-10 (dev)
### Added
- Stronger heading steering so chosen direction is obvious (left/right/compass).
- Idle alignment so tug stays visible after script reloads.
- Menu: **Settings → Reload XPPython3 Scripts** (uses XPPython3 command if available).

## [0.0.9] - 2025-08-10 (dev)
### Added
- First visible tug instance using object instancing (library model).

## [0.0.8] - 2025-08-10 (dev)
### Fixed
- Safer flight loop creation; extra scheduling logs.
### Added
- Diagnostics and error logging improvements.

## [0.0.7] - 2025-08-10 (dev)
### Fixed
- Menu selection crash (non‑int itemRef). Switched to integer action IDs + map.

## [0.0.6] - 2025-08-10 (dev)
### Fixed
- Menu bug handling; improved exception reporting in menu handler.

## [0.0.5] - 2025-08-10 (dev)
### Added
- Branded plugin name: **SimPushbackXP by SimLandings** (hard‑coded).
- Direction presets and logging to `SimPushbackXP.log`.

## [0.0.4] - 2025-08-09 (dev)
### Fixed
- Implemented required `class PythonInterface` wrapper for XPPython3 legacy API.

## [0.0.3] - 2025-08-09 (dev)
### Fixed
- Correct folder placement and load order under `Resources/plugins/PythonPlugins/`.

## [0.0.2] - 2025-08-09 (dev)
### Added
- Initial menu structure: tug selection, distance presets, start/stop entries.

## [0.0.1] - 2025-08-08 (dev)
### Added
- Core pushback motion (reverse with acceleration, distance target).

## [0.0.0] - 2025-08-08 (dev)
### Added
- Initial scaffolding, project structure, and versioning scheme.
- Error database started (E‑0001…).
  
---

## Error Codes (summary)
- **E‑0001**: Plugin not visible → folder/Windows unblock.  
- **E‑0002**: Missing `PI_` prefix → rename to `PI_SimPushbackXP.py`.  
- **E‑0003**: Missing `PythonInterface` class → implement legacy API wrapper.  
- **E‑0004**: Menu type error (`method` vs `int`) → integer action IDs.  
- **E‑0005**: No movement (loop not firing / on_ground=0) → register loop + debug logging.  
- **E‑0006**: Crash selecting “Super Tug” → integer IDs fix.  
- **E‑0007**: No tug visual → correct enumerator + bundled OBJ fallback.  
- **E‑0008**: Flight loop signature mismatch → use register/unregister callbacks only.

---

## Release/Tag Notes
Create and push tags per version:
```bash
git tag v0.0.12
git push origin v0.0.12
```
Then draft a GitHub Release and paste the matching section from this changelog.
