# Modes

VIM is a mode-based editor.

* Normal Mode (default)
* Insert Mode (similar to what most people are used to)
* Command Mode
* Visual Mode
* Replace Mode
* (ex mode)

## Normal Mode

### Motion

* use H J K L (try to move your cursor HERE)
  * H = left
  * L = right (easy to remember amirite.jpg)
  * J = down (= jump)
  * K = up (= kill)
* never use arrow keys, because it reduces efficiency

### Advanced motions

* {, } for paragraphs (move your cursor after this paragaph)
* Ctlr + U / Ctrl + D for moving to the next "page" (go to the next page and back)
* b, e for Beginning and End of word (move to the B of Beginning)
* Ctrl + O for last position
* gg, G for beggggginning and end of buffer (go there and come back with Ctrl + O)
* 50gg to go to line 50 (go there and come back)
* $ to go to end of line, 0 to go to beginning of line (go to the beginning of the line)
* :help motion.txt

### Repeat motions

* use 20j to jump 20 lines
* use repeat with many other motions

## Insert Mode

In normal mode:
* press i to go to insert mode before cursor, a to go to insert mode after cursor
* I to move to the beginning of the line, A to move to the end of the line
* o opens a newline below and O one above

Write your name HERE. And after the colon:
Fit a newline between this and the previous line and write your username.

BACK TO NORMAL: Press ESC

**Generally do your editing and then go back to normal mode. Don't move around in
insert mode.**

## Undo and redo

NICE!

In normal mode: use u and Ctrl + r to undo and redo. Undos/redos last action in
insert mode or last operator executed.

## Operators

Combined with motion this is where the magic happens:

operator + motion

In normal mode:

* d to delete, d MOTION to delete everything under your motion

Delete this line.
Delete the first sentence. But let the second one live.

* c to change

Another motion is inner word or iw.

Change ‘phikes’ in the next line to your name using a motion.
I am phikes. Hi, I am dad.

### Shortcuts

* dd to delete line
* cc to change line

## Command Mode

In normal mode write commands by typing a colon, e.g. :quit or :write (or :q and :w or :wq)

## Visual Mode

Make visual selections and apply operators. In normal mode: Use v for character
based visual mode and V for line based.

Use motions to modify your selection. Select this block visually and delete it.

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
culpa qui officia deserunt mollit anim id est laborum.

## Replace Mode

Replace mode is a special insert mode where characters under the cursor are written over.
Enter single character replace mode with r and replace mode with R.

Replace the extension of this file with “.jpg”: replace_me.png

## Searching

Use / to search for text in the current buffer. Use n/N to jump between results.
Use :noh to turn off the highlight again

## Search and replace

Use :%s/OLD/NEW/g to replace in current buffer (OLD is a regex) or :s/OLD/NEW/g
to replace occurences on the current line.

Replace every OLD on the second line in the next paragraph with NEW

OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD
OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD
OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD
OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD
OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD OLD

## Bonus motions

* t/T jumps BEFORE the next or previous occurence of the following character. (e.g. tA jumps to this A)
* f/F is like t/T but jump ON the character

## Copy/Paste

* yy for the whole line (works with motions as well, so y + Motion) to copyyyyy (or yyyyank)
* p for pasting (if you copied a line-ending use P to paste above)

Copy me until the dot. And paste me after the colon:
