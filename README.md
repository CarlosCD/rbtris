# Tetris game in less than 200 lines of code

![](https://storage.googleapis.com/rbtris.github.nakilon.pro/screenshot5.png)

## Controls

**Arrows**, **R** to restart, **P** or **Space** to pause.

## Installation

```
bundle install
bundle exec ruby main.rb
```

## TODO

* [ ] projetion of the piece at the bottom
* [x] [SRS canonical rotation](https://tetris.fandom.com/wiki/SRS)
* [ ] SRS wall kicks
* [x] scoreboard (maybe at `$HOME/.rbtris`)
* [x] ability to fall down only partially
* [x] ability to hold UP (just for fun)
* [x] Mutex stdlib class (no MRuby support)
* [ ] autoresize to screen
* [x] option to restart
* [ ] cheat for testing purposes
* [x] canonical increase of speed
* [x] holding LEFT and RIGHT
* [ ] [canonical scoring](https://tetris.fandom.com/wiki/Scoring)
* [ ] see next piece
* [x] pause key
* [ ] window size configuration
* [ ] canonical music
* [ ] restore controller support
* [ ] color scheme configuration
* [ ] boss key

## Notes

By default ruby2d looks for a font only in one system directory -- this is why ruby2d dependency here was [forked and patched](https://github.com/Nakilon/ruby2d/commit/a80fa4b47e713e22995a7c2698fd055f5464b23b) a bit to support sourcing from the working directory (and `$HOME/Library/Fonts`).

Sketch of the almost current program structure:

![](https://storage.googleapis.com/rbtris.github.nakilon.pro/refactoring4.JPG)
