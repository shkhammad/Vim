# Vim Commands

Vim has three modes namely **normal, insert** and **visual**.

In Windows, we have **Windows Subsystem for linux (WSL)**, where we can access Vim.

To access Vim, we can type **vim** on the terminal emulator. This opens the Vim editor.

Initially, we have **normal** mode which can be used to **delete** and **traverse** through the document (but not **write**).

To start **editing** (inserting) we can type **i** to go into the **insert** mode and start editing the document.

Since this creates a new file we have to name the file first before saving we can type **:w (file).(extension)** to name the file. Then to save, we can use **:wq** this saves and exits the Vim editor.

We use **vim (file)** to open vim with the given filename. If the file exists in the given directory it will open that file else new file will be created and we have to give the filename.

Below, **n** may be substituted with any integer

| Command | Description |
| - | - |
| `:q` | Exits vim directly |
| `:wq` | Save (file) and exit  |
| `:q!` | Exit without saving |
| esc | Exits current mode |
| `:w (file).(extension)` | Name a file |
| h | Traverses leftwards character by character |
| j | Traverses downwards character by character |
| k | Traverses upwards character by character |
| l | Traverses rightwards character by character |
| `ndd` | Deletes **n** line or lines (also cuts the line)|
| `ndw` | Deletes **n** word or words |
| `nx` | Deletes **n** character or characters |
| `nu` | Do **n** undo or undo's |
| `: set number` | Show line numbers |
| `:(line)` | Goes to the given line number |
| `gg` | Top of the document |
| shift + g | End of the document |
| `nw` | Traverses **n** word by word (fast traversing) |
| `nb` | Same as above but in **reverse** direction |
| `p` | Paste (line) |
| `dd` | Cut (line) |
| `nce` | Deletes a word or words and jumps into **insert** mode for editing |
| `c$` | Deletes entire line and jumps into **insert** mode for editing |
| `yy` | Copy (line) |
| `y$` | Copies from cursor to the end (line) |
| `v` | Goes in visual mode where we can select the text using &#8593; / &#8595; and then press d / y to cut / copy, then it will jump to normal mode where we can paste using `p` |
| `/(word)` + enter | Searches the given word, for next press **n** and for previous press **N** |
| `r(letter)` | Replaces the cursor (letter) with the given letter |
| `:split (file)` | Splits the screen horizontally and open a file with the given name if it exists in the same directory |
| `:vsplit (file)` | Same as above but splits it vertically |
| ctrl + `ww` | Switches files |
| 0 | Start (line) |
| `f(character)` | Jumps to the given character in the line |
| `F(character)` | Same as above but in reverse direction |
| A | Jumps the cursor to the end (line) and goes into **insert** mode for editing |
| s | Deletes the character (cursor) and goes into **insert** mode for editing|
| s | Start (line) |
| S | Deletes the line and goes into **insert** mode for editing |
| o | Creates a new line below the current line and goes into **insert** mode for editing |
| O | Creates a new line above the current line and goes into **insert** mode for editing |
| `d$` | Deletes from cursor to the end (line) |
| % | Searches **( )** in a line |
| `:%s/(old)/(new)/g` | Replaces old word with the new word in the document |
| `:%s/(old)/(new)/gc` | Same as above but with prompts |
| `:recover` | Recovers accidentally deleted file |
|`vim (file) (file)` | Opens two files (side-by-side) if they both exists in the same directory. Use **:n** for next and **:prev** for previous|
| ctrl + d | Checks if the command is **valid** and other related commands |
| `:!(command)` | Enter system commands without quitting |



