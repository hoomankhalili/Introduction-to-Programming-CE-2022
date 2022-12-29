Unlike the harmonic numbers, the sum 1/1 + 1/4 + 1/9 + 1/16 + ... + 1/n² does converge to a constant as n grows to infinity. (Indeed, the constant is π² / 6, so this formula can be used to estimate the value of π.) Which of the following for loops computes this sum? Assume that n is an int initialized to 1000000 and sum is a double initialized to 0.       
```java
(a) for (int i = 1; i <= n; i++) 
       sum = sum + 1 / (i * i);
```
```java
(b) for (int i = 1; i <= n; i++)
       sum = sum + 1.0 / i * i;
```
```java
(c) for (int i = 1; i <= n; i++)
       sum = sum + 1.0 / (i * i);
```
```java
(d) for (int i = 1; i <= n; i++)
       sum = sum + 1 / (1.0 * i * i);
```


