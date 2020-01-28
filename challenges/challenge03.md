# Challenge 03 - Visual mode

This challenge is designed to get you used to using visual mode, i.e. selecting lines or blocks and making changes.

#### Commands

* `V` (shift+v) to select the current line under the cursor, then you can use motion controls to select more lines up or down.
* `ctrl+v` to select a vertical block of text under the cursor, then you can use motion controls to select more characters in the block vertically and horizontally.
* `x` will delete the character(s) currently under the cursor/selection in visual mode.
* `>>` in normal mode and visual mode to tab to the right one tab.
* `<<` in normal mode and visual mode to tab to the left one tab.

This challenge can be accomplished exclusively with the above commands plus commands from previous challenges for editing.

Note that I left out one visual mode, character mode.
Character mode is accessed with `v`, but we don't need it here.
Feel free to play with it.

#### Intermediate

n/a 

#### Advanced

Come back to this challenge and do it with [macros](challenge09.md)!

## Challenge

Here are the tasks to accomplish in this order:

1. Select the `$` character for each of the 3 lines using `ctrl+v` and `j` and delete it with an `x`.
2. Select the three lines vith visual line mode `V` and type `>>`.
3. Treat each line as a json entry and append `: true`, like `withSugar: true`.

```
$withUser
$withProfile
$withOrder
```