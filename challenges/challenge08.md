# Challenge 06 - Repeating previous commands

Let's deal with the situation in which you want to repeat a previously run command.

#### Commands

* `.` repeats the last command run
* `&` repeats the last substitution
* `~` to toggle case
* `:s/the//g`

You could optionally use the following commands:

* `gU` then a motion will uppercase
* `gu` then motion to lower case

Just to mention the one other one, but for macros (next challenge):

* `@@` repeats the last run macro

## Challenge

Uppercase the beginning of each word, but strictly only uppercase the first word, repeat the command for every successive word.

> small mice large cats quickly chase slowly eat green cheese.

Next remove `the` from the first sentense using find/replace on a single line, then remove them from the next three sentences by repeating the previous command.

> What the mouse?
> What the cat?
> What the dog?

Next delete all text in the `""` in the below keys. But only do it on the first key `"withA"`, then repeat the command for the rest.

```
{
    "withA": 1,
    "withB": 2,
    "withC": 3,
    "withD": 4,
    "withE": 5
}
```