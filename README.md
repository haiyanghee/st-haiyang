# st

To apply patch, do `patch -p1 < patchHere`.

# This patch is based on `vim browse` patch
It requires some work to make the patch working (I put the `normalMode.c` into `st.c` because these files depend on each other apparently).
- It works very well
- You cannot scroll using the scrollback patch anymore (there is probably a patch for vim browse that handles it but I'm too lazy to repatch it, it takes lots of time)
    - Thus you can ***only*** scroll using the normal mode
This patch is good if you want to copy paste very specific things in terminal.. but I think I don't need that very often, since I could just copy paste the output in the terminal to vim and go from there..

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

# TODO
- The buffer often does not refresh if applies the `scroll` program.. but if doesn't use `scroll` then the lines does not resize properly (will result in line cut off) when resized.. Did not find a good solution for this yet.
