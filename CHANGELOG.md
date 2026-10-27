# Zorvo changelog

Snapshots (beta) are marked; full releases are the stable versions.

## Zorvo 0.0.10(26w44b) - 2026-10-27

Changed: Zorvo Settings is now a popup everywhere, with the license, terms and privacy links at the top, Latest Release / Latest Snapshot (with the beta warning) and the auto-update options.
Changed: Check for updates now lives only in Zorvo Settings.
Changed: The Projects screen has the same menu bar as the editor; things that need a project are greyed out. Export as file is only usable inside a project.
Changed: The Projects screen looks good in a big window and in full screen (F11).
Fixed: The Projects screen closes right away when you open a project.
Fixed: The mouse turns into a text cursor in the script editor and Terminal.
Fixed: hitboxes.json and filters.json are hidden from the Explorer, the Terminal and scripts.

## Zorvo 0.0.10(26w44a) - 2026-10-27

Added: Typing func suggests the hooks on_start, on_update and on_click.
Added: The Properties panel scrolls sideways when it is too narrow.
Changed: A func can now change and make a gvar.
Fixed: Text labels stay sharp when you zoom the viewport, and zoomed pictures look smooth unless they are pixel art.

## Zorvo 0.0.10 - 2026-10-26

Changed: The i next to a suggestion opens the exact docs section for that word, like the Variables section for var.
Changed: Hooks like on_start, on_update and on_click are not suggested, because Zorvo calls them for you and they are not functions.
Changed: The deprecated commands in the docs have a clear table with the versions they work in.

### Also new since the last full version (from the snapshots)

**Zorvo 0.0.9(26w44b)**
Added: wait(seconds) for while forever and while true loops, and Error 51 for a while true loop that never rests or ends.
Added: Suggestions use a smart search (left finds arrow_left, explroer finds explorer), show each name once, and have an i that opens the docs page.
Changed: The hooks on_start, on_update and on_click work again and are suggested after func. Starter games use them. The old Project Settings choice is gone.
Changed: Playing a game opens it in its own window again. Playing inside the Viewport is a choice in Zorvo Settings.
Changed: The docs show the versions once on top of each subcategory, faint, and deprecated things show a range like 0.0.1-0.0.8.
Fixed: If the game crashes, what Python says is shown in the Terminal.

**Zorvo 0.0.9(26w44a)**
Fixed: Testing a game opens in a second or two instead of unpacking Zorvo all over again (it took 10 seconds or more).
Changed: The loading picture says Loading into Zorvo Engine when you open Zorvo, and Loading your game when you test a game, with dots that count . .. ... .

## Zorvo 0.0.9(26w44b) - 2026-10-26

Added: wait(seconds) for while forever and while true loops, and Error 51 for a while true loop that never rests or ends.
Added: Suggestions use a smart search (left finds arrow_left, explroer finds explorer), show each name once, and have an i that opens the docs page.
Changed: The hooks on_start, on_update and on_click work again and are suggested after func. Starter games use them. The old Project Settings choice is gone.
Changed: Playing a game opens it in its own window again. Playing inside the Viewport is a choice in Zorvo Settings.
Changed: The docs show the versions once on top of each subcategory, faint, and deprecated things show a range like 0.0.1-0.0.8.
Fixed: If the game crashes, what Python says is shown in the Terminal.

## Zorvo 0.0.9(26w44a) - 2026-10-26

Fixed: Testing a game opens in a second or two instead of unpacking Zorvo all over again (it took 10 seconds or more).
Changed: The loading picture says Loading into Zorvo Engine when you open Zorvo, and Loading your game when you test a game, with dots that count . .. ... .

## Zorvo 0.0.9 - 2026-10-26

Changed: Tabs switch and close instantly, like a browser, without redrawing the whole editor.
Changed: Zorvo Settings is only in the File menu now, not in the Explorer.
Changed: The loading picture says Loading your game.
Changed: The anchor point can only go from -2.5 to 2.5.
Fixed: Turning a drawing is smooth now (pixel art keeps its hard pixels).
Fixed: The game keeps its window open even if a frame cannot be drawn, and it uses the frame rate from Project Settings.

### Also new since the last full version (from the snapshots)

**Zorvo 0.0.8(26w44m)**
Fixed: The Properties panel scrolls when the window is too small, so nothing is cut off.

**Zorvo 0.0.8(26w44l)**
Fixed: while forever now works inside a function you call once, like start().
Added: Yellow warnings when a function is made twice, or when on_start or on_update is made in a project that does not call them by itself.
Fixed: A cropped object no longer uses the hitbox of the whole picture in the Viewport.

