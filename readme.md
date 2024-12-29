# CAD Perimeter Product
In this problem, a list of line segments is given, and each segment has the coordination of its start and end points as:

[((x1, y1), (x2, y2)), …] 

I want to calculate the multiplicative product of
all perimeters of all the individual enclosed areas. To solve this problem, I used graph theory and considered each line segment as the edge of the graph, and all points as nodes of the graph. Then,
using graph modeling, find all unique sub-loops, then calculate their perimeters. 

# Repository organization
This repository has one main file, main.py, and two helper files.



**>>> model.py**: Compute perimeter product for entered line segments

```
usage: python3 main.py [-h] -e input_edges
positional argument:
  input_edges  Two edges (list points) and a precision parameter for rounding the float numbers.

  The format of input_edges: (list of edges, that each edge is a tuple of start and end points)
    1) A variable name of edges defined in the script:
       (edges_window_1, edges_window_2, edges_window_3,
        edges_window_d_1, edges_window_d_2, edges_window_d_3,
        edges_test).
    2) A list of edges in the format: "[(x1,y1),(x2,y2)],[(x3,y3),(x4,y4)], ..." 

Returns:
  1) List of all new sub-edges
  2) List of all available intersections (new nodes)
  3) List of all unique sub-cycles
  4) List of perimeters of all unique sub-cycles
  5) Product of all perimeters (float number)
```

![Screenshot 2024-12-29 12 23 58 AM](https://github.com/user-attachments/assets/e351f2ba-344a-40ae-97bb-802d6275b3d8)


