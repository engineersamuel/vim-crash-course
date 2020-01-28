# Introduction

My focus in this crash course is to get you up and running with vim in VSCode assuming no real prior knowledge.
Topics such as optimal `.vimrc` configurations or setting up vim in your shell to do auto-completion will not be covered.
VSCode provides an incredible development environment, and that paired with vim is a comprehensive solution for my purposes.
That's not to say I don't have [gripes](#vscode-vim-problems).

While I'm targetting a happy path for beginners, I do cover intermediate and advanced commands for each challenge to more versed vim users can benefit as well.

## Getting started

* Install vim in VSCode: https://marketplace.visualstudio.com/items?itemName=vscodevim.vim
* In VSCode edit settings (cmd+, or ctrl+,) and search for "lineNumbers" then ensure the dropdown says "relative"
* Fork this [repo](https://aka.ms/vimcrashcourse): `git clone git@github.com:engineersamuel/vim-crash-course.git`

Since you will be modifying your fork in the challenges, it may be a good idea to have the master git repo open in a tab for reference, just in case you deviate a bit to far in your editing.

## The power of vim

To see a little bit of the magic you can do with vim see the [examples](#examples-of-vim-usage) below.

## Understanding vim syntax

If you want to decifer any vim syntax on the net, you need to know the grammar.
While it can get more complicated when we are talking about commands and searching, to keep it basic, just remember this: `{operator}{count}{motion}`

Examples:
* `daw` translates to `{operator: delete}{count: a single}{motion: word}`
* `x` translates to `{operator: delete}{count: unused}{motion: unused}`
* `d5j` translates to `{operator: delete}{count: 5}{motion: down}`
* `4k` translates to `{operator: unused}{count: 4}{motion: up}`

## Challenges

The challenges are designed in an OpenHack style where each successive challenge builds on the previous ones.
The challenges have a list of commands that are required, and many times have addtiional intermediate and advanced commands that are optional.
Remember, commands can only be run in normal mode.

While you can click through and view each challenge in github, the repo is meant to be cloned and completed within VSCode.

* [Challenge 00 - Hello World](./challenges/challenge00.md)
* [Challenge 01 - Motion and editing](./challenges/challenge01.md)
* [Challenge 02 - Moving around the screen](./challenges/challenge02.md)
* [Challenge 03 - Visual mode](./challenges/challenge03.md)
* [Challenge 04 - Editing text](./challenges/challenge04.md)
* [Challenge 05 - Moving and Selecting in brackets](./challenges/challenge05.md)
* [Challenge 06 - Find and Search](./challenges/challenge06.md)
* [Challenge 07 - Search and Replace](./challenges/challenge07.md)
* [Challenge 08 - Registers](./challenges/challenge08.md)
* [Challenge 09 - Repeating commands](./challenges/challenge09.md)
* [Challenge 10 - Macros](./challenges/challenge10.md)

#### Examples of vim usage

Two demo videos of using vim.
Note that the mouse was never touched in these screencasts.
I still maybe only consider myself a 7.5/10 in the vim mastery department, always room for improvement.

Here is a screencast of extracting out dictionary keys to an enum.

![Macros](media/vim_macros.gif)

And one of converting a React class to a function.

![Class to Func](media/class_to_func.gif)

#### VSCode Vim problems

* Key latency and performance.
I've encountered instances where I can type significantly faster than VSCode can handle the input creating a very annoying situation where I have to continually `u` and retype what I want since my vim commands were lagging.
Many times restarting VSCode completely helps, or my computer.
From what I've read on the VSCode github issues section this is largely due to vim commands going through an emulation layer instead of being natively handled by the underlying vim package like how Sublime handles it.
