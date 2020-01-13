FallingCode
=======================

### Introduction ###
Simulation of the scene of falling code on the terminal. It is generated by pure character, instead of drawing.<br>


![alt text](https://fr.ubergizmo.com/wp-content/uploads/2017/03/matrix.jpg)

### Dependent library ###
ncurses<br>
You need to install it by yourself. If you want to use another library, just edit `SysTool.cpp` and `makefile`.

### Installation ###
Download and execute `make`.

### Execution ###
Go to the directory `bin` and execute one of the commands as below:
* `./matrix.out [colorValue]`. E.g. `./matrix.out 23`.
* `./matrix.out <string> [colorValue]`. E.g. `./matrix.out "hello world!" 122`.
<br>Besides, the `colorValue` is optional and its range is [0, 255].

### Attention ###
Some `pts`-tpye remote terminal may not work as expected, the reason is that the coordinate of terminal is transformed by the `pts`-type remote terminal.


### Additional... ###
I'd like to execute `./matrix.out` because the color by default is green.<br>

There is an issue left: I want to set a tail (with a different color) for each column, whose length is 0.3 * lengthOfColumn, but it would be a very heavy calculation (read the comment in the file Column.h) as it's about `double - multiplication`.<br>
My PC is a Mac Pro with 4GB RAM and its performance is not good enough so I commented the tail part. If you have another way to add the tail without any heavy calculation, it would be appreciated if you let me know.
