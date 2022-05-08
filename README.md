
<strong>1 Player Control Scheme</strong>

Building the control scheme for the game is an important task. A great control scheme can make or break a game, and the following describes the control scheme of our game:

The basic rule is simple: The user can use the arrow keys on the keyboard to navigate Pac-Man. The movement of Pac-Man will be updated instantaneously to the screen for the user.
We used X and Y coordinates to achieve the implementation of character control. First, control the movement direction of the Pac-Man. When player press the arrow key Up (↑) and there is no Obstacle on the current position of the Pac-Man (x, Y-1), then the Pac-Man will change the movement direction to the north and rotate the image of the Pac-Man. Similarly, press Down (↓), Left (←), and right (→) to perform corresponding actions. Second, to control the movement of the Pac-Man and make it move automatically. We used the same judgment method, when the Pac-Man's North=1 and there are no obstacles in the upper (North) direction, then the Pac-Man moves forward by one unit. Similarly, when South, West, and East each value is "1", the Pac-Man moves forward by one unit in the corresponding direction.

<strong>2 Unique Scripting Implementations</strong>

Unique scripting implementations are those created by the team and distinct from any online examples.

2.1 Random Movements of Ghosts

For the random movements, we first determine the current direction of the ghost, then determine the direction in which it can move, and finally randomly generate a direction in its available directions. Firstly, the direction in which the ghost can advance is judged, and the size of an integer variable Vychody is used to record the direction in which the ghost can advance. The ghost can advance only when there is no obstacle on the current side. According to the size of variable Vychody, one, two or three of the four directions will be determined. If there are two or more directions, one direction will be randomly generated. If there is only one direction, this direction will be selected.

2.2 Motion Regulation of Ghosts

The motion of ghosts is similar to Pac-Man movement, using X and Y coordinates, the first images shrunk to half of their original size, and then make it within the specified four grid clockwise direction, each time in a grid in a picture, down to half of the original image size at the same time, this is in order to achieve animation effects and so on; The other three colours are the same, but the images and moving positions of the ghosts are slightly different.

<strong>3 Known Issues</strong>

There is a slight l ag in character control, sometimes pressing the arrow keys one time will move the character two units.
The random movement of the ghost may cause the ghost to return to the direction it was previously in.

<strong>4 Future Development</strong>

	More level designs.

	Add lives to Pac-Man and save the player’s  progress.

	Add menu for adjusting background volume.
