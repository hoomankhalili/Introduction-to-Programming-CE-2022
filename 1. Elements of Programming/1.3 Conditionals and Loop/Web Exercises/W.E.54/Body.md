اگر مقدار N = 5 باشد برنامه Circle.java چه چیزی را چاپ می کند؟
```java
for (int i = -N; i <= N; i++) {
   for (int j = -N; j <= N; j++) {
      if (i*i + j*j <= N*N) System.out.print("* ");
      else                  System.out.print(". ");
   }
   System.out.println();
}
```
