What does the program Circle.java print out when N = 5?
```java
for (int i = -N; i <= N; i++) {
   for (int j = -N; j <= N; j++) {
      if (i*i + j*j <= N*N) System.out.print("* ");
      else                  System.out.print(". ");
   }
   System.out.println();
}
```
