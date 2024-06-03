# MazeCreator
a small console application, that creates diferrent mazes of ,as I it percieve, a medium quality. Nothing, but a small practice of my python skills.

# How it works?
I have invented a weird algorithm of bounding spaces with back- and forward slashes and thought, that it could be a good idea to develop it further. I will describe the principes in following
1. Fill the square net with back- or forwardslashs by the rules: "/" cannot be neighbored to "\" and "/" so, that they form a connected line.
For example, it is not allowed to form the following nets:
\/\

\\\
//

if you put this symbols together, you will have a line. The following example is permitted:

////
/ /
 \
 by some reason, if we continue to fill the net in the same manner, we won't get "thick walls", that is, a group of walls 3x3 and bigger.
 So we fill each square of the net, ande if either "/" or "\" cannot be put in one of them, we let it stay empty
 2. Then we put the wall symbol - "O" - insted of slashs. On this point we are usually going to get a maze with a planty of small spaces, which are not connected to each other.
 To extend the maze, I additionaly run the "wall breaker" algorithm three times, that is, I connect them by replacing "O" symbol to " " inbetween
 
3. After that the maze will still look pretty ugly, but you don't have to do much in order to complete it. Just connect remaining separate spaces and close holes on the outer wall. I have also uploaded an example of a possible maze. That is!
