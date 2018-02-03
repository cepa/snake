# Snake

This is a clone of the legendary Snake game written by any wanna be programmer
at some point.

![snake.png](https://github.com/cepa/snake/raw/master/snake.png)

I created this one in 2004 in pure x86 assembly language for DOS operating system
and can be run in DosBox nowadays.

## How to compile it?
The compiled version _snake.com_ is in the repo so you can skip this point and
simply run it in DosBox, however if you want to try building it yourself do this:

* Install NASM compiler
On Ubuntu simply run
~~~
apt-get install nasm
~~~

* Compile _snake.asm_ to _snake.com_:
~~~
nasm -o snake.com -fbin snake.asm
~~~
