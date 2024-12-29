# CAD Perimeter Product
In this problem, a list of line segments is given, and each segment has the coordination of its start and end points as:

[((x1, y1), (x2, y2)), …] 

I want to calculate the multiplicative product of
all perimeters of all the individual enclosed areas. To solve this problem, I used graph theory and considered each line segment as the edge of the graph, and all points as nodes of the graph. Then,
using graph modeling, find all unique sub-loops, then calculate their perimeters. 

There are one main file, main.py, and two helper files in this repository.


