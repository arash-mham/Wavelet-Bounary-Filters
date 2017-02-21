
These 4 files can be viewed as plain text or used in MATLAB (hence the .m extension on their names).

Each file contains a succession of P, A, B, or Q filters for short boundary curves.  The succeswsions run from the shortest boundary curve (4 vertices) up to 13-vertex curves, after which the interior vertices of any boundary curve behave according to the cyclic filters given as the last entry in every file.

For example in file BoundaryPMatrices.m:

   P10x4 embodies the subdivision of a 4-vertex curve into a 10-vertex curve
   P13x5 embodies the subdivision of a 5-vertex curve into a 13-vertex curve
   P16x6 embodies the subdivision of a 6-vertex curve into a 16-vertex curve
   P19x7 embodies the subdivision of a 7-vertex curve into a 19-vertex curve
   P22x8 embodies the subdivision of an 8-vertex curve into a 22-vertex curve
   P25x9 embodies the subdivision of a 9-vertex curve into a 25-vertex curve
   P28x10 embodies the subdivision of a 10-vertex curve into a 28-vertex curve
   P31x11 embodies the subdivision of an 11-vertex curve into a 31-vertex curve
   P34x12 embodies the subdivision of a 12-vertex curve into a 34-vertex curve
   P37x13 embodies the subdivision of a 13-vertex curve into a 37-vertex curve
and
   CyclicP embodies the subdivision of an 11-vertex curve into a 31-vertex curve, but more importantly its columns all express the general column pattern that appears first in P25x9 and continues on as the central column pattern for all larger P matrices.  One should use the P matrices from 10x4 through 25x9 as given.  From then on, any larger P matrix may be formed by adding further central columns to appropriately enlarged versions of P25x9, and one can check that this is being done correctly by looking at P28x10 through P37x13.

The matrices in the other files offer corresponding models for A, B and Q.