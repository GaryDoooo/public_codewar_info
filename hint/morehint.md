
```
+---+                          +---+
| A |                          | A |
+---+---+---+---+      +---+---+---+---+
| B | D | E | F |      | B | D | E | F | 
+---+---+---+---+      +---+---+---+---+
| C |                      | C |
+---+                      +---+
```
The above two nets are equivalent. The finished 3D cubes from these two nets have all the 6 faces A, B, C, D, E and F in the same positions. The square A will connect to B, D, E and F in the end. But just use one of its edges to connect to the net, while they are different edges to connect to B and E. Same situation applies to square C.

I quoted a website in the Kata description. There is a paper in the website, which uses edges welding to analysis the 3D net. It's like using welding corners to solve the 2D net for a cube... Try not to use that approach.