## Zorvo 0.0.8(26w44m) - 2026-10-26

Fixed: The Properties panel scrolls when the window is too small, so nothing is cut off.

## Zorvo 0.0.8(26w44l) - 2026-10-26

Fixed: while forever now works inside a function you call once, like start().
Added: Yellow warnings when a function is made twice, or when on_start or on_update is made in a project that does not call them by itself.
Fixed: A cropped object no longer uses the hitbox of the whole picture in the Viewport.

## Zorvo 0.0.8 - 2026-10-26

Added: Border system: border, player touches border, border:Keep(player), KeepInside and TouchingBorder.
Added: while forever do loops, and your own functions instead of on_start and on_update in new projects.
Added: print, warn and error, and Workspace/name paths (explorer/ is optional, capital letters matter).
Added: Hitbox points tool in the vector editor for custom hitboxes.
Added: Quote and bracket auto-pairing, better suggestions, and a tab arrow that can no longer be split.
Added: Zorvo Settings fonts and colors, Project Settings tab, 40 Google fonts, Crop for objects, more menu items.
Changed: Drawings stay sharp at any size in the Viewport and the game. No more black bars: the game fills the window.
Changed: Auto update is off by default. The docs show versions, snapshots and a fuzzy search.

### Also new since the last full version (from the snapshots)

**Zorvo 0.0.7(26w44k)**
- Added: Tween. box:Tween(transparency(1, 0, 1)) changes a property smoothly over time (x, y, width, height, rotation, transparency, saturation, edgeamount, hue), no bounce
- Added: Edges in Properties: Straight, Indent or Smooth, with an amount slider that only shows for Indent and Smooth
- Added: objects now turn around their anchor point, and the anchor dots and hitboxes can be shown or hidden above the viewport
- Added: Zorvo Settings (File menu) for the whole app, with automatic updates for full versions. Project Settings stay for one game
- Added: sprites have a Filter (Auto, Pixel or Smooth), and vector sprites are saved bigger so they are smooth instead of pixelated
- Added: vector sprites have a film strip for frames and animations
- Added: Hue now tints a picture, and the sliders have number boxes so you can type exact values
- Added: code suggestions for the objects in your Workspace and their properties, and you can click them
- Added: the thick green line on the loading picture moves while Zorvo starts
- Changed: the Properties panel updates in place and does not flash, and moving, turning and drawing are smoother
- Changed: the + list shows everything and greys out what cannot go there, and right-click Add opens the same list
- Changed: the starter games have comments that explain every part
- Changed: names are the same in Properties and in code, and a name with a space is written without it
- Removed: the gravity property and the set_gravity command (the Platformer and Duck Jumping make their own gravity)
- Fixed: the drawing editor keeps your tool after you draw, and the line you drag looks the same as the finished line

**Zorvo 0.0.7(26w44j)**
- Added: new sprites can be Vector (shapes, smooth lines) or Pixel art, you pick when you add one
- Added: a Fill tool, live drawing while you drag, and Move forward 1 / Move back 1 for layers (greyed out when they cannot move)
- Added: icons on every tab, and when there are too many tabs they show just the icon
- Added: click a suggestion in the code list to use it, and the list scrolls when it is long
- Added: dragging an object out of the Workspace shows the blocked sign
- Changed: Frames, Saved data, Updates and the License pages open as tabs, and renaming is typed in the Explorer, so no extra windows
- Changed: the Updating window stays on screen with a Loading bar, and Zorvo comes to the front when it restarts
- Changed: Color is called Hue (Text Color for text), and in code it has no space: hue, textcolor
- Removed: the gravity property. The Platformer and Duck Jumping presets now do their own gravity in their script
- Fixed: Transparency and Saturation now show in the viewport
- Fixed: moving the viewport, scrolling code and the drawing editors are smooth (the scroll bars were slowing them down)
- Fixed: the viewport can be moved far in every direction, and the side panels in the drawing editors can be resized
- Fixed: line numbers appear at once when you press Enter
- Changed: the tab bar is grey instead of blue, and the animation panel is simpler

**Zorvo 0.0.7(26w44i)**
- Added: vector drawing. Sprites are shapes now (rectangle, ellipse, line, pen, freehand) that you can move, resize and reorder, drawn smooth, no pixels
- Added: the command bar can change things, like explorer/workspace/object1.gravity = 1
- Added: drag scripts and sprites into any folder, and a blocked sign shows where you cannot drop
- Added: drop a picture on an object in the Explorer to give it that texture
- Changed: Play and Stop are only in the viewport, the top bar and Test in window are gone
- Changed: a game with an error in its code is reported at once instead of opening the window first
- Changed: an error while the game runs no longer freezes it
- Changed: changing Visible or Gravity no longer reloads the whole Properties panel, and Properties show less text
- Changed: the selection lines in the viewport are solid

