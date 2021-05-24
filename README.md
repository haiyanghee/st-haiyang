# st

To apply patch, do `patch -p1 < patchHere`.

To install, run `sudo make clean install`.

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
- font2 (to see colored emojies, please install **`libxft-bgra`**, which is a fix for libxft colored emoji rendering problem. It is available from the [AUR](https://aur.archlinux.org/packages/libxft-bgra/))
- externalpipe (plus copying urls and output that [Luke](https://github.com/LukeSmithxyz/st) made with [video](https://www.youtube.com/watch?v=5E9bO5ZURcs&ab_channel=LukeSmith))
- xresources (allows customization of st parameters on the fly with xresources) 


# TODO
- The buffer often does not refresh if applies the `scroll` program.. but if doesn't use `scroll` then the lines does not resize properly (will result in line cut off) when resized.. Did not find a good solution for this yet.
