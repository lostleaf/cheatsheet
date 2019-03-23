*Mostly copied from [Derek Wyatt's Tutorial](http://derekwyatt.org/vim/tutorials/index.html)*

**Basic movement** - Character-wise movements: `h`, `j`, `k` and `l`

**Line terminus** 
- Beginning of line: `^`;
- First non-blank: `0`
- End of line: `$`

**word** - A sequence of characters in the 'iskeyword' class(`()[],-` and whitespace etc)

**WORD** - A sequence of characters separated by whitespace

**Forward word movement** - Move to the beginning(end) of next word: `w`(`e`), and WORD: `W`(`E`)

**Backward word movement** - Move backward to the beginning(end) of pervious word: `b`(`ge`), and WORD: `B`(`gE`)

**Move to character** 
- Move forward to *{char}*: `f*{char}*`, and `F` backward
- Move forward to the character just before *{char}*: `t*{char}*`, and `T` backward after
- `;` to repeat and `,` to repeat backwards

**Paging** 
- Full page forward and backward: `CTRL-f` and `CTRL-b`
- Half page forward and backward: `CTRL-u` and `CTRL-d`

**Scroll** - Scroll one line: `CTRL-y` and `CTRL-e`

**Cursor jumping** 
- Head, middle and last line of a screen: `H`, `M` and `L`
- Top and Bottom: `gg` and `G`

**Jumping to a particular line** - `(number)G` or `:(number)`

**Seach current word** - `*` and `#`, or `g*` and `g#` with no word bounds(E.g. 'app' in 'apple')

**Regular expression searching** - `/` and `?`. Repeat next and pervious: `n` and `N`

**Start of Function or Class Jumping** - Beginning of previous* and *next* functions or classes: `[[` and `]]`

**End of Function or Class Jumping** - *Forwards* and *backwords* to the end of a function or class: `][` and `[]`

**Jumping to Matching Braces** - `%`

**Marks**
- Set mark *{char}* at current cursor location: `m*{char}*`
- Jump to line of mark *{char}*: `'*{char}*` (first non-blank character in line)
- Jump to position of mark *{char}*: <code>\`*{char}*</code> (line and column)
- List all marks: `:marks`

**Insert** - Insert before the current character: `i`. Insert at the beginning of the line: `I`(equals to `^i`)

**Append** - Insert **after** the current character: `a`. Insert at the end of the line: `A`(equals to `$a`)

**Insert a New Line** - Insert a new line after the current: `o`, and `O` before

**Replacing** 
- Replace the character under cursor: `r`
- Switch to replace mode: `R`
- Change things: `c + <text object>` or `c + <motion>`. 
- Change the current whole line: `cc` (equals to `^c$`)
- Change from the current character to the end of the line: `C` (equals to `c$`)

**Deleting** 
- Delete a single character under the cursor: `x`, `X` before the cursor
- Delete things: `d + <text object>` or `d + <motion>`
- Delete the current whole line: `dd` 
- Delete from the current character to the end of the line: `D`

**Repeat** - Repeat the last command: `.`

**Yanking(copying)** 
- Copy things: `y + <text object>`
- Copy the current whole line: `yy`

**Pasting** - Paste after the cursor `p`, and `P` before

**Joining** - Join lines: `J`, `gJ` without extra spaces

**Visual Selection** 
- Character-wise visual selection: `v` 
- Line-wise selection: `V` 
- Block-mode selection `ctrl-v`
- Re-select an area just selected: `gv`
