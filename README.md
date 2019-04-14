# Isabella gtk
This is a theme for gtk and gnome-shell. I generated it from [Arc](https://github.com/NicoHood/arc-theme) using the ["change_color"](https://github.com/NicoHood/arc-theme/blob/master/change_color.sh) bash script from the Arc repo and then further manually modified various elements. It's not perfect, for example I would change the window buttons but I don't know enough about gtk theming to actually do that.

The icons are also modified from the Arc icon theme, I just dropped them in GIMP and made them orange.

![gtk screenshot](https://i.imgur.com/7sGgTb1.png)

## Install
Download the [latest gnome zip](https://github.com/Tiamarth/Isabella/releases/download/04%2F14%2F19/gnome.zip) from the [releases tab](https://github.com/Tiamarth/Isabella/releases/) of the repo, and put "Isabella" and/or "Isabella-Light" in `~/.themes` or `/usr/share/themes`. Then put "Isabella-Icons" in `~/.icons` or `/usr/share/icons`.

Or, using your terminal, enter these commands:

```shell
git clone https://github.com/Tiamarth/Isabella.git && cd Isabella/gnome
mv Isabella ~/.themes
mv Isabella-Light ~/.themes
```

Note that these commands will clone the whole repo onto your system, including the [Sublime Text color scheme](https://github.com/Tiamarth/Isabella/tree/master/sublime) and the [Vivaldi skin.](https://github.com/Tiamarth/Isabella/tree/master/vivaldi)

If you want to download Arc and then manually generate this theme, here are the commands for that:

```shell
git clone https://github.com/NicoHood/arc-theme --depth 1 && cd arc-theme
./change_color.sh --output Isabella <(echo -e "BG=333335\nFG=d1d1d1\nHDR_BG=101013\nHDR_FG=d1d1d1\nSEL_BG=be4318\nSEL_FG=d1d1d1\nTXT_BG=2c2c2c\nTXT_FG=d1d1d1\nBTN_BG=2c2c2c\nBTN_FG=d1d1d1\n")
./change_color.sh --output Isabella-Light <(echo -e "BG=f9f9f9\nFG=4c4f59\nHDR_BG=cccccc\nHDR_FG=4c4f59\nSEL_BG=be4318\nSEL_FG=d1d1d1\nTXT_BG=e5e5e5\nTXT_FG=4c4f59\nBTN_BG=e5e5e5\nBTN_FG=4c4f59\n")
```

But some colours will be off with this method because the script isn't perfect. I had to further modify the generated files in order to make various aspects of gnome-shell legible.
