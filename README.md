# Personal Blog Template

!! Deprecated

## tl;dr

1. Fork this repo
2. Change name of repo
3. edit ./config.md ./index.md ./\_assets/favicon.png ./\_assets/dp.webp
4. use `./blog new`
5. use `./blog spcheck posts/filename.md`
6. use `./blog publish`

For Dhruva alone, https://stackoverflow.com/a/30352360

## What it is

This is a template for a [Franklin.jl](https://github.com/tlienart/Franklin.jl) powered blog adapted from the hyde theme, but with a dark theme and some `utils.jl` and bash scripts to handle basic blog tasks

### Grammar check

~~As part of the blogging process, most people tend to run their work through a third party spell/grammar check, but these services are either not free (as in libre and as beer), or worse, do not even integrate with text editors. Hence, I have added a utility julia script called LanguageTool.jl which uses a local [LanguageTool](https://languagetool.org/) server to check your code.~~

LanguageTool has support for (n)vim and vscodium(vscode), and supporting the plugin seems pointless.

### Github action

The Franklin github action is used unchanged so that blog builds are done at every push.

## Setup

### Minimal

1. Create a GitHub account
2. Click the "Fork" button on the top right.
3. This will open https://github.com/Your-User-Name/blog-template
4. Click Settings and change the name of the repo to `blog`, or something of your choice. Your blog will then be hosted at https://Your-User-Name.github.io/reponame/

1. On your laptop, install [git](https://git-scm.com/)
2. Run `git clone https://github.com/Your-User-Name/your-repo-name.git`, which creates a connected copy of your blog for you to edit.
3. `cd your-repo-name` 
4. edit ./config.md ./index.md ./\_assets/favicon.png ./\_assets/dp.webp and fill your info.

### Complete

These steps are only necessary if you want to build the site locally or run spellcheck

1. Do all steps as before until the second last step.
2. Install [julia](https://julialang.org/).
3. Run `./blog setupjl`
4. Run `./blog setuplt`

## Usage

1. `cd reponame`
2. `./blog new`. DO NOT change the file name.
3. Edit your blog post in [Markdown](https://franklinjl.org/syntax/markdown/)
4. `./blog publish`

If you also want to build and see your site locally,

1. `./blog serve`

If you want to run spellcheck too,

1. `./blog spcheck posts/filename.md`

# Happy Blogging!

If you decide to use my template, let me know! I'll link your blog on mine, and you do the same!

