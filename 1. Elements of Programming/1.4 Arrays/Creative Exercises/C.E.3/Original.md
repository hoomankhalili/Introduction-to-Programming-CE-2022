**Hadamard matrix.** The n-by-n Hadamard H(n) matrix is a boolean matrix with the remarkable property that any two rows differ in exactly n/2 bits. (This property makes it useful for designing error-correcting codes.) H(1) is a 1-by-1 matrix with the single entry true, and for n > 1, H(2n) is obtained by aligning four copies of H(n) in a large square, and then inverting all of the entries in the lower right n-by-n copy, as shown in the following examples (with T representing true and F representing false, as usual).

```
H(1)  H(2)    H(4)
-------------------
 T    T T   T T T T
      T 0   T 0 T 0
            T T 0 0
            T 0 0 T 

```

Write a program Hadamard.java that takes one command-line argument n and prints H(n). Assume that n is a power of 2
