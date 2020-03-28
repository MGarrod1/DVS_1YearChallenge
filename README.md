# DVS_1YearChallenge
Code used to create my entry for the Data Visualisation Society's 1st year anniversary challenge.

![](https://github.com/MGarrod1/DVS_1YearChallenge/blob/master/overview.png)

Out of the data about 11573 members I was able to find 2120 unique geographic locations. The figure above visualises a path which passes through all of the locations. At each step the walker jumps to the closest point which has not been visited previously. In the simulation we manage to visit all of the 2120 by travelling a total of 302,079 km. 

This approach is far from the optimal solution which would involve solving the [travelling salesman problem](https://en.wikipedia.org/wiki/Travelling_salesman_problem) on this set of points. I also cheat by allowing the walker to “tunnel” through the earth (since distances are computed from the positions in 3D space) meaning that the distance travelled is underestimated.

# Requirements

The plots were created using Python 3.7 on an Anaconda distribution (conda version : 4.7.12).
