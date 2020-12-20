# Sergey's build of st - simple terminal emulator for X

This is my terminal which I use every day and update from time to time.

+ Based on [st-0.8.4](https://st.suckless.org/)
+ Default theme: `Solarized Light` swap between light/dark with `F6`
+ Default font: `Monospace`
+ Default shell: `sh`

## Bindings

+ **Scrollback**: with `shift-↑/↓` or `ctrl+shift-h/ctrl+shift-j`
+ **Scrollback mouse**: `shift` while scrolling the mouse
+ **Change font size**:`ctrl+shift-↑/↓`
+ **Reset font size**: `ctrl+shifts-home` returns to default
+ **Copy/Paste text**: with `ctrl+shift-c`, `ctrl+shift+v`, `ctrl+shift-insert` and right mouse button2/button3 click
+ **Extract all visible URLs** and present rofi/dmenu to select and open one: `ctrl+shift+U`

## Requirements

+ `make` tool for building
+ `libXft` library for fonts drawing
+ `Xlib` header files for interacting with an X server
+ `libxft-bgra` libXft with BGRA glyph (color emoji) rendering & scaling pathes
+ `xurls` tool for extract urls from plain text
+ `ttf-joypixels` emoji as a Service (formerly EmojiOne)

## Patches

+ st-scrollback
+ st-scrollback-mouse
+ alpha
+ externalpipe
+ rightclickpaste
+ font2
+ xresources
+ solarized-both

## Simple installation

```
git clone https://github.com/ssilaev/st
cd st
sudo make install
```

## Dynamic configuration thought Xresources

You can specify a font, color theme, alpha, and ximspot interval in .Xresources.
After applying new settings, need to update X server resources via xrdb utility `xrdb ~/.Xresources`.

Example:

```
st.alpha:		0.8
st.font:		Droid Sans Mono Slashed for Powerline:pixelsize=16
st.shell:		zsh
st.termname:    st-256color
st.color0:		#073642
st.color1:		#dc322f
st.color2:		#859900
st.color3:		#b58900
st.color4:		#268bd2
st.color5:		#d33682
st.color6:		#2aa198
st.color7:		#eee8d5
st.color9:		#cb4b16
st.color8:		#fdf6e3
st.color10:		#586e75
st.color11:		#657b83
st.color12:		#839496
st.color13:		#6c71c4
st.color14:		#93a1a1
st.color15:		#fdf6e3
...
```

Full list of available variables you can check in `config.h`.


