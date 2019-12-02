# st - simple terminal emulator for X.

+ Default font: [Fira Code](https://github.com/tonsky/FiraCode)
+ Default theme: [Solarized](https://ethanschoonover.com/solarized/) (swap between light/dark with F6)

## Patches

+ st-scrollback
+ st-scrollback-mouse
+ st-solarized-both
+ st-font2
+ alpha

## Requirements

+ `make` tool for building
+ `libXft` library for fonts drawing
+ `Xlib` header files for interacting with an X server
+ `Fira Code` just default font, which you can change it in `config.h`

## Simple installation

```
git clone https://github.com/ssilaev/st
cd st
sudo make install
```
