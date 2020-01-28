[Prev](./challenge02.md) - [Next](./challenge04.md)

# Challenge 03 - Editing text

This challenge involes editing text, specifically editing words.
Vim considers a word a block of text surrounded by a space or new line.

#### Commands

* `daw` delete a word and trailing whitespace and stay in normal mode.
* `ciw` delete current word and go into insert "mode".
* `ci<CHAR>` deletes anything in wrapped in the current `<CHAR>` excluding the `<CHAR`>, which is restricted to: ``` {}''""[]()`` ```.
* `yaw` "yank" a word.
* `p` pastes whatever you last yanked or deleted _after_ the cursor.
* `P` pastes whatever you last yanked or deleted _before_ the cursor.

These commands may be helpful but are not strictly necessary:

* `di<CHAR>` deletes anything in wrapped in the current `<CHAR>` including the `<CHAR`>, which is restricted to: ``` {}''""[]()`` ```.
I personally don't use this much.

## Challenge

Delete every other word.

Input:

> The dog jumped over the cat

Output:

> dog over cat

or
> The jumped the


Now let's take something in quotes and change it.

Input:

> The "dog" jumped over the 'cat' (but did not jump over the house)

Output:

> The "cat" jumped over the 'dog' (and over the house)

Finally, let's yank something and paste it 5 times.

Input:

> The annoying dog says "woof woof".

Output:

> The annoying dog says "woof woof woof woof woof woof woof".
 
[Prev](./challenge02.md) - [Next](./challenge04.md)