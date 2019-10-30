# avdv-point-group
Write an executable that calculates the point group operations of an arbitrary 2D lattice.
Lattice vectors must be inputted through a file, which contains the *a* and *b* vectors as columns.
Your program should print out the size of the point group, followed by the Cartesian matrix representations for each operation.

## Example
A file named `triangular.txt` contains the lattice vectors for a triangular lattice:
```
1.0        -0.5      
0.0         0.8660254
```

The program to find the point group has been compiled as `avdv-find-point-group`.
Running
```
avdv-find-point-group triangular.txt
```
outputs (trucated):
```
The 12 operations of the lattice are:


 1.0 0.0
 0.0 1.0
 ------------------

 0.5       -0.8660254
 0.8660254  0.5      
 ------------------

-0.5       -0.8660254
 0.8660254 -0.5      
 ------------------

-1.0  0.0
 0.0 -1.0
 ------------------

-0.5        0.8660254
-0.8660254 -0.5      
 ------------------

 0.5        0.8660254
-0.8660254  0.5      
 ------------------

 1.0  0.0
 0.0 -1.0
 ------------------
...

```

## Requirements
* Written in c++
* Final product available through git
* Provide a Makefile or bash script that will compile your program
* Works for any 2D lattice, inputted as a file
* Prints number of operations in point group
* Prints the matrix of each point group operation
* Written by you (no sharing code)

## Bonus points
* Well structured code (e.g. delegating tasks to functions or classes)
* Readable code
* Prove results are correct by showing group is closed
* Print multiplication table of point group
