# Challenge 06 - Macros

Now let's get to some of the more advanced parts, the incredibly powerful macro command.

#### Commands

* `q<character>` starts recording
* `q` ends recording
* `{count}@{macro char}` will execute the macro bound to the given `char` `count` times.

If you choose `a` as your character then: `3@a` would run the macro three times.

* `@@` would repeat the previously run macro on the current line.

## Challenge

Given the following dictionary:

```
const dictionary = {
    A: 1,
    B: 2,
    C: 3,
    D: 4,
    E: 5,
    F: 6,
    G: 7,
    H: 8,
    I: 9,
    J: 10,
    K: 11,
    L: 12,
    M: 13,
    N: 14,
    O: 15,
    P: 16,
    Q: 17,
    R: 18,
    S: 19,
    T: 20,
    U: 21,
    V: 22,
    W: 23,
    X: 24,
    Y: 25,
    Z: 26
}

enum Letters {

}
```

Make the following modifications using exclusively macros, visual block mode, and yank:

* `A: 1` should become `[Letters.A]: 1`...`[Letters.Z]: 26`.
* The enums should contain `A = 'A'`...`Z = 'Z'`.

Hint: See the gif at the bottom of the [README](../README.md#examples-of-vim-usage) in this repo to see an example of the above transformations.