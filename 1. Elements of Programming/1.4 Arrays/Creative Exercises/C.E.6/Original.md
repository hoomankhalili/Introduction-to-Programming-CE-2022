**Binomial coefficients.** Write a program BinomialDistribution.java that builds and prints a two-dimensional ragged array a such that ```a[n][k]``` contains the probability that you get exactly k heads when you toss a coin n times. Take a command-line argument to specify the maximum value of n. These numbers are known as the binomial distribution: if you multiply each entry in row i by 2^n, you get the binomial coefficients—the coefficients of x^k in (x+1)^n—arranged in Pascal's triangle. To compute them, start with ```a[n][0] = 0.0``` for all n and ```a[1][1] = 1.0```, then compute values in successive rows, left to right, with ```a[n][k] = (a[n-1][k] + a[n-1][k-1]) / 2```.    

```
Pascal's triangle   Binomial distribution
--------------------------------------------
1                   1 
1 1                 1/2  1/2 
1 2 1               1/4  1/2  1/4 
1 3 3 1             1/8  3/8  3/8  1/8 
1 4 6 4 1           1/16 1/4  3/8  1/4  1/16
```
