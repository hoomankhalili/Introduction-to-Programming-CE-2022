با توجه به دو عدد صحیح مثبت a و b، قطعه کد زیر، چه مقداری را برای c نتیجه خواهد داد؟

```java
c = 0;
while (b > 0) {
   if (b % 2 == 1) c = c + a;
   b = b / 2;
   a = a + a;
}
```