**Zorvo 0.0.7(26w44h)**
- Added: folders inside Scripts and Assets; drag a script or sprite onto a folder (or onto the list name to take it out)
- Added: + on the Scripts and Assets rows can make a folder
- Fixed: the pinned taskbar icon and the running Zorvo are one icon again (the pinned shortcut now always gets the same ID, and Zorvo Admin and Zorvo Kids shortcuts are left alone)

**Zorvo 0.0.7(26w44g)**
- Added: a Loading your app... picture while Zorvo starts, and the restart after an update is faster
- Added: Texture picker in Properties with a search box, Import image, and drag a picture from Assets onto Properties
- Added: Transparency and Saturation sliders in Properties (also obj.transparency and obj.saturation in scripts)
- Added: new objects start as a grey placeholder box with an X
- Added: a picture follows your mouse while you drag things in the Explorer
- Changed: naming a new folder, sprite or script is typed right in the Explorer, no popup window
- Changed: hidden objects are fully hidden in the viewport
- Changed: the Projects window has a fixed size, because maximized it looked stretched
- Fixed: the viewport no longer snaps while you move around

**Zorvo 0.0.7(26w44f)**
- Added: Play and Stop right inside the viewport (Play button, F5), plus a Test in window button for final testing
- Added: drag a picture from Windows onto the Explorer to make a sprite, or onto the drawing editor to put it in
- Added: a + on the Workspace, Scripts and Assets rows, and Object in the + menu
- Added: in the drawing editor, drag the selected area and it follows your mouse
- Changed: hidden objects show faded in the viewport
- Changed: the Made with Zorvo credit only shows in exported games
- Changed: Export menu just says .exe and .dmg
- Fixed: pressing Enter after if ... then now adds end, also inside a func
- Fixed: less lag when typing code, zooming and moving things in the viewport

**Zorvo 0.0.7(26w44e)**
- Changed: Back to the earlier light look: light panels, the normal menu bar, and Frames, Saved data and Updates open in their own windows again
- Kept: the (i) help buttons, anchor point, Enabled and AutoStart for scripts, presets with real scenes
- Added: Visible and Gravity properties for every object (with (i) help)

**Zorvo 0.0.7(26w44d)**
- Added: anchor points. Every object has an anchor point (default 0, 0 = top left, so old games are unchanged). x and y are where the anchor is. Set it in Properties (Anchor X, Anchor Y, 0.5 and 0.5 = middle), drag the red dot in the viewport, or write hero.AnchorPoint = Vector2(0.5, 0.5)
- Added: animation frames of different sizes stay put around the anchor point, so an animation anchored in the middle plays from the middle
- Added: every property has an i with a hover explanation
- Added: scripts have Enabled and AutoStart (greyed out for main.zv). Disabled scripts are greyed out in the Explorer
- Changed: the starter games come with their own pictures in Assets and their objects already in the Workspace, so they show how a real project is built. Pong is now Paddle Ball
- Changed: a new dark look for the whole app, a flat menu bar, and Frames, Saved data and Updates open as tabs instead of extra windows
- Changed: the Properties panel and the Explorer have shorter, clearer texts

**Zorvo 0.0.7(26w44c)**
- Added: spritesheets and animations: open a picture, Frames and animations > Frames window to cut it into squares or draw your own frames, give every frame its own hitbox and make animations
- Added: in code, hero:Play("run"), hero:Stop(), hero.Frame, hero.FrameCount, hero.Playing, hero.Animation (Errors 46 and 47)
- Added: four new starter games: Highway Run, Space Shooter, Pong and Snake
- Added: the viewport can zoom (Ctrl + mouse wheel, + and - buttons, Fit to window) and scroll; F4 hides all panels; small screens start maximized
- Added: Run > Saved data shows everything save_data keeps (test and real), lets you edit, delete or clear it, and can start every test with empty saved data
- Changed: the docs have a version list, new features say which version they came in, and old commands are marked deprecated with the new way to do it
- Changed: the docs now show a working example for every key and mouse function
- Fixed: a stray box in the top left corner appeared when starting the game or pasting code

## Zorvo 0.0.7(26w44k) - 2026-10-26

- Added: Tween. box:Tween(transparency(1, 0, 1)) changes a property smoothly over time (x, y, width, height, rotation, transparency, saturation, edgeamount, hue), no bounce
- Added: Edges in Properties: Straight, Indent or Smooth, with an amount slider that only shows for Indent and Smooth
- Added: objects now turn around their anchor point, and the anchor dots and hitboxes can be shown or hidden above the viewport
- Added: Zorvo Settings (File menu) for the whole app, with automatic updates for full versions. Project Settings stay for one game
- Added: sprites have a Filter (Auto, Pixel or Smooth), and vector sprites are saved bigger so they are smooth instead of pixelated
- Added: vector sprites have a film strip for frames and animations
- Added: Hue now tints a picture, and the sliders have number boxes so you can type exact values
- Added: code suggestions for the objects in your Workspace and their properties, and you can click them
- Added: the thick green line on the loading picture moves while Zorvo starts
- Changed: the Properties panel updates in place and does not flash, and moving, turning and drawing are smoother
- Changed: the + list shows everything and greys out what cannot go there, and right-click Add opens the same list
- Changed: the starter games have comments that explain every part
- Changed: names are the same in Properties and in code, and a name with a space is written without it
- Removed: the gravity property and the set_gravity command (the Platformer and Duck Jumping make their own gravity)
- Fixed: the drawing editor keeps your tool after you draw, and the line you drag looks the same as the finished line

## Zorvo 0.0.7(26w44j) - 2026-10-26

- Added: new sprites can be Vector (shapes, smooth lines) or Pixel art, you pick when you add one
- Added: a Fill tool, live drawing while you drag, and Move forward 1 / Move back 1 for layers (greyed out when they cannot move)
- Added: icons on every tab, and when there are too many tabs they show just the icon
- Added: click a suggestion in the code list to use it, and the list scrolls when it is long
- Added: dragging an object out of the Workspace shows the blocked sign
- Changed: Frames, Saved data, Updates and the License pages open as tabs, and renaming is typed in the Explorer, so no extra windows
- Changed: the Updating window stays on screen with a Loading bar, and Zorvo comes to the front when it restarts
- Changed: Color is called Hue (Text Color for text), and in code it has no space: hue, textcolor
- Removed: the gravity property. The Platformer and Duck Jumping presets now do their own gravity in their script
- Fixed: Transparency and Saturation now show in the viewport
- Fixed: moving the viewport, scrolling code and the drawing editors are smooth (the scroll bars were slowing them down)
- Fixed: the viewport can be moved far in every direction, and the side panels in the drawing editors can be resized
- Fixed: line numbers appear at once when you press Enter
- Changed: the tab bar is grey instead of blue, and the animation panel is simpler

## Zorvo 0.0.7(26w44i) - 2026-10-26

- Added: vector drawing. Sprites are shapes now (rectangle, ellipse, line, pen, freehand) that you can move, resize and reorder, drawn smooth, no pixels
- Added: the command bar can change things, like explorer/workspace/object1.gravity = 1
- Added: drag scripts and sprites into any folder, and a blocked sign shows where you cannot drop
- Added: drop a picture on an object in the Explorer to give it that texture
- Changed: Play and Stop are only in the viewport, the top bar and Test in window are gone
- Changed: a game with an error in its code is reported at once instead of opening the window first
- Changed: an error while the game runs no longer freezes it
- Changed: changing Visible or Gravity no longer reloads the whole Properties panel, and Properties show less text
- Changed: the selection lines in the viewport are solid

## Zorvo 0.0.7(26w44h) - 2026-10-26

- Added: folders inside Scripts and Assets; drag a script or sprite onto a folder (or onto the list name to take it out)
- Added: + on the Scripts and Assets rows can make a folder
- Fixed: the pinned taskbar icon and the running Zorvo are one icon again (the pinned shortcut now always gets the same ID, and Zorvo Admin and Zorvo Kids shortcuts are left alone)

## Zorvo 0.0.7(26w44g) - 2026-10-26

- Added: a Loading your app... picture while Zorvo starts, and the restart after an update is faster
- Added: Texture picker in Properties with a search box, Import image, and drag a picture from Assets onto Properties
- Added: Transparency and Saturation sliders in Properties (also obj.transparency and obj.saturation in scripts)
- Added: new objects start as a grey placeholder box with an X
- Added: a picture follows your mouse while you drag things in the Explorer
- Changed: naming a new folder, sprite or script is typed right in the Explorer, no popup window
- Changed: hidden objects are fully hidden in the viewport
- Changed: the Projects window has a fixed size, because maximized it looked stretched
- Fixed: the viewport no longer snaps while you move around

## Zorvo 0.0.7(26w44f) - 2026-10-26

