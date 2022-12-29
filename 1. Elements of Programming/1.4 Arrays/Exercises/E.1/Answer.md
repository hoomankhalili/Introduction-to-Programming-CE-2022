This program compiles cleans.
When n is 1000, it leads to the following error

* java.lang.NegativeArraySizeException
 
because 1000^4 overflows an int and results in a negative integer.
When n is 200, it leads to the following error

 * java.lang.OutOfMemoryError: Requested array size exceeds VM limit
