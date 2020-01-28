# Challenge 06 - Find and Search

This challenge is designed to get you used to using `f` and `F` to find a character within a line and also searching with `/<chars>` and `?<chars>`.

#### Commands

The core search commands are `f`ind and un`t`il.
* `f<char>` will jump forward to the given char, then you can cycle to the next matched char with `;`.
* `F<char>` will jump backward to the given char, then you can cycle to the previous matched char with `;`.
* `t<char>` will jump forward to just before the given char, then you can cycle to the next match with `;`.
* `T<char>` will jump backward to just before the given char, then you can cycle to the previous match with `;`.

There's also more powerful search tools available.
* `/the` will find all occurrences of `the` looking forward, then you can press `n` to cycle to the next match or `shift+n` to go to the previous match.
This supports regex!
* `?the` will find all occurrences of `the` looking backwards, then you can press `n` to cycle to the next match looking back, or `shift+n` to look at the previous match (which in this case is looking forward, confusing I know!)
This supports regex, too!
* `:nohl` will stop highlighting.

Replacing characters

* `r<char>` will change the character under the cursor to `<char>`, i.e. `rb` will change the current character to a `b`.

## Challenge

Jump to the character `a` and change it to `b`, then back to the character `B` and change it to `b`, then forward to `C` and change it to `b` then back to `D` and change it to `b`.

> BbbbDbbbbbabbbbbbbCbbb

With the next sentence type `/bear` which will highlight all occurrences of `bear`.  Practice typing `n` and `shift+n` to move forward and backward for the matching `bear`.

> The bear found a rough tree and the bear scratched its back.