What is the value of the variable s after running the following loop when N = 1, 2, 3, 4, and 5.
````java
String s = "";
for (int i = 1; i <= N; i++) {
   if (i % 2 == 0) s = s + i + s;
   else            s = i + s + i;
}
````
