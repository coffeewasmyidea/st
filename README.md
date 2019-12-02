# st - simple terminal emulator for X.

+ Default font: [Fira Code](https://github.com/tonsky/FiraCode)
+ Default theme: [Solarized](https://ethanschoonover.com/solarized/)

## Bindings

+ **Swap between light/dark theme**: with `F6`
+ **Scrollback**: with `shift-↑/↓` or `shift-h/shift-j`
+ **Scrollback mouse**: `shift` while scrolling the mouse
+ **Change font size**:`ctrl+shift-↑/↓`
+ **Reset font size**: `ctrl+shifts-home` returns to default
+ **Copy/Paste text**: with `ctrl+shift-c` and `ctrl+shift+v` or `ctrl+shift-insert`

## Requirements

+ `make` tool for building
+ `libXft` library for fonts drawing
+ `Xlib` header files for interacting with an X server
+ `Fira Code` just default font, which you can change it in `config.h`

## Patches

+ st-scrollback
+ st-scrollback-mouse
+ st-solarized-both
+ st-font2
+ alpha

## Simple installation

```
git clone https://github.com/ssilaev/st
cd st
sudo make install
```
