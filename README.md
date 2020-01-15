# Introduction

This crash course focuses on vim in VSCode.  Topics such as optimal `.vimrc` configurations or setting up vim in your shell to do auto-completion will not be covered.  VSCode provides an incredible development environment, and that paired with vim is a comprehensive solution for my purposes.  That's not to say I don't have [gripes](#vscode-vim-problems).

The other focus of this course is assume no prior knowledge of vim.  While that is true, I do have a way to make thise course challenging for medium to advanced users as well.

## Getting started

* Install vim in VSCode: https://marketplace.visualstudio.com/items?itemName=vscodevim.vim
* Clone this [repo](https://aka.ms/vimcrashcourse): `git clone git@github.com:engineersamuel/vim-crash-course.git`
* Put together a screencast of the power of vim.

For more advanced users, if you want a challenge while still doing the intro content do the following:
* For Windows see:

![image](https://gist.github.com/engineersamuel/a0fbd261d38d958a17eb89cc2500a391/raw/Wed_Jan_15_2020_1579128499718.png)

* Mac, by default disables repeated keys, however if you have already re-enabled them do the following:
```
$ defaults write com.microsoft.VSCode ApplePressAndHoldEnabled -bool false         # For VS Code
$ defaults write com.microsoft.VSCodeInsiders ApplePressAndHoldEnabled -bool false # For VS Code Insider
```

## The power of vim

TBD

## How to quit vim

TBD

## Understanding vim syntax

TBD: Tech basic syntax and how it is written.  For example daw, x, d5j, i.e. {operator}{count}{motion}

## Moving around

TBD

## Editing

TBD

## My productive mainstays

TBD

#### VSCode Vim problems

* Key latency and performance.  I've encountered instances where I can type significantly faster than VSCode can handle the input creating a very annoying situation where I have to continually `u` and retype what I want since my vim commands were lagging.  Many times restarting VSCode completely helps, or my computer.  From what I've read on the VSCode github issues section this is largely due to vim commands going through an emulation layer instead of being natively handled by the underlying vim package like how Sublime handles it.
