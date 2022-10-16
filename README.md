# dmenu - dynamic menu

`dmenu` is an efficient dynamic menu for X.

## Changes

The following sections describe the various changes I have added to the st
codebase. The suckless documentation, FAQ, legacy notice, and license for `st`
can be found in the `suckless` directory.

## Build

The config.mk file has had the `PREFIX` variable changed from `/usr/local/` to
`~/.local/`. This allows the st tool to only be installed for my user without 
having to use sudo.

## config.h

The following section describes no patch related changes made to the `config.h`
header file.

## Patches

The following section describes applied patches and any further modifications
using those patches.

### printindex

These patches were applied to get the index of the selected option rather than
the selected option.

- dmenu-printindex-5.0.diff
- dmenu-printindex-cole.diff

The `-cole` variant of the patch was created since the original patch failed to
apply on my build. I have not figured out why. The problem was in the 
`readstdin(void)` function.

### numbers

These patches were applied to get an m/n numbering on the right side of the 
dmenu prompt

- dmenu-numbers-20220512-28fb3e2.diff

This patch would only successfully apply when using the three way merge option
of `git apply`.

```
git apply -3 patches/dmenu-numbers-20220512-28fb3e2.diff
```
