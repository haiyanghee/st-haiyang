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
- font2 (to see colored emojies, please install **`libxft-bgra`**, which is a fix for libxft colored emoji rendering problem. It is available from the [AUR](https://aur.archlinux.org/packages/libxft-bgra/))

# Small changes
- By default st will copy your selection of text in the terminal, so if you do not want this, in `x.c` and function `void brelease(XEvent *e)` you can comment out the part ( which is what I did)
    ```
    if (e->xbutton.button == Button1)
    mousesel(e, 1);
    ```

# TODO
- The buffer often does not refresh if applies the `scroll` program.. but if doesn't use `scroll` then the lines does not resize properly (will result in line cut off) when resized.. Did not find a good solution for this yet.
