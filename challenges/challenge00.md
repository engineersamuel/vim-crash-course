# Challenge 00 - Hello World

Let's start with the most basic vim functionality: 
* insert mode: where you can edit text like you would in any text editor.
* normal mode: where you can move around the screen.  You can do more than this, but let's keep it simple for now.

#### Commands

* `i` enters insert mode, then you can edit as you would normally in VSCode or any text editor.
* `ESC` or `ctrl+[` or `jj` or `ctrl+c` to exit insert mode and enter normal mode.
* `u` will undo what you just did in insert mode
* `ctrl+r` will redo what you just undid

## Hello World!

Below this to the right of the `>` enter insert mode, type Hello World!, then enter normal mode.

`>`

Now that the above reads `> Hello World!` and you are back in normal mode, type `u` to undo what you just did, the text should now read `>` as it originally did, then type `ctrl+r`, `> Hello World!` should reappear.