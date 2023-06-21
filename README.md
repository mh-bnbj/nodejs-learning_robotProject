# nodejs-learning_robotProject

This is robot movement project for learning nodejs course

## what does this app do :

Draw a 5x5 checkerboard

The robot should be placed in SOUTH WEST, i.e. point (0,0).

A command file should be given to the system, which can contain the following commands in each line:

-   PLACE X,Y,F
    Set the robot at the X and Y points, and the direction of F: NORTH/SOUTH/WEST/EAST

-   MOVE
    The robot moves forward one step in the F direction. Note that the bot cannot leave the board

-   LEFT
    The robot rotates in the anti-clockwise direction

-   RIGHT
    The robot rotates clockwise

-   REPORT
    The robot reports where it is.

## how app runs:

there is two way to use robot and send command :

-   by commands.txt file and console

-   by html webPage and webServer

### text file

first you should write down all the commands in commands.txt file line by line

after that run this code to start project :

    $ npm run startFile

then as you can see on console, first it read the commands.txt and extract commands and then it will run the command and will return the result

### webServe

commands.txt file is not necessary in this method

first run this code to start project :

    $ npm run startServer

it will start server on 127.0.0.1 (localhost) on port 3000

if you open "http://127.0.0.1:3000/mainPage" in you browser you can use the "command" input and "send command" button on html WebPage to write command and send it to webServer which there it will process and use the robotModel and respond the result and it will be shownd in the left 5\*5 table.

you can also se you previous command and its result in the right box
