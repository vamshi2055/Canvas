*** The Problem ***

__Description__

You're given the task of writing a simple console version of a drawing program. 
At this time, the functionality of the program is quite limited but this might change in the future. 
In a nutshell, the program should work as follows:
 1. Create a new canvas
 2. Start drawing on the canvas by issuing various commands
 3. Quit

Please note that i have introduced a new command to print a diagnol line

Command 		Description
C w h           Should create a new canvas of width w and height h.
L x1 y1 x2 y2   Should create a new line from (x1,y1) to (x2,y2). Currently only
                horizontal or vertical lines are supported. Horizontal and vertical lines
                will be drawn using the 'x' character.
R x1 y1 x2 y2   Should create a new rectangle, whose upper left corner is (x1,y1) and
                lower right corner is (x2,y2). Horizontal and vertical lines will be drawn
                using the 'x' character.
D x1 y1 x2 y2   Should create a new Diagonal line from (x1,y1) to (x2,y2). Diagonal line
                is drawn using the 'x' character.For a line to be Diagonal (x2-x1)=(y2-y1)
B x y c         Should fill the entire area connected to (x,y) with "colour" c. The
                behavior of this is the same as that of the "bucket fill" tool in paint
                programs.                
Q               Should quit the program.

__Sample I/O__

Below is a sample run of the program. User input is prefixed with enter command:

enter command: C 10 20
------------
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
------------

enter command: L 1 2 6 2
------------
|          |
|xxxxxx    |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |

enter command: L 6 3 6 4
------------
|          |
|xxxxxx    |
|     x    |
|     x    |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
------------

enter command: D 2 3 7 8
------------
|          |
|xxxxxx    |
| x   x    |
|  x  x    |
|   x      |
|    x     |
|     x    |
|      x   |
|       x  |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
|          |
------------

Enter Command:R 1 14 3 18
------------
|          |
|xxxxxx    |
| x   x    |
|  x  x    |
|   x      |
|    x     |
|     x    |
|      x   |
|       x  |
|          |
|          |
|          |
|          |
|xxx       |
|x x       |
|x x       |
|x x       |
|xxx       |
|          |
|          |
------------

Enter Command:B 8 3 o
------------
|oooooooooo|
|xxxxxxoooo|
|oxoooxoooo|
|ooxooxoooo|
|oooxoooooo|
|ooooxooooo|
|oooooxoooo|
|ooooooxooo|
|oooooooxoo|
|oooooooooo|
|oooooooooo|
|oooooooooo|
|oooooooooo|
|xxxooooooo|
|x xooooooo|
|x xooooooo|
|x xooooooo|
|xxxooooooo|
|oooooooooo|
|oooooooooo|
------------

Enter Command:Q
------------
|oooooooooo|
|xxxxxxoooo|
|oxoooxoooo|
|ooxooxoooo|
|oooxoooooo|
|ooooxooooo|
|oooooxoooo|
|ooooooxooo|
|oooooooxoo|
|oooooooooo|
|oooooooooo|
|oooooooooo|
|oooooooooo|
|xxxooooooo|
|x xooooooo|
|x xooooooo|
|x xooooooo|
|xxxooooooo|
|oooooooooo|
|oooooooooo|
------------
***********Quitting***********************"# Canvas" 
