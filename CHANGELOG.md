# Zorvo changelog

Snapshots (beta) are marked; full releases are the stable versions.

## Zorvo 0.0.2(26w43a) - 2026-10-24

- Added: New project page in the hub with settings: Name (max 32 characters, blank = Project 1), Template (Coin Collector or Empty), Movement system (None, arrow keys/WASD, or Platformer with jumping) and window size. A fresh install now starts with no projects.
- Added: Share your game - Export as .zarv (works on any device with Python and pygame-ce: python MyGame.zarv; on Windows double-click it) or as .exe (Windows, runs by itself with nothing to install). Files are named after your project.
- Added: Terms of Service and Privacy Policy in the Projects menu (Help menu and footer links), not only inside a project.
- Added: Multiple scripts - View > Scripts opens each script as its own tab; all scripts run together and errors name the file.
- Added: Explorer and Properties stay visible on every tab; hide or show Explorer, Properties and Terminal from the View menu.
- Added: custom matching icons (folder, open folder, script, image, object, game) instead of arrows.
- Added: clicking a picture in Assets previews it in Properties and shows it in the Sprites editor.
- Added: Uninstall wizard (Windows Settings > Apps) and .zarv double-click support on Windows.
- Added: Zorvo Player and build_player.py.
- Changed: the Sprites editor scales with the window, its left side scrolls, and painting is much smoother; moving objects in the viewport no longer lags.
- Changed: snapshots are named like 0.0.2(26w43a).

## Zorvo 0.0.1 - 2026-10-24

- Added: Projects hub - a main menu listing every project on this device; opening one opens it in its own window. First project is "My First Zorvo Project".
- Added: Environment with Explorer, Viewport and Properties; drag objects to change what draws in front.
- Added: closable Script, Sprites (pixel art) and Docs tabs; one Run/Stop button; Terminal with commands.
- Added: ZorvoScript language with Tab auto-complete for blocks, key names like arrow_left and w, velocity and gravity, and full docs with examples.
- Added: projects auto-save; closing a project returns to the hub, closing the hub quits.
- Added: installer with Terms/Privacy acceptance and optional desktop shortcut.
- Added: File > Updates with snapshots (beta), green progress bar, and a launch popup for new full versions.

