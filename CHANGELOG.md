# Zorvo changelog

Snapshots (beta) are marked; full releases are the stable versions.

## Zorvo 0.0.3(26w43p) - 2026-10-24

- Fixed: Testing a game in the editor showed the Python icon; it now shows the Zorvo logo
- Changed: the test window title ends with 'Made with Zorvo'

## Zorvo 0.0.3(26w43o) - 2026-10-24

- Fixed: Update check no longer hangs on 'Fetching update...' on some networks (GitHub API and release feed are now asked at the same time)

## Zorvo 0.0.3(26w43n) - 2026-10-24

- Changed: License and Terms of Service now clearly protect the engine, the Made with Zorvo credit and the Zorvo name, while your games stay yours

## Zorvo 0.0.3(26w43m) - 2026-10-24

- Added: + menu has Folder; right-click Explorer shows Add with a side menu and icons
- Added: press F3 while testing to show hitboxes
- Added: License page (Help menu and Projects page)
- Changed: engine errors no longer show technical details
- Fixed: update check works on other computers (backup release feed)

## Zorvo 0.0.3(26w43l) - 2026-10-24

- Fixed: exported games and running games show the Zorvo logo in the window instead of the default Python/pygame icon
- Fixed: File > Updates could stay on 'Checking for updates...' forever on other computers; it now gives up after 20 seconds with a clear message and a Try again button

## Zorvo 0.0.3(26w43k) - 2026-10-24

- Added: the Mac app can update itself without a new Mac build: every release now carries the engine's compiled code (Zorvo-code.zip) and the Mac app downloads it from File > Updates
- Changed: the Mac installer is one file, Zorvo-mac-arm64.dmg, attached to every release from 0.0.3 on

## Zorvo 0.0.3(26w43j) - 2026-10-24

- Added: main.zv always starts the game and cannot be renamed or deleted; other scripts start from code: var e = explorer/scripts/enemy then e.start (also /scripts/enemy, e.running)
- Added: Properties of a script has 'Start when the game starts' and copy-ready start lines; new scripts start switched off (older projects keep working)
- Added: hitboxes. Every picture has one, edited in the sprite editor (Hitbox tool, Fit to the drawing, Whole picture); collisions use it, also when sprites are resized or rotated
- Added: sprite editor gets Line, Rectangle, Ellipse (filled option), mirror drawing, select area + Crop, Trim empty edges, Flip, Turn 90, and Resize with an anchor or stretch; the hitbox follows every crop and resize
- Added: your own folders and files sit under the three built-in ones in the Explorer (the Files section is gone); drag them into folders or onto empty space, sub-folders as deep as you like, right-click empty space for new folders
- Added: the Mac app can update itself (downloads the Mac build of the release and replaces Zorvo.app)
- Fixed: code examples in the Docs can be selected with the mouse, and the Copy button sits in the top-right corner of each box
- Changed: Docs explain several scripts and hitboxes

## Zorvo 0.0.3(26w43i) - 2026-10-24

- Added: sprite objects - var hero = workspace.assets.hero.png, then hero.position.x / hero.position.y (read and change), hero.width, hero.rotation; sprite commands accept the object too. Old code keeps working
- Changed: indentation uses tabs, shown as a small arrow (never saved or copied); old space-indented scripts convert when opened
- Changed: Docs can be selected and copied (Ctrl+C, right-click, Copy button on every example), have a search box (Ctrl+F) and a cleaner look

## Zorvo 0.0.3(26w43h) - 2026-10-24

- Added: autocomplete in the script editor (like VS Code): suggestions appear while you type for keywords, built-in commands (with their arguments), and your own functions and variables
- Added: Tab or Enter accepts a suggestion, Esc closes it, Ctrl+Space opens it any time
- Added: typing func, if, while, for or repeat on an empty line and accepting writes the whole block

## Zorvo 0.0.3(26w43g) - 2026-10-24

- Added: the game window can be resized; the game scales evenly and stays centred (text in the middle stays in the middle), no code changes needed
- Added: Ctrl+F find bar in the script editor (Enter / Shift+Enter / F3, Esc closes)
- Changed: Terminal colors: errors red, warnings yellow, print output green, commands blue

## Zorvo 0.0.3(26w43f) - 2026-10-24

- Fixed: The X on editor tabs was cut off

## Zorvo 0.0.3(26w43e) - 2026-10-24

- Removed: Movement system and Window size choices from the New project page
- Changed: The Empty template is now truly empty (an empty main.zv and an assets folder, no sample sprites or code)
- Changed: Panel sizes (Explorer, Properties, Terminal) are remembered across all projects

## Zorvo 0.0.3 - 2026-10-24

