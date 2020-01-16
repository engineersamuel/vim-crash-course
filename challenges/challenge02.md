# Challenge 02 - Moving around the screen

This challenge is designed to get you used to moving around the screen and re-orienting your view.

* Beginner commands expected:
`ctrl+d` to scroll down one page
`ctrl+u` to scroll up one page

This challenge can be accomplished exclusively with the above commands plus commands from previous challenges for editing.

* Intermediate:
`G` (shift+g) to move to the bottom of the screen
`gg` to move to the top of the screen, though that really isn't necessariliy where you want to go
`zz` to center the screen where the cursor is

* Advanced

`/somewhere{ENTER}` will search the page for somewhere, then you can press `n` to cycle to the next occurrence.
`{count}j` will jump `count` downwards
`{count}u` will jump `count` upwards

* Advanced

In normal mode you can use `V` (shift+v) to enter visual mode to select a block of text.  Then you can `j` or `shift+]` to select the block of 0s.  Once selected you can type `:s/0/1/g` to replace 0s with 1s.

## Challenge

Here are the tasks to accomplish in this order:
* At the very bottom of this document find `I'm at the somewhere on the page` and change `somewhere` to `bottom`
* Then scroll to the middle and change `somewhere` to `middle`.
* Then scroll back up right below these instructions and change `somewhere` to `top`.

```
I'm somewhere on the page











































I'm somewhere on the page

















































I'm somewhere on the page
```