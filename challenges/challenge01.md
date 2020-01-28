[Prev](./challenge00.md) - [Next](./challenge02.md)

# Challenge 01 - Motion and editing

This challenge is designed to get you accustomed to motion controls in vim.

Vim was designed by lazy programmers.
It's designed to make sure your fingers spend as much time on the home row on a QWERTY keyboard as possible.
![Home Row](https://i.pinimg.com/originals/3b/e3/2f/3be32f612f5b183ea24bfa37e21c07f9.png)

Remember, hotkeys like this work in normal mode.
Here are the most commonly used motions:

* `h`: left
* `j`: down
* `k`: up
* `l`: right

Note: Look familiar?
Look at the right hand of the home row.
";" got left out ;,(

There are a lot of other powerful motions as well!
* `ctrl+d`: page down
* `ctrl+u`: page up
* `gg`: goes to the top of the page
* `G`: (shift+g) goes to the bottom of the page
* `zz`: centers the page
* `$`: moves to the end of a line
* `^` or `0`: moves to the beginning of a line

If you are in insert mode you'll have to either `ESC` or `ctrl+[` or `jj` (If you've configured that key combo, don't worry if you haven't, or just ask) or `ctrl+c` to escape to normal mode, then you can use the motion keys.

Sometimes motions don't work in vim like you think they should, for example on this line, which, while a run-on sentence, is actually intentionally really long, because it allows us to play around with different motions in vim.

Moving around it with just `j` and `k` sucks.
That's because they work on what your file thinks is the next line, not what _looks_ like the next line.

If you have word wrap on, you can use `gj` or `gk` to "go" down or up visually.
Maneuvering that paragraph is a breeze.

#### Commands:

* `j` to move down, `k` to move up, `h` to move left, `l` to move right.
* `i` to enter insert mode and edit as you would normally expect in a text editor.
* `ESC` or `ctrl+[` or `jj` or `ctrl+c` to exit insert mode and enter normal mode.
(I won't spell this out again, in further challenges I'll just specify to exit insert mode or enter normal mode.)
* `u` in normal mode will undo the previous change.

This challenge can be accomplished exclusively with the above commands.

#### Intermediate

* `1j` will jump down one line, `2f` will jump down two lines and `2k` will jump up two lines.
* `$` to move to the end of the line.
* `w` to move forward to the next word.
* `b` to move backward to the previous word.
* `e` to move forward to the end of a word.
* `ge` to move backward to the end of a word.
* `r2` will replace the character under the cursor with 2.

#### Advanced

In normal mode you can use `V` (shift+v) to enter visual mode to select a block of text.
Then you can `j` or `shift+]` to select the block of 0s.
Once selected you can type `:s/0/1/g` to replace 0s with 1s.

If you want to play with `$` for changing the first 1 you could navigate to the line with the first 1, type `$` to move to the end of the line, then make the change.

## Change 0s to 1s

```
      0

0   0   0   0


0 0 0 0 0 0 0

0           0

      0
```

## Jump by paragraph

Moving by paragraph is extremely common in development, it's one of the most common things I do.
For example, if you want to jump through each function, if there are two new lines between them, moving by paragraph is very efficient.

Practice typing `{` (shift+[) and `}` (shift+]) to move to the top, middle, and bottom, of the two paragraphs below.
This is all done in normal mode.

> "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."

> "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."

[Prev](./challenge00.md) - [Next](./challenge02.md)