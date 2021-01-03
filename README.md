# st

To apply patch, do `patch -p1 < patchHere`.

# Patches installed
- alpha
- anysize
- delkey
- newterm (no need)
- dracula
- scroll
    - scroll can resize st screen
    - disable the shortcuts for scrolling in scroll, use the patch scrollback instead!!
- scrollback
    - scrollback mouse altscreen
    - scrollback mouse altscreen increment
- vertcenter
- clipboard
- workingdir

# TODO
- The buffer often does not refresh if applies the `scroll` program.. but if doesn't use `scroll` then the lines does not resize properly (will result in line cut off) when resized.. Did not find a good solution for this yet.
