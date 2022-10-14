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

