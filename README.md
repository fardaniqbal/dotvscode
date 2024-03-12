# dotvscode
This repo stores my config for VSCode.

## Usage
Clone this repo, then symlink `%USERPROFILE%\\.vscode` to your clone of
this repo.  This is pretty straightforward on UNIX-like systems, but
involves a few more steps on Windows:
1.  On Windows, clone this repo somewhere on your local storage.  For
    example, `%USERPROFILE%\\dotfiles\\dotvscode\\`.
2.  Edit `%PROGRAMFILES%\\Git\\etc\\gitconfig`:
    1.  Find the `[core]` section and set `symlinks = true`.
3.  Run `git-bash` **as administrator**.
4.  In the `git-bash` administrator prompt:
    1.  Run `export MSYS=winsymlinks:nativestrict`.
    2.  Run `ln -si /c/Users/<YOUR-USERNAME>/dotfiles/dotvscode /c/Users/<YOUR-USERNAME>/.vscode`
