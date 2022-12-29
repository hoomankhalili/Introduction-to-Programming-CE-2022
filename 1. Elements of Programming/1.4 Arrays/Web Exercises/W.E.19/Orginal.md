**Spearman's footrule distance.** Given two permutations, Spearman's footrule distance is the L1 distance between the permutations as vectors. Useful in top-k lists.
````
int footrule = 0;
for (int i = 0; i < N; i++)
    footrule = footrule + Math.abs(p[i] - q[i]);
 ````
