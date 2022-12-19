کد زیر چه چیزی را چاپ می کند؟
```java
int f = 0, g = 1;
for (int i = 0; i <= 15; i++) {
   System.out.println(f);
   f = f + g;
   g = f - g;
}
```