- Added: Play and Stop right inside the viewport (Play button, F5), plus a Test in window button for final testing
- Added: drag a picture from Windows onto the Explorer to make a sprite, or onto the drawing editor to put it in
- Added: a + on the Workspace, Scripts and Assets rows, and Object in the + menu
- Added: in the drawing editor, drag the selected area and it follows your mouse
- Changed: hidden objects show faded in the viewport
- Changed: the Made with Zorvo credit only shows in exported games
- Changed: Export menu just says .exe and .dmg
- Fixed: pressing Enter after if ... then now adds end, also inside a func
- Fixed: less lag when typing code, zooming and moving things in the viewport

## Zorvo 0.0.7(26w44e) - 2026-10-26

- Changed: Back to the earlier light look: light panels, the normal menu bar, and Frames, Saved data and Updates open in their own windows again
- Kept: the (i) help buttons, anchor point, Enabled and AutoStart for scripts, presets with real scenes
- Added: Visible and Gravity properties for every object (with (i) help)

## Zorvo 0.0.7(26w44d) - 2026-10-26

- Added: anchor points. Every object has an anchor point (default 0, 0 = top left, so old games are unchanged). x and y are where the anchor is. Set it in Properties (Anchor X, Anchor Y, 0.5 and 0.5 = middle), drag the red dot in the viewport, or write hero.AnchorPoint = Vector2(0.5, 0.5)
- Added: animation frames of different sizes stay put around the anchor point, so an animation anchored in the middle plays from the middle
- Added: every property has an i with a hover explanation
- Added: scripts have Enabled and AutoStart (greyed out for main.zv). Disabled scripts are greyed out in the Explorer
- Changed: the starter games come with their own pictures in Assets and their objects already in the Workspace, so they show how a real project is built. Pong is now Paddle Ball
- Changed: a new dark look for the whole app, a flat menu bar, and Frames, Saved data and Updates open as tabs instead of extra windows
- Changed: the Properties panel and the Explorer have shorter, clearer texts

## Zorvo 0.0.7(26w44c) - 2026-10-26

- Added: spritesheets and animations: open a picture, Frames and animations > Frames window to cut it into squares or draw your own frames, give every frame its own hitbox and make animations
- Added: in code, hero:Play("run"), hero:Stop(), hero.Frame, hero.FrameCount, hero.Playing, hero.Animation (Errors 46 and 47)
- Added: four new starter games: Highway Run, Space Shooter, Pong and Snake
- Added: the viewport can zoom (Ctrl + mouse wheel, + and - buttons, Fit to window) and scroll; F4 hides all panels; small screens start maximized
- Added: Run > Saved data shows everything save_data keeps (test and real), lets you edit, delete or clear it, and can start every test with empty saved data
- Changed: the docs have a version list, new features say which version they came in, and old commands are marked deprecated with the new way to do it
- Changed: the docs now show a working example for every key and mouse function
- Fixed: a stray box in the top left corner appeared when starting the game or pasting code

## Zorvo 0.0.7 - 2026-10-26

- Fixed: when the update check fails, File > Updates now lists every way it tried and a plain-words reason (antivirus, firewall, proxy, no internet)
- Fixed: update checks and downloads also work behind firewalls and antivirus (falls back to curl and PowerShell)

### Also new since the last full version (from the snapshots)

**Zorvo 0.0.6(26w44b)**
- Added: player.Parent = Explorer/scene (or nothing, or another object); children move with their parent
- Added: Explorer/... in scripts works with any capital letters
- Added: you can scroll and pan around the viewport (mouse wheel, Shift+wheel, middle or right mouse drag, Home)
- Fixed: checking for and downloading updates now also works when a firewall, antivirus or proxy blocks Python (falls back to curl and PowerShell)
- Fixed: downloaded updates are checked and unblocked so Windows does not stop them

**Zorvo 0.0.6(26w44a)**
- Fixed: File > Updates showed a blank window when the update check failed; it now shows the reason and a Try again button

**Zorvo 0.0.6(26w43za)**
- Added: four new starter games that really play: Coin Collector (now with movement, score and best score), Platformer, Duck Jumping and Clicker Game
- Changed: the update popup at launch now only offers full versions, never snapshots (File > Updates still lists them)
- Changed: the docs moved to chromovia.com/docs, with light and dark mode, instant chapters and a new look
- Changed: snapshot letters continue after z with za, zb, zc and so on

**Zorvo 0.0.6(26w43z)**
- Added: if, elif (or elseif, else if) and else, plus while, for, repeat, break and continue are back
- Added: lists [1, 2, 3] and dicts {name = "Bo"} with actions like append, pop, sort, keys, has, upper, split and replace
- Added: math and random functions (abs, min, max, round, sqrt, clamp, lerp, random_int, PI ...), // and ** operators, default values for function values, Vector2
- Added: type a key name or sound name inside key_pressed(), key_down() and play_sound() and the popup suggests them
- Added: the Zarv# docs explain every word, symbol and function in detail, with a new flatter design
- Changed: color previews follow the text instantly while you scroll, and can be turned off in Project settings
- Changed: mistakes are no longer underlined while you type; they show in the Terminal when you test the game

