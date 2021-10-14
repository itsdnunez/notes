## Maze robot

## Absolute directions

> NORTH, EAST, SOUTH, WEST

Each are int values and when + 1, it refers to the next direction 90 degrees clockwise.

## Relative direction to robot

> LEFT, RIGHT, AHEAD, BEHIND, CENTRE(null) 

Also type int with the same relation. 

All references to headings and direction are done with the constant name.

Use interface name IRobot when referring to constants.

> e.g. Irobot.AHEAD

## Sensing 

Method robot.look(direction) returns a value from a relative direction (LEFT, etc.) showing the state of that square. 

> IRobot.PASSAGE(unvisited squares), IRobot.WALL, IRobot.BEENBEFORE 

### Robot's current heading 

> robot.getHeading()

Returns current heading relative to absolute direction in the maze. 

> IRobot.setHeading(x)

Sets the heading of the robot.

### Location of robot and target

> robot.getLocation(), robot.getLocation().x or robot.getLocation().y
> Can also use robot.getTargetLocation() similarly

Returns object called 'Point' with 2 variables, the x and y co-ordinates of the robot.

Top left square being (1,1).

### Start of a run and change of maze

> robot.getRuns() 

Returns an int showing the previous runs on a maze.

## Movement 

The robot's movement is polled - your code will be called each time the environment is ready to move the robot.

The purpos of the code is point the robot's direction then the controller will automatically advance in the direction the robot is facing.

### Turns 

> robot.face(direction) 

Turns to direction specified relative to current heading.

### RNG

Math.random() generates a random floating point number 0 <= x < 1. 

To generate random numbers take the result and multiply it by n then use Math.round(x) to round it to the nearest integer. 



