---
layout: post
title: The bash alias and you.
date: 2023-04-17 18:45:00 -0700
categories: [bash, terminal, programming]
tags: [bash, terminal, shortcuts]
---

# What's in a name?
Anything your nerdy heart desires!

I love using my keyboard as much as possible. Hotkeys, shortcuts, you name it, but I also avoid typing any more than I need to.
I have aliases for just about every command I run regularly. It's about efficiency and ease of use.
I also think aliases are easier for muscle memory.

Typing something like `gst` is much easier and faster for my fingers to learn and repeat than `git status`.


### How do you make a bash alias?
They start with the `alias` command followed by the string you want to type,
then the command you want to execute when you type that string.

To create one, add a line to your `.bashrc` or `.zshrc` file.

```bash
alias be="bundle exec"
```

Then `source` that file to load the alias into your current bash session.

```bash
source ~/.zshrc
```

Since I edit that file a ton... I have an alias to do so!

```bash
zshconfig='sudo nvim ~/.zshrc'
```

### What are my bash aliases?
To list all of your existing aliases, just run `alias`.

```bash
$ alias
=> ...
g='git'
ga='git add'
gaa='git add --all'
gba='git branch -a'
rkdc='rake db:create'
rkdd='rake db:drop'
rkdm='rake db:migrate'
rs='rails server'
...
```

### What does that do again?
If you ever wanna know what a particular alias is gonna do, run `alias {name_of_alias}`.

```bash
$ alias keti
=> keti='kubectl exec -t -i'
```