**Zorvo 0.0.6(26w43y)**
- Fixed: Zorvo showed two taskbar buttons (one for the shortcut or pinned icon and one for the open window). Shortcuts now share the window's taskbar ID, also ones you pinned before. If it still shows two once, close Zorvo and open it again from the pinned icon

**Zorvo 0.0.6(26w43x)**
- Added: Circle, Rectangle and Triangle: draw shapes without picture files (their hitboxes fit the shape)
- Added: Button(text, x, y, w, h) with an on_click(button) function, plus clicked, hovered, enabled and visible
- Added: key_pressed, key_released, mouse_pressed and mouse_released fire once per press; clicks also work as taps on touch screens
- Added: show_hitboxes(true) shows hitboxes (red while touching) and logs when things touch; also a project setting
- Added: destroy_all, sprite_count, exists, and vx, vy, gravity on every object; an old variable can no longer control a new object with the same name
- Added: play_sound("flap"), "score", "hit", "click" and "pause" are built in, no files needed
- Added: Project settings is the first item in the Explorer (also View > Project settings); settings that cannot change, like the preset, are greyed out
- Added: a Game Tools chapter in the Zarv# docs
- Fixed: updates showed "No changelog provided"; the notes now always show

**Zorvo 0.0.6(26w43w)**
- Fixed: Zorvo now uses one taskbar button for the Projects window, the editor and the test game, also when pinned (re-pin Zorvo once if you had it pinned before)

**Zorvo 0.0.6(26w43v)**
- Added: Assets/player.png (or Explorer/Assets/player.png or /player) with :Clone(x, y) to put a picture into the game from code; :Destroy() removes a copy
- Added: TextLabel fonts (three built in with bold and italic, import and delete your own), outline, and gradients with several colors (also from code: Properties(outline), Properties(gradient) = Gradient(...))
- Added: HasHitbox on text and sprites (Properties and in code)
- Added: Scripts can be switched off in Properties so they never run
- Added: Scale the game to the window setting in Game properties (on by default)
- Added: A round rotate arrow on selected objects; resizing a TextLabel now scales its letters
- Changed: The Workspace no longer has Add object (use Assets/...:Clone or a TextLabel); the starter project clones its pictures in code
- Changed: The usage log also sends the computer name, how long the app was open and how often features were used (Privacy Policy updated)
- Fixed: Small startup bugs in the new usage counters

## Zorvo 0.0.6(26w44b) - 2026-10-26

- Added: player.Parent = Explorer/scene (or nothing, or another object); children move with their parent
- Added: Explorer/... in scripts works with any capital letters
- Added: you can scroll and pan around the viewport (mouse wheel, Shift+wheel, middle or right mouse drag, Home)
- Fixed: checking for and downloading updates now also works when a firewall, antivirus or proxy blocks Python (falls back to curl and PowerShell)
- Fixed: downloaded updates are checked and unblocked so Windows does not stop them

## Zorvo 0.0.6(26w44a) - 2026-10-26

- Fixed: File > Updates showed a blank window when the update check failed; it now shows the reason and a Try again button

## Zorvo 0.0.6(26w43za) - 2026-10-25

- Added: four new starter games that really play: Coin Collector (now with movement, score and best score), Platformer, Duck Jumping and Clicker Game
- Changed: the update popup at launch now only offers full versions, never snapshots (File > Updates still lists them)
- Changed: the docs moved to chromovia.com/docs, with light and dark mode, instant chapters and a new look
- Changed: snapshot letters continue after z with za, zb, zc and so on

## Zorvo 0.0.6(26w43z) - 2026-10-25

- Added: if, elif (or elseif, else if) and else, plus while, for, repeat, break and continue are back
- Added: lists [1, 2, 3] and dicts {name = "Bo"} with actions like append, pop, sort, keys, has, upper, split and replace
- Added: math and random functions (abs, min, max, round, sqrt, clamp, lerp, random_int, PI ...), // and ** operators, default values for function values, Vector2
- Added: type a key name or sound name inside key_pressed(), key_down() and play_sound() and the popup suggests them
- Added: the Zarv# docs explain every word, symbol and function in detail, with a new flatter design
- Changed: color previews follow the text instantly while you scroll, and can be turned off in Project settings
- Changed: mistakes are no longer underlined while you type; they show in the Terminal when you test the game

