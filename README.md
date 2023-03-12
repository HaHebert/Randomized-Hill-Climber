# Randomized-Hill-Climber

This program implements a Randomized Hill Climbing function to experiment with probabilistic search algorithms.

The Randomized Hill Climbing program uses a simple randomized Hill Climbing algorithm to minimize a given function. The RHC function is called thirty-three times with different parameter value combinations to test for the optimal minimized solution. The function uses a starting point (x,y) value that is plugged into the given function to give a starting solution. A random number generator creates two values that are -z,+z which are then added to the starting point values, the new x and y values are plugged into the given function and the solution is stored into a vector. After p iterations, the best solution generated is tested against the original solution, if the generated solution is less than the original solution, the generated solution becomes the new best solution. This process continues until the algorithm cannot generate a better solution than the “best solution”, or until the x or y values become less than -4.5 or greater than +4.5 of the original starting point values. 

Program Language:
•	C++

Function to be Minimized:
•	F(x,y) = (1.5 – x + x * y)^2 + (2.25 – x + x * y * y)^2 + (2.625 – x + x * y * y * y )^2

Parameter Values Used in First 32 Runs:
•	Sp = (2, 2), (1, 4), (-2, -3), (1, -2)
•	P = 80, 500
•	Z = 0.1, 0.002
•	Seed = 1676661595, 10

Parameter Values Used in 33rd Run:
•	Sp = (1, -1)
•	P = 1000
•	Z = 0.0002
•	Seed = 10

Executing Program:
•	No user input needed

Author:
•	Hannah Hebert
