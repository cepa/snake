# Snake

This is yet another clone of the legendary Snake game.

![snake.png](https://github.com/cepa/snake/raw/master/snake.png)

I created this one in 2004 in pure x86 assembly language for DOS operating system
and can be run in DosBox nowadays. It is a 16bit retro game and should run on
anything newer than ancient Intel 80186 processor.
Graphics is displayed using a very old 13H mode with 320x200 pixel with a custom
colour palette and screen buffering. Fonts are displayed using the BIOS builtin
glyphs available in system memory. Sprites and pictures were created with another custom
program that converted them to a byte array representation.

## How to compile it?
The compiled version _snake.com_ is in the repo so you can skip this point and
simply run it in DosBox, however if you want to try building it yourself do this:

* Install NASM compiler, on Ubuntu you can simply run:
~~~
apt-get install nasm
~~~

* Compile _snake.asm_ to _snake.com_:
~~~
nasm -o snake.com -fbin snake.asm
~~~

## How to run it?
* First you need to clone this repo or download _snake.com_ to a folder.
* Next you need to install [DosBox](https://www.dosbox.com/), on Ubuntu just run:
~~~
apt-get install dosbox
~~~
* Next run DosBox and mount directory where _snake.com_ is located
~~~
mount c path/to/snake/folder
~~~
* Now you can start _snake.com_
~~~
snake.com
~~~
* Use keyboard arrows (_Up_, _Down_, _Left_, _Right_) to drive the snake
* _ESC_ quits the game
* _A_ print about
* _P_ pause the game

This code is protected by the [Beerware](https://en.wikipedia.org/wiki/Beerware) license :P
