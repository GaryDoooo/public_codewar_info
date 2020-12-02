# Four Color Theorem for Cylindrical Projection Hints

This Kata will have maps with 90 territories. As far as I know, trying all color combinations by brute force will time out. To ensure one map can be colored with 2 or 3 colors need go through each part of the map, but quickly.

We can simplify the problem to just look at each territory and its neighbors. If one territory's all neighbors need 3 colors to paint, then this territory has to be the 4th color. Then the question becomes how many colors is needed for its neighbors.
```
      1                 1                ---1---
      |                 |                |  |  |
      |                 |                |  |  |
      2                 2                |  2  |
     / \               / \               | / \ |
    /   \             /   \              |/   \|
   3     4           3-----4             3-----4

```
In the examples, vertex 2 has three neighbors: 1, 2, and 4.
1. In the first scenario, 1, 2, and 4 do not connect to each other. So they can have a same color. Vertex 2 thus can have the 2nd color;
1. In the scenario in the middle, 3 and 4 connect to each other. So they have to use two different colors. Vertex 2 neighbors need total two colors. Thus the Vertex 2 need take the 3rd color.
1. The last one is the simpliest connection which need four colors. 

But real possible connections on a cylinder will have trickier cases. Simply looking at one vertex's neighbors is not enough. 

This's just about how I solved the problem. There must be better ways. 

I even don't know if the algorithm works all correctly. So far by my manually checking, its output looks right. In case you find any errors, please don't hesitate to let me know. Thanks!

GLHF
