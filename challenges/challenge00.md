# Challenge 00 - Hello World

While it's tempting to unlock everything that vim has to offer, let's start simple.
Now that you've got it setup on your machine, you've taken the first step.
(And if you haven't, make sure to peek at the [README](../README.md).)

Although this new tool has a lot of power, let's start with the most basic vim functionality, so you can use your editor like usual.
Vim has many modes, but there are two you'll want to know right away:
1. insert mode: where you can edit text almost like you would in any text editor.
2. normal mode: where you can move around the screen.
You can do more than this, like shortcuts and hotkeys, but we'll keep it simple for now.

Normal mode is the default mode of vim when launched.
You can only enter other modes from normal mode!

#### Commands

* `i` enters insert mode, then you can edit almost as you would normally in VSCode or any text editor.
* `ESC` or `ctrl+[` or `jj` or `ctrl+c` to exit insert mode and enter normal mode.
* `u` will undo what you just did in insert mode.
* `ctrl+r` will redo what you just undid.

## How to quit vim

If you haven't seen [how-to-exit-vim](https://github.com/hakluke/how-to-exit-vim) take a look.
I believe this site is more sarcastic humor than it is reality.

How you exit vim?
From normal mode, just type `:q`.

If you've made edits, vim will warn you.
You can force exit with `:q!`, it's that simple.
(And in VSCode, you don't even need to do that, just `ctrl|cmd+w` or just close the editor tab.)

As easy as that was, you technically used command mode, but we'll cover that later.

## Hello World!

Below this sentence, to the right of the `>` enter insert mode, type Hello World!, then enter normal mode.

`>`

Now that the above reads `> Hello World!` and you are back in normal mode, type `u` to undo what you just did.
The text should now read `>` as it originally did.
Type `ctrl+r` and `> Hello World!` should reappear.