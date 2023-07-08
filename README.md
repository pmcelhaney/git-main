# git-main

A bash script to checkout the main / default branch of a git repository.

## Motivation

I work with a lot of git repositories that have inconsistently named main/default/master branches. Sometimes the "main" branch is called something like "dev" or "release".
I got tired of trying to keep them straight in my head, so I wrote a little bash script (with the help of ChatGPT).

## Installation

Copy the `git-main` file to somewhere in your `$PATH` and make it executable.

```sh
sudo cp git-main /usr/local/bin
sudo chmod +x /usr/local/bin/git-main
```

## Usage

```sh
git main
```

The first time you run it, it will ask you to choose a default branch name. It will then checkout the branch with that name. The next time you run it, it will checkout that branch without asking. The default branch name for each working directory is stored in `~/.git-main`.

## License

MIT
