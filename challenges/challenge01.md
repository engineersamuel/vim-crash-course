# Challenge 01 - Motion and editing

This challenge is designed to get you accustomed to motion controls in vim.  

Here are the most commonly used motions:

* `h`: left
* `j`: down
* `k`: up
* `l`: right
* `ctrl+d` is page down
* `ctrl+u` is page up
* `gg`: goes to the top of the page
* `G`: (shift+g) goes to the bottom of the page
* `zz`: centers the page
* `$` will move to the end of a line
* `0` will move to the beginning of a line

These are all while in normal mode.  If you are in insert mode you'll have to either `ESC` or `ctrl+[` or `jj` (If you've configured that key combo, don't worry if you haven't, or just ask) or `ctrl+c` to escape to normal mode, then you can use the motion keys.

#### Commands:

* `j` to move down, `k` to move up, `h` to move left, `l` to move right.
* `i` to enter insert mode to edit as you would normally expect in a text editor.
* `ESC` or `ctrl+[` or `jj` or `ctrl+c` to exit insert mode and enter normal mode.  I won't spell this out again, in further challenges I'll just specify to exit insert mode or enter normal mode.
* `u` in normal mode will undo the previous change.

This challenge can be accomplished exclusively with the above commands.

#### Intermediate

* `1j` will jump down one line, `2f` will jump down two lines and `2k` will jump up two lines.
* `$` to move to the end of the line.
* `w` to move forward to the next word.
* `b` to move backward to the previous word.
* `e` to move forward to the end of a word.
* `ge` to move backword to the end of a word.
* `r2` will replace the character under the cursor with 2.

#### Advanced

In normal mode you can use `V` (shift+v) to enter visual mode to select a block of text.  Then you can `j` or `shift+]` to select the block of 0s.  Once selected you can type `:s/0/1/g` to replace 0s with 1s.

If you want to play with `$` for changing the first 1 you could navigate to the line the first 1, type `$` to move to the end of the line, then make the change.

## Change 0s to 1s

```
      0

0   0   0   0


0 0 0 0 0 0 0

0           0

      0
```

## Jump by paragraph

Moving by paragraph is extremely common in development, it's one of the most common things I do, for example if you want to jump through each function, if there are two new lines between them, is very efficient.  Practice typeing `{` (shift+[) and `}` (shift+]) to move to the middle, bottom, middle and two, of the two below paragraphs.  This is all done in normal mode.

> "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."

> "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."
