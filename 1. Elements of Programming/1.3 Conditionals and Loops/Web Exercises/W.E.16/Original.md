Given two positive integers a and b, what result does the following code fragment leave in c

```java
c = 0;
while (b > 0) {
   if (b % 2 == 1) c = c + a;
   b = b / 2;
   a = a + a;
}
```
