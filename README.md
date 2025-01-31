# w.ORIC-PAINT
Oric Atmos Hires Paint program in your webbrowser

(C) 2024 Jonas S Karlsson

Try it out in the browser: [w.ORIC-PAIN](https://yesco.github.io/w.ORIC-PAINT/oric-paint.html).

# Capabilities

- built-in *manual* - at the end
- view HIRES screens with attributes
- draw on the picture using dots
- unlimited *UNDO*
- command line driven. Just type! Clicking on buttons runs text commands...
- various `brush`es
  - line diagonal down circle square
- `spray 5` (%) using the current "brush"-shape
- *unique:* unlimited "mixing" of colors, just select the color and paint! Undo, if you didn't like it. See more detail in the manual/help.
- `load` HIRES screens from file
- `tap` to save the HIRES screen to a tap-file
   *Note:* for some reason the webbrowser add .txt to the name, lol

# Commands

## colors

- `paper green` == `paper 2`
- `ink black`
- `draw red`
- `0` == `k` == `black` == `0`
- `1 `== `r` == `red`
- `2` == `g` == `green`
- `3` == `y' == `yellow` 
- `4` == `u` == `blue`
- `5` == `m` == `magnenta`
- `6` == `c` == `cyan`
- `7` == 'w' == `white`

- `clr` == clear bits of current brush, similar to `curset x,y,fb` fb=0
- `set` == clear bits of current brush, similar to `curset x,y,fb` fb=1
- `xor` == clear bits of current brush, similar to `curset x,y,fb` fb=2

## brushes

- `brush` - default `brush circle`;`size 10`;`spray 10`
- `brush thin` - pixel
- `brush flat` - straight line "-"
- `brush cursive` - diagonal line "/"
- `brush down` - bar "|"
- `brush circle` - uses a circle template
- `brush square` - uses a square

## size

- `size 1` - pixels
- `size 6`
- `size 20`
- `size 50`

## other

- `erase` - erase the current drawing - can be undone!
- `undo` - undo last action
- `redraw` - if you think something isn't correct
- `load` - prompts user to load a HIRES .tap-file
- `tap` - saves a .tap-file of HIRES screen
- `xtap` - experimental: saves a .tap-file, with 3 text lines, with an attribute that changes display to HIES (TODO: add charsets, text garbled)
- `import` - NIY: import any image and try to edit it, currently only uses background attributes, so you can't draw on it. Use `pict-conv` from OSDK.


