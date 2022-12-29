**8 queens checker.** A permutation of the integer 0 to n-1 corresponds to a placement of queens on an n-by-n chessboard so that no two queens are in the same row or column. Write a program QueensChecker.java that determines whether or not a permutation corresponds to a placement of queens so that no two are in the same row, column, or diagonal. As an example, the permutation { 4, 1, 3, 0, 2 } is a legal placement:
````
* * * Q * 
* Q * * * 
* * * * Q 
* * Q * * 
Q * * * * 
````
Try to do it without using any extra arrays besides the length n input permutation q. Hint: to determine whether setting q[i] conflicts with q[j] for i < j.

if q[i] equals q[j]: two queens are placed in the same row<br/>
if q[i] - q[j] equals j - i: two queens are on same major diagonal<br/>
if q[j] - q[i] equals j - i: two queens are on same minor diagonal<br/>
