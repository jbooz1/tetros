# TetrOS
TetrOS is a small *feature rich* Tetris clone which is written in Assembly.
It fits completely into a 512 byte boot sector and is executed during the
boot sequence before any operating system is loaded. It does not need any
existing operating system. TetrOS is its own operating system, hence the suffix
OS in its name.

This is how it looks like:

![TetrOS - Tetris in 512 byte boot sector](https://github.com/daniel-e/mbr_tetris/blob/master/tetros_tetris_screenshot.png)

And this is the complete machine code:

![TetrOS - Machine code](https://github.com/daniel-e/mbr_tetris/blob/master/code.png)

## Features
* Each brick shape has a unique color.
* Blinking cursor is not visible.
* Left and right arrow to move a brick.
* Up arrow to rotate a brick.
* Down arrow to drop a brick.
* Game over detection. It stops if a new brick could not be placed.
* Selects the next brick at random via a linear congruential generator.
* Shows a nice playing field.

## Features missing due to size limits
* Scores and highscores.
* Intro.
* Game over message and restart without rebooting.
* Show next brick.
* Increase speed.

## Similar projects
* https://github.com/dbittman/bootris
* https://github.com/Shikhin/tetranglix
* http://olivier.poudade.free.fr/src/BootChess.asm
