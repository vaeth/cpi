# `cpi` and `mvi`

(C) Martin Väth (martin at mvath.de).
This project is under the BSD license 2.0 (“3-clause BSD license”).
SPDX-License-Identifier: BSD-3-Clause

A POSIX shell wrapper for `cp -i -a` and `mv -i`, making use of `diff`

This is a somewhat verbose frontend for `cp -i -a` and `mv -i`:
For each file you see the differences before you confirm/reject
the copying/moving.

You get more detailed instructions by calling
- `cpi -h`
- `mvi -h`

### Requirements

The cpi variant requires that your `cp` command supports the non-POSIX options
- `-a`
- `-d`
- `--preserve=timestamps`

### Installation

For installation. just copy the content of `bin/` into your `$PATH`.
To obtain support for __zsh completion__, copy the content of `zsh/` to your
zsh's `$fpath`.

For Gentoo, there is an ebuild in the mv overlay (available over layman).
