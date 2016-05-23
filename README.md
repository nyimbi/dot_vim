# dot_vim
== my .vim setup ==
to use 
git clone https://github.com/nyimbi/dot_vim.git ~/.vim

optimized for editing LaTeX sources, node, typescript, python and other programming languages.

I have adapted ProVim setting and added a couple of bundles vim-latex etc


Here is a really great synopsis of how to use Vim
http://stackoverflow.com/questions/5400806/what-are-the-most-used-vim-commands-keypresses?lq=1


General
* Nearly all commands can be preceded by a number for a repeat count. eg. 5dd delete 5 lines
* <Esc> gets you out of any mode and back to command mode
* Commands preceded by : are executed on the command line at the bottom of the screen
* :help help with any command
Navigation
* Cursor movement: ←h ↓j ↑k l→
* By words:
    * w next word (by punctuation); W next word (by spaces)
    * b back word (by punctuation); B back word (by spaces)
    * e end word (by punctuation); E end word (by spaces)
* By line:
    * 0 start of line; ^ first non-whitespace
    * $ end of line
* By paragraph:
    * { previous blank line; } next blank line
* By file:
    * gg start of file; G end of file
    * 123G go to specific line number
* By marker:
    * mx set mark x; 'x go to mark x
    * '. go to position of last edit
    * ' ' go back to last point before jump
* Scrolling:
    * ^F forward full screen; ^B backward full screen
    * ^D down half screen; ^U up half screen
    * ^E scroll one line up; ^Y scroll one line down
    * zz centre cursor line
Editing
* u undo; ^R redo
* . repeat last editing command
Inserting
All insertion commands are terminated with <Esc> to return to command mode.
* i insert text at cursor; I insert text at start of line
* a append text after cursor; A append text after end of line
* o open new line below; O open new line above
Changing
* r replace single character; R replace multiple characters
* s change single character
* cw change word; C change to end of line; cc change whole line
* c<motion> changes text in the direction of the motion
* ci( change inside parentheses (see text object selection for more examples)
Deleting
* x delete char
* dw delete word; D delete to end of line; dd delete whole line
* d<motion> deletes in the direction of the motion
Cut and paste
* yy copy line into paste buffer; dd cut line into paste buffer
* p paste buffer below cursor line; P paste buffer above cursor line
* xp swap two characters (x to delete one character, then p to put it back after the cursor position)
Blocks
* v visual block stream; V visual block line; ^V visual block column
    * most motion commands extend the block to the new cursor position
    * o moves the cursor to the other end of the block
* d or x cut block into paste buffer
* y copy block into paste buffer
* > indent block; < unindent block
* gv reselect last visual block
Global
* :%s/foo/bar/g substitute all occurrences of "foo" to "bar"
    * % is a range that indicates every line in the file
    * /g is a flag that changes all occurrences on a line instead of just the first one
Searching
* / search forward; ? search backward
* * search forward for word under cursor; # search backward for word under cursor
* n next match in same direction; N next match in opposite direction
* fx forward to next character x; Fx backward to previous character x
* ; move again to same character in same direction; , move again to same character in opposite direction
Files
* :w write file to disk
* :w name write file to disk as name
* ZZ write file to disk and quit
* :n edit a new file; :n! edit a new file without saving current changes
* :q quit editing a file; :q! quit editing without saving changes
* :e edit same file again (if changed outside vim)
* :e . directory explorer
Windows
* ^Wn new window
* ^Wj down to next window; ^Wk up to previous window
* ^W_ maximise current window; ^W= make all windows equal size
* ^W+ increase window size; ^W- decrease window size
Source Navigation
* % jump to matching parenthesis/bracket/brace, or language block if language module loaded
* gd go to definition of local symbol under cursor; ^O return to previous position
* ^] jump to definition of global symbol (requires tags file); ^T return to previous position (arbitrary stack of positions maintained)
* ^N (in insert mode) automatic word completion

