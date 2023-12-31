# SPOJ Laser Phones - Laser Phones

The cows have a new laser-based system so they can have casual conversations while out in the pasture which is modelled as a W × H grid of points (1 <= W <= 100; 1 <= H <= 100).

The system requires a sort of line-of-sight connectivity in order to sustain communication. The pasture, of course, has rocks and trees that disrupt the communication but the cows have purchased diagonal mirrors ('/' and '\' below) that deflect the laser beam through a 90 degree turn. Below is a map that illustrates the problem.

H is 8 and W is 7 for this map. The two communicating cows are notated as 'C's; rocks and other blocking elements are notated as '*'s:

7 . . . . . . .         7 . . . . . . .
6 . . . . . . C         6 . . . . . /-C
5 . . . . . . *         5 . . . . . | *
4 * * * * * . *         4 * * * * * | *
3 . . . . * . .         3 . . . . * | .
2 . . . . * . .         2 . . . . * | .
1 . C . . * . .         1 . C . . * | .
0 . . . . . . .         0 . \-------/ .
  0 1 2 3 4 5 6           0 1 2 3 4 5 6
  
Determine the minimum number of mirrors M that must be installed to maintain laser communication between the two cows, a feat which is always possible in the given test data.

Input

Line 1: Two space separated integers: W and H.
Lines 2..H+1: The entire pasture.

Output

Line 1: A single integer: M.

Example

Input:

7 8
.......
......C
......*
*****.*
....*..
....*..
.C..*..
.......

Output:

3
