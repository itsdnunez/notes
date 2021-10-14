## Maze robot

## Absolute directions

> NORTH, EAST, SOUTH, WEST

Each are int values and when + 1, it refers to the next direction 90 degrees clockwise

## Relative direction to robot

> LEFT, RIGHT, AHEAD, BEHIND, CENTRE(null) 

Also type int with the same relation 

All references to headings and direction are done with the constant name

Use interface name IRobod when referring to constants

> e.g. Irobot.AHEAD

## Sensing 

Method robot.look(direction) returns a value from a relative direction (LEFT, etc.) showing the state of that square 

> IRobot.PASSAGE(unvisited squares), IRobot.WALL, IRobot.BEENBEFORE 