- Added: right-click a project on the Projects page to Open, Rename, Show in Explorer, Remove from list or Delete it (F2 renames, Delete deletes). Deleting asks first and refuses anything that is not a Zorvo project.
- Fixed: File > Updates says Update to when a version is newer than yours and Switch back to only when it is older.
- Changed: snapshots now carry the full version they are built on (after 0.0.3 they are 0.0.3(26w44a) and so on; the next full version is 0.0.4), and snapshots of older versions are never offered.

## Zorvo 0.0.2(26w43d) - 2026-10-24

- Added: right-click a project on the Projects page to Open, Rename, Show in Explorer, Remove from list, or Delete it (F2 renames, Delete deletes). Renaming also updates the game window title if it still had the old name; deleting asks first and refuses anything that is not a Zorvo project.

## Zorvo 0.0.2(26w43c) - 2026-10-24

- Fixed: File > Updates no longer says Switch back to a full version that is actually NEWER than your snapshot. It says Update to when it moves you forward and Switch back to only when it goes back.
- Changed: snapshots carry the full version they are built on (after full 0.0.2 the snapshots are 0.0.2(26w44a)...; the next full version is 0.0.3). The two earlier snapshots were renamed 0.0.1(26w43a) and 0.0.1(26w43b).

## Zorvo 0.0.2 - 2026-10-24

- Added: New project page in the Projects hub: Name (max 32 characters, blank = Project 1), Template (Coin Collector or Empty), Movement system (None, arrow keys/WASD or Platformer) and window size. Terms of Service and Privacy Policy are in the Projects menu too.
- Added: Share your game as a Windows .exe (File > Export): one file, named after your project, that runs by itself. It shows a short, small Made with Zorvo credit first. A Mac .dmg is planned (it needs a Mac build).
- Added: Zarv# errors have numbers, like Error 20 on line 5: Unknown name. The Docs list what every number means (Error 404 = unknown).
- Added: repeat 5 times loops, the in operator, list functions remove / pop / contains, set_rotation() and restart_game().
- Added: the sprite editor handles pixel art up to 4096 x 4096 with zoom, panning, undo / redo, brush sizes and a fast fill. Import an image into a sprite from inside its tab; right-click a picture to duplicate it.
- Added: Explorer with a small + beside its name (Script or Sprite, with search), right-click to rename or delete, matching icons, folder icons that stay correct; Ctrl+Z / Ctrl+Y undo and redo changes to your scene.
- Added: multiple scripts (each in its own tab), scripts scroll sideways, View > Word wrap in scripts, Explorer / Properties / Terminal can be hidden.
- Added: Updating opens its own small window, saves your project, closes Zorvo, installs, and reopens on the Projects page.
- Added: Uninstall wizard (Windows Settings > Apps).
- Added: snapshots (beta versions) in File > Updates, named like 0.0.3(26w44a), with the latest version and its changelog.
- Changed: the toolbar is the project name with a small run button beside it; Save and Export are in the File menu. Moving objects in the viewport and painting sprites are much smoother.
- Fixed: Failed to load Python DLL error after an update (confirmed cause and fix; copies updated from older snapshots may show it once - just open Zorvo again).

## Zorvo 0.0.1(26w43b) - 2026-10-24

- Removed: the .zarv file format. Games are now shared as a Windows .exe (one file, runs by itself). A Mac .dmg is planned but needs a Mac build.
- Added: exported games show a short, small "Made with Zorvo" credit with a soft fade before the game starts (click or press a key to skip).
- Added: Zarv# errors now have numbers, like Error 20 on line 5: Unknown name 'speed'. The Docs have an Error Codes list explaining every number (Error 404 = unknown).
- Added: repeat 5 times loops, the in operator (if x in my_list), list functions remove / pop / contains, set_rotation() and restart_game() - enough to make a game like Flappy Bird.
- Added: the sprite editor now handles pixel art up to 4096 x 4096 with zoom, panning, undo / redo, brush sizes and a fast fill. New sprites ask for a size.
- Added: scripts scroll sideways; View > Word wrap in scripts wraps long lines on screen.
- Added: Explorer: one + button with search, right-click to rename / delete, folder icons fixed, sprites open in their own tab.
- Changed: the toolbar is just a small run button; Save and Export are in the File menu.
- Fixed: safer restart after an update (clean start environment and a short wait) to avoid the Failed to load Python DLL error.

## Zorvo 0.0.1(26w43a) - 2026-10-24

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
- Added: Zarv# language with Tab auto-complete for blocks, key names like arrow_left and w, velocity and gravity, and full docs with examples.
- Added: projects auto-save; closing a project returns to the hub, closing the hub quits.
- Added: installer with Terms/Privacy acceptance and optional desktop shortcut.
- Added: File > Updates with snapshots (beta), green progress bar, and a launch popup for new full versions.

