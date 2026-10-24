# Zorvo changelog

Snapshots (beta) are marked; full releases are the stable versions.

## Zorvo 0.0.2(26w43b) - 2026-10-24

- Added: .zarv - a portable Zorvo game file. Export > Export as .zarv saves your game as one file named after your project; it is the same file on every operating system and plays in any Zorvo player.
- Added: on Windows, double-click a .zarv (or drag it onto Zorvo) to play it. The installer and the app set this up; uninstall removes it.
- Added: Export menu with both options: .zarv (any device) and .exe (Windows, runs by itself with nothing installed). Files are named after your project.
- Added: Zorvo Player and build_player.py so a player can be built for macOS and Linux (it must be built on those systems).
- Changed: games now carry a manifest (name, engine version) and give a friendly message if a game needs a newer Zorvo.

## Zorvo 0.0.2(26w43a) - 2026-10-24

- Added: New project page in the hub with settings: Name (max 32 characters, blank = Project 1), Template (Coin Collector or Empty), Movement system (None, arrow keys/WASD, or Platformer with jumping) and window size. A fresh install now starts with no projects.
- Added: Export game as .exe - File > Export game as .exe makes ONE file you can send to friends; they play it without installing anything.
- Added: Multiple scripts - View > Scripts opens each script as its own tab named after the file; + Script in the Explorer; all scripts run together and errors name the file.
- Added: Explorer and Properties stay visible on every tab; hide or show Explorer, Properties and Terminal from the View menu.
- Added: custom icons in the same green/gray style (folder and open folder, script, image, object, game) instead of arrows.
- Added: clicking a picture in Assets previews it in Properties and shows it in the Sprites editor.
- Changed: the Sprites editor scales with the window, its left side scrolls instead of getting cut off, and painting is much smoother (fills gaps in fast strokes).
- Changed: moving objects in the viewport no longer lags.
- Added: Uninstall wizard (Windows Settings > Apps).
- Changed: snapshots are now named like 0.0.2(26w43a).

## Zorvo 0.0.1 - 2026-10-24

- Added: Projects hub - a main menu listing every project on this device; opening one opens it in its own window. First project is "My First Zorvo Project".
- Added: Environment with Explorer, Viewport and Properties; drag objects to change what draws in front.
- Added: closable Script, Sprites (pixel art) and Docs tabs; one Run/Stop button; Terminal with commands.
- Added: ZorvoScript language with Tab auto-complete for blocks, key names like arrow_left and w, velocity and gravity, and full docs with examples.
- Added: projects auto-save; closing a project returns to the hub, closing the hub quits.
- Added: installer with Terms/Privacy acceptance and optional desktop shortcut.
- Added: File > Updates with snapshots (beta), green progress bar, and a launch popup for new full versions.