## Zorvo 0.0.6(26w43y) - 2026-10-25

- Fixed: Zorvo showed two taskbar buttons (one for the shortcut or pinned icon and one for the open window). Shortcuts now share the window's taskbar ID, also ones you pinned before. If it still shows two once, close Zorvo and open it again from the pinned icon

## Zorvo 0.0.6(26w43x) - 2026-10-25

- Added: Circle, Rectangle and Triangle: draw shapes without picture files (their hitboxes fit the shape)
- Added: Button(text, x, y, w, h) with an on_click(button) function, plus clicked, hovered, enabled and visible
- Added: key_pressed, key_released, mouse_pressed and mouse_released fire once per press; clicks also work as taps on touch screens
- Added: show_hitboxes(true) shows hitboxes (red while touching) and logs when things touch; also a project setting
- Added: destroy_all, sprite_count, exists, and vx, vy, gravity on every object; an old variable can no longer control a new object with the same name
- Added: play_sound("flap"), "score", "hit", "click" and "pause" are built in, no files needed
- Added: Project settings is the first item in the Explorer (also View > Project settings); settings that cannot change, like the preset, are greyed out
- Added: a Game Tools chapter in the Zarv# docs
- Fixed: updates showed "No changelog provided"; the notes now always show

## Zorvo 0.0.6(26w43w) - 2026-10-25

- Fixed: Zorvo now uses one taskbar button for the Projects window, the editor and the test game, also when pinned (re-pin Zorvo once if you had it pinned before)

## Zorvo 0.0.6(26w43v) - 2026-10-25

- Added: Assets/player.png (or Explorer/Assets/player.png or /player) with :Clone(x, y) to put a picture into the game from code; :Destroy() removes a copy
- Added: TextLabel fonts (three built in with bold and italic, import and delete your own), outline, and gradients with several colors (also from code: Properties(outline), Properties(gradient) = Gradient(...))
- Added: HasHitbox on text and sprites (Properties and in code)
- Added: Scripts can be switched off in Properties so they never run
- Added: Scale the game to the window setting in Game properties (on by default)
- Added: A round rotate arrow on selected objects; resizing a TextLabel now scales its letters
- Changed: The Workspace no longer has Add object (use Assets/...:Clone or a TextLabel); the starter project clones its pictures in code
- Changed: The usage log also sends the computer name, how long the app was open and how often features were used (Privacy Policy updated)
- Fixed: Small startup bugs in the new usage counters

## Zorvo 0.0.6 - 2026-10-25

- Added: Polygon hitboxes (round or precise shapes) and a smarter Fill in the sprite editor
- Added: TextLabel, RGB with a color picker, /picture_name shortcuts, smarter autocomplete, red error underline after 5 seconds idle
- Changed: Zarv# was stripped back to a small core to be rebuilt step by step (func, var, gvar, numbers, text, booleans)
- Changed: Documentation moved to the online Zarv# book at chromovia.com/docs/zarv
- Added: Anonymous usage log (can be switched off in the File menu); Terms and Privacy Policy updated

### Also new since the last full version (from the snapshots)

**Zorvo 0.0.5(26w43u)**
- Removed: Most of the Zarv# language was stripped so it can be rebuilt step by step. What stays: func, return, var, gvar, numbers, text, booleans, nothing, math, comparisons, and/or/not, print, int, float, str, len, RGB, /asset names, workspace + Properties (TextLabel). if, while, for, repeat, lists, Vector2 and all game commands are gone for now (using one gives Error 17)
- Changed: The starter project script is now tiny; autocomplete only suggests what exists
- Changed: Update check errors now say exactly why a check failed (GitHub API and release feed), and are added to the usage log
- Changed: The Zarv# book on chromovia.com matches the new language

