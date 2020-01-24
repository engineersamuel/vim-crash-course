# Challenge 04 - Moving and selecting within brackets

This challenge is designed to get you used to selecting motion and selection within brackets `{}[]()`.  You'll use this practically every single day when workin in code.

#### Beginner commands expected

* `di(` delete in `(` brackets.
* `%` will jump to the matching `{}[]()` bracket.

This challenge can be accomplished exclusively with some or more of the commands plus commands from previous challenges for editing.

#### Advanced

* `vl"ay` If executed will yank the character under the cursort to the `a` buffer.
* `"aP` will paste buffer `a` in place.

## Challenge

Practice selecting in `{}`, position the cursor over `{` then type `%` and optionally now type `y` to yank the selection into the buffer.

```
function printHello() {
    console.log(`Hello World!`);
}
```

Optional output:
```
{
    console.log(`Hello World!`);
}
```

Now practice selecting within `()`, for example if you want to extract arguments from a function.

```
function concat(a: string, b: string, c: string) {
    return a + b + c;
}
```

Optional output: `a: string, b: string, c: string`

Input:

```
public int Sum(int y, int x) {
    return y + x;
}
```

Desired output:

```
public string Append(string a, string b) {
    return a + b;
}
```

Input:

```
function sum(x, y) {
    return x + y;
}
```

Desired output: `(x, y) => x + y;`