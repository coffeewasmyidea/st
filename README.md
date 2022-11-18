# st - simple terminal emulator for X

This is a terminal that I use everyday, and maybe it will work for you too.

+ Based on [st-0.9](https://st.suckless.org/) with patches from 0.8.5
+ Default theme: [gruvbox](https://github.com/morhetz/gruvbox)
+ Default font: [FantasqueSansMono](https://github.com/belluzj/fantasque-sans)
+ Spare font: `Source Code Pro`

## Bindings

+ **Swap theme (dark|light)** : with `F11`
+ **Scrollback**: with `shift-↑/↓`
+ **Scrollback mouse**: `shift` while scrolling the mouse
+ **Change font size**:`ctrl+shift-↑/↓`
+ **Reset font size**: `ctrl+shift-home` returns to default
+ **Copy/Paste text**: with `ctrl+shift-c`, `ctrl+shift+v` and `ctrl+shift-insert` or right mouse click
+ **Extract all visible URLs and present rofi/dmenu to select and open one**: `ctrl+shift+U`

## Requirements

+ `make` tool for building
+ `libXft` library for fonts drawing
+ `Xlib` header files for interacting with an X server
+ `xurls` tool for extract urls from plain text
+ `Fantasque` default font which you can change in `config.h`

## Patches

+ st-scrollback
+ st-scrollback-mouse
+ alpha
+ externalpipe
+ rightclickpaste
+ font2

## Simple installation

```
git clone https://github.com/ssilaev/st
cd st
sudo make install
```