**Zorvo 0.0.5(26w43t)**
- Added: Sprite editor Fill now stops exactly at lines (fills only the inside of a drawn circle, no leaking through diagonal gaps)
- Added: Polygon hitboxes: drag corners, click a line to add a corner, right-click a corner to remove it, plus Round it (ellipse) and Follow the outline buttons
- Added: TextLabel in the Explorer + menu; label.Properties(text) = "Hi" and label.Properties(color) = RGB(255, 2, 205)
- Added: RGB(r, g, b) with a color picker square beside it in the code editor
- Added: /cat_picture and /"cat picture" shortcuts for pictures in Assets (Error 42 if missing)
- Added: Autocomplete for explorer/ paths and / pictures; accepting a func name writes (); typing ( writes () with the cursor in the middle; Enter after func/if/while/for/repeat writes the end
- Added: After 5 seconds without typing the editor underlines the line with a mistake in red
- Added: Anonymous usage log (File > Share anonymous usage data turns it off); Terms and Privacy Policy updated
- Added: The launch update popup also offers a newer snapshot when you run a snapshot
- Changed: gvar can only be created at the top of a script and funcs can only read it (Error 19 and 39)
- Changed: The Docs tab now points to the online Zarv# book; the built-in documentation was removed
- Changed: Game preview shows the Made with Zorvo credit first; errors only appear in the Terminal
- Fixed: explorer/assets/... pictures failed to load
- Fixed: Stopping a game sometimes left its window open
- Fixed: After an update from inside a project, Zorvo reopens that project

**Zorvo 0.0.5(26w43s)**
- Changed: Sprite editor side panel redesigned with a 'Sprite Editor' header
- Added: Every group in the sprite editor (Tools, Color, View, Hitbox, Crop and size, Edit) can be collapsed, so no more scrolling for tools

## Zorvo 0.0.5(26w43u) - 2026-10-25

- Removed: Most of the Zarv# language was stripped so it can be rebuilt step by step. What stays: func, return, var, gvar, numbers, text, booleans, nothing, math, comparisons, and/or/not, print, int, float, str, len, RGB, /asset names, workspace + Properties (TextLabel). if, while, for, repeat, lists, Vector2 and all game commands are gone for now (using one gives Error 17)
- Changed: The starter project script is now tiny; autocomplete only suggests what exists
- Changed: Update check errors now say exactly why a check failed (GitHub API and release feed), and are added to the usage log
- Changed: The Zarv# book on chromovia.com matches the new language

## Zorvo 0.0.5(26w43t) - 2026-10-25

- Added: Sprite editor Fill now stops exactly at lines (fills only the inside of a drawn circle, no leaking through diagonal gaps)
- Added: Polygon hitboxes: drag corners, click a line to add a corner, right-click a corner to remove it, plus Round it (ellipse) and Follow the outline buttons
- Added: TextLabel in the Explorer + menu; label.Properties(text) = "Hi" and label.Properties(color) = RGB(255, 2, 205)
- Added: RGB(r, g, b) with a color picker square beside it in the code editor
- Added: /cat_picture and /"cat picture" shortcuts for pictures in Assets (Error 42 if missing)
- Added: Autocomplete for explorer/ paths and / pictures; accepting a func name writes (); typing ( writes () with the cursor in the middle; Enter after func/if/while/for/repeat writes the end
- Added: After 5 seconds without typing the editor underlines the line with a mistake in red
- Added: Anonymous usage log (File > Share anonymous usage data turns it off); Terms and Privacy Policy updated
- Added: The launch update popup also offers a newer snapshot when you run a snapshot
- Changed: gvar can only be created at the top of a script and funcs can only read it (Error 19 and 39)
- Changed: The Docs tab now points to the online Zarv# book; the built-in documentation was removed
- Changed: Game preview shows the Made with Zorvo credit first; errors only appear in the Terminal
- Fixed: explorer/assets/... pictures failed to load
- Fixed: Stopping a game sometimes left its window open
- Fixed: After an update from inside a project, Zorvo reopens that project

## Zorvo 0.0.5(26w43s) - 2026-10-25

- Changed: Sprite editor side panel redesigned with a 'Sprite Editor' header
- Added: Every group in the sprite editor (Tools, Color, View, Hitbox, Crop and size, Edit) can be collapsed, so no more scrolling for tools

## Zorvo 0.0.5 - 2026-10-24

- Added: Zarv# has its own logo (Docs tab header and script icon)
- Added: drag a picture from Assets onto the viewport to place it in the scene
- Added: full Zarv# reference manual online at chromovia.com/docs/zarv
- Changed: the installer and app are now built with a freshly compiled bootloader, so Windows Defender no longer flags them (the old build was blocked on some PCs)
- Changed: Docs welcome page links to the online manual

## Zorvo 0.0.4(26w43r) - 2026-10-24

- Added: Zarv# has its own logo (Docs tab header and script icon)
- Added: full Zarv# reference manual online at chromovia.com/docs/zarv
- Changed: Docs welcome page links to the online manual

## Zorvo 0.0.4 - 2026-10-24

- Added: macOS version (download on chromovia.com)
- Fixed: update check no longer hangs on Fetching update...
- Fixed: Python icon when testing a game; test window title ends with Made with Zorvo
- Fixed: typing in the script editor was laggy

## Zorvo 0.0.3(26w43q) - 2026-10-24

- Fixed: typing in the script editor was laggy (colouring now runs once typing pauses and is much faster on long scripts)

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

