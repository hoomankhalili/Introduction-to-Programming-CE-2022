**Parity check.** A Boolean matrix has the parity property when each row and each column has an even sum. This is a simple type of error-correcting code because if one bit is corrupted in transmission (bit is flipped from 0 to 1 or from 1 to 0) it can be detected and repaired. Here's a 4 x 4 input file which has the parity property:
```
1 0 1 0
0 0 0 0
1 1 1 1
0 1 0 1
```
