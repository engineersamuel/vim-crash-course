# Challenge 03 - Visual mode

This challenge is designed to get you used to using visual mode, i.e. selecting lines or blocks and making changes.

#### Beginner commands expected
* `V` (shift+v) to select the current line under the cursor, then you can use motion controls to select more lines up or down.
* `ctrl+v` to select a vertical block of text under the cursor, then you can use motion controls to select more characters in the block vertically and horizontally.
* `x` will delete the characters currently selected in visual mode.
* `>>` in normal mode and visual mode to tab to the right one tab.
* `<<` in normal mode and visual mode to tab to the left one tab.

This challenge can be accomplished exclusively with the above commands plus commands from previous challenges for editing.

Note that I left out one visual mode, character mode, which is just `v` but we don't need it here, but feel free to play with it.

#### Intermediate

n/a 

#### Advanced

n/a though you could use macros to accomplish this faster, but that will be covered in a later challenge.

## Challenge

Here are the tasks to accomplish in this order:
* Select the `$` character for each of the 3 lines using `ctrl+v` and `j` and delete it with an `x`.
* Select the three lines vith visual line mode `V` and type `>>`.

```
$withUser
$withProfile
$withOrder
```