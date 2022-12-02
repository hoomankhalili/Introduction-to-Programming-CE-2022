for ";" :
```
HelloWorld.java:3: error: ';' expected
		System.out.println("Hello, World!")
		                                   ^
1 error
```
for first " : 
```
HelloWorld.java:3: error: ')' expected
		System.out.println(Hello, World!");
		                               ^
HelloWorld.java:3: error: unclosed string literal
		System.out.println(Hello, World!");
		                                ^
HelloWorld.java:3: error: ';' expected
		System.out.println(Hello, World!");
		                                   ^
HelloWorld.java:6: error: reached end of file while parsing
}
 ^
4 errors
```
for second " :
```
HelloWorld.java:3: error: unclosed string literal
		System.out.println("Hello, World!);
		                   ^
HelloWorld.java:3: error: ';' expected
		System.out.println("Hello, World!);
		                                   ^
HelloWorld.java:6: error: reached end of file while parsing
}
 ^
3 errors
```
for first " { " : 
```
HelloWorld.java:1: error: '{' expected
public class HelloWorld
                       ^
1 error
```
for second " { " :
```
HelloWorld.java:2: error: ';' expected
	public static void main(String[] args)
	                                      ^
HelloWorld.java:6: error: class, interface, or enum expected
}
^
2 errors
```
for first " } " :
```
HelloWorld.java:6: error: reached end of file while parsing
}
 ^
1 error
```
for second " } " :
```
HelloWorld.java:5: error: reached end of file while parsing
	}
	 ^
1 error
```
