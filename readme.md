# CAD Perimeter Product
In this problem, a list of line segments is given, and each segment has the coordination of its start and end points as:

[((x1, y1), (x2, y2)), …] 

I want to calculate the multiplicative product of
all perimeters of all the individual enclosed areas. To solve this problem, I used graph theory and considered each line segment as the edge of the graph, and all points as nodes of the graph. Then,
using graph modeling, find all unique sub-loops, then calculate their perimeters. 

# Repository organization
This repository has one main file, main.py, and two helper files.



**- model.py**: Compute perimeter product for entered line segments

```
usage: python3 main.py [-h] -e input_edges
positional arguments:
  input_edges  Two edges (list points) and a precision parameter for rounding the float numbers.

Returns:
  1) List of all new sub-edges
  2) List of all available intersections (new nodes)
  3) List of all unique sub-cycles
  4) List of perimeters of all unique sub-cycles
  5) Product of all perimeters (float number)
```


