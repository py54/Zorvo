# Zorvo Kids changelog

## 0.3.2 - 2026-10-26

- Fixed: updating now also works when a firewall, antivirus or proxy blocks the app's own connection (it falls back to curl and PowerShell, like Zorvo does).
- Fixed: the update check asks for up to 200 releases and, if the list cannot be reached, looks for the next version by its download address. Before, Zorvo Kids could stop seeing its own updates once Zorvo had published many releases.
- Fixed: a failed update check or download leaves a short note in zorvokids_update.log (in your temp folder) saying why, instead of failing silently.
- Fixed: a downloaded update is unblocked so Windows SmartScreen does not stop it.

## 0.3.1 - 2026-10-25

- Changed: the tour (Show me how!) has a spotlight now. The whole screen goes dark except the thing to look at or tap. It zooms up, gets a pulsing red circle and a bouncing arrow, and a big speech bubble with a voice explains it. Tapping the lit spot works like tapping the real thing. The name page has it too.
- Changed: scrolling the bricks and the category buttons is smooth now (it eases, and only the list moves).
- Fixed: the group headings in the palette (like START THE GAME) were hidden behind the start bricks.
- Added: when an update has been downloaded while the app is open, a popup asks "A new Zorvo Kids is ready! Update now?" Update now saves your game, closes, installs the update and opens the new version. Later asks again in half an hour.

## 0.3.0 - 2026-10-25

- Added: Math. Drag a little calculation brick (2 + 3, random, bigger of...) into any number box, even inside another calculation. Tapping a calculation puts it in the chosen brick.
- Added: Sensing. Bricks that give back a number: my x, my y, my size, mouse x and y, distance to, timer, score and variables.
- Added: more bricks (64 now): glide, point, slide left and down, make smaller, repeat until touching, wait for a key, send and get messages, a random number, if numbers compare and more.
- Added: the backdrop is its own thing. Tap Backdrop (or an empty spot on the stage) to draw it on a wide canvas and give it its own code. It updates right away.
- Added: variables stay hidden until you show them. Tap the eye next to a variable, or use the new Show variable and Hide variable bricks. Drag a shown variable anywhere on the stage.
- Added: full screen. The Full screen button (or F11) fills your screen, and Play big runs your game on a stage that fills the whole screen (Esc comes back).
- Added: you can pick up and move sprites by hand while the game runs.
- Changed: the tour (Show me how!) was remade. It starts by naming your game and then shows the stage, the game name, the bricks, Go, Stop, Voice, Draw and Home, with a Next button and a voice.
- Changed: bricks, buttons and sprites are drawn smooth (no jagged edges), and every brick has a name under it in your pile too.
- Changed: the category list scrolls, the palette has a scroll bar, and the bricks are grouped with headings, so nothing is cut off any more.
- Changed: the self-update checks every few hours, checks the download, finishes an update that did not get installed the next time you open the app, and says Updated! on the home page.

## 0.2.0 - 2026-10-25

- Added: vector drawing. Sprites are now drawings made of shapes and lines (no more pixels), with a huge drawing canvas, pencil, line, box, circle, triangle and star tools, color it, move, erase, undo and redo.
- Added: drag a picture file (png, jpg, gif, bmp, webp) onto the window to make a new sprite from it, or use Add image. You can draw on top of it.
- Added: variables. Make your own (like points or lives), then set them, change them, compare them and say them. They show on the stage.
- Added: 12 sprites to pick from, all redrawn as vectors, and a new example (Count the Clicks).
- Changed: bricks that are inside a loop now sit inside a clear frame, so you can see they are held by it.
- Changed: the bricks in each group are organized with headings (Walk, Slide, Jump to a spot, Talk, Size, Loops, Ask a question...).
- Changed: "pictures" are now called "sprites". Old games open fine: their pixel pictures turn into vector sprites.

## 0.1.0 - 2026-10-25

The whole app was rebuilt for young kids.

- Added: icon bricks. Every brick is a big picture (an arrow, a flag, a speech bubble...) so you do not have to read. They sit side by side like a train of Lego bricks and wrap to the next row.
- Added: tap a brick on the left to add it. New bricks go after the brick you picked, or inside a loop you picked. Dragging still works, and the others slide over to show where it will snap.
- Added: tap a brick in your pile to try it right away. Bricks glow while the game runs.
- Added: a little card under the picked brick with big minus and plus buttons for its numbers, big choice buttons (keys, sounds, backdrops) and Try, Copy and Throw away buttons.
- Added: "Show me how!" is a step by step guide that makes a first game, with a blinking ring and a voice.
- Added: the Voice reads bricks out loud.
- Added: a picture chooser and a backdrop chooser with big pictures, a bouncing cube on the home page, and a clear message when you press Go! without a Start brick.
- Changed: the picture you work on has a dashed frame on the stage. The stage and the drawing area use the room of big screens.
- Changed: loops have a little end brick and a bar under everything inside them.

## 0.0.4 - 2026-10-25

- Added: tap a brick to add it. No dragging needed (dragging still works).
- Added: tap a brick in your pile to try it right away on the stage.
- Added: the app reads bricks out loud for kids who cannot read yet (Voice button, on by default).
- Added: number boxes have little arrows to make the number smaller or bigger.
- Added: a 4 step guide on an empty game.
- Changed: much bigger bricks, buttons and text, and a bigger stage on big screens.

## 0.0.3 - 2026-10-25

- Added: an installer (ZorvoKidsSetup.exe) with a desktop shortcut and an uninstall entry in Windows Apps. Updates keep working by themselves.
- Added: Lego-style bricks with studs. They click together, pop down when they snap, and show where they will snap while you drag.
- Added: name your game when you make it, and a loading screen when it starts or opens.
- Added: new games start empty with one Cube picture.
- Added: two new bricks (go to the mouse, if the mouse is pressed) and two new examples (Pet the Cat, Follow the Mouse).
- Changed: the first brick now says "when game starts". New look with chunky 3D buttons, round category buttons and example cards.

## 0.0.2 - 2026-10-25

- Added: Zorvo Kids now updates itself. It downloads new versions quietly and installs them when you close the app.
- Changed: new logo, a mini Zorvo hexagon in rainbow colors.

## 0.0.1 - 2026-10-25

- Added: Zorvo Kids, a colorful block-coding app for kids. Drag blocks, draw your own pictures, make games.
- Added: four example games, built-in pictures, sounds and a score.
