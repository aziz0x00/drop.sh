# 🗑 drop.sh

**drop.sh** is an `rm` alternative with trash functionality with `fzf`

![Preview](./preview.gif)

## ⚡️ Requirements

- `fzf` (for search in trash)
- `uuidgen`, `awk` and some other `coreutils` that you are very likely to have

## 📦 Installation

For now you can just copy `drop` to a directory included in your `PATH`

## 🚀 Usage

```
Usage: drop [FILE]...
  or: drop [OPTION]
The default action will move FILE(s) to the trash directory where it can be
restored later with the option --restore with the fuzzy finder *fzf*.

  -h, --help      display this help text
  -r, --restore   to restore files, this must be the first argument, ignoring any other
  -V, --version   output version inforamtion

To remove a file whose name starts with a '-', for example '-h',
use one of these commands:
    drop -- -h

    drop ./-h

    drop anotherfiletodelete -h
```
