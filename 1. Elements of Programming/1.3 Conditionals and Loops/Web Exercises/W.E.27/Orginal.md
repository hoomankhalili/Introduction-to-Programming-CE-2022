What do the following two code fragments do?
````
for (int i = 0; i < N; i++)
   for (int j = 0; j < N; j++)
       if (i != j) System.out.println(i + ", " + j);

for (int i = 0; i < N; i++)
   for (int j = 0; (i != j) && (j < N); j++)
       System.out.println(i + ", " + j);
````
