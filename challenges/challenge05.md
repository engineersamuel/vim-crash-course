# Challenge 05 - Find and Search

This challenge is designed to get you used to using `f` and `F` to find a character within a line and also using search with `/<chars>` and `?<chars>`.

### Commands

`f<char>` will jump forward to the given char, then you can cycle to the next matched char with `;`.
`F<char>` will jump backward to the given char, then you can cycle to the previous matched char with `;`.
`rb` will change the character under the cursor to `b`
`/the` will find all occurrences of `the` looking forward, then you can press `n` to cycle to the next match or `shift+n` to go to the previous match.
`?the` will find all occurrences of `the` looking backwards, then you can press `n` to cycle to the next match looking back, or `shift+n` to look at the previous match (which in this case is looking forward, confusing I know!)
`:nohl` will stop highlighting.

## Challenge

Jump to the character `a` and change it to `b`, then back to the character `B` and change it to `b`, then forward to `C` and change it to `b` then back to `D` and change it to `b`;

BbbbDbbbbbabbbbbbbCbbb

With the next sentence type `/bear` which will highlight all occurrences of `bear`.  Practice typing `n` and `shift+n` to move forward and backward for the matching `bear`.

The bear found a rough tree and the bear scratched it's back.

A more practical example would be extracting out arguments into a separate type, the example is still just a toy example, but I've done this many times:

Input:

```
function sum(a: number, b: number): number {
    return a + b;
}
```

Hints:
* Consider moving the cursor to the function line, type `f(` then `vi(` to select within `(`.

Desired Output:

```
type Args = {
    a: number;
    b: number;
}

function sum(args: Args): number {
    return args.a + args.b;
}
```