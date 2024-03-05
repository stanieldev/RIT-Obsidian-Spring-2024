### Maxwell equation
 - Domain decomposition
 - Synchronization
 - Time Derivatives
 - Boundaries
We assume there is no periodicity.

With $n$ cells, we break up the domain into equal partitions, where $x_0 = x_{kn}$ for $k\in\mathbb{Z}$
Each processor will have the main value and a ghost zone $\pm1$ indexed around it.
With periodic systems, we wrap around to the other end, but the same principle applies.

Each cell has a local grid, with a lower left, and upper right, as well as their neighbors.
For a 3d grid, a equipartition in all dimensions would have a rank 0 to 7.

112 in Ternary is the center of a 3x3x3 grid.
Up 1 Z, In 1 Row, 2nd on that next row.
= 222 - 110 (Subtract 1 from all but last to be on "top" of the section).