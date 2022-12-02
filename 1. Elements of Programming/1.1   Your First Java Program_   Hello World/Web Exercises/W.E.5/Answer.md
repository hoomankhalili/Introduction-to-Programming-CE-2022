for main: 
کامپایل شد ولی:
```
Error: Main method not found in class HelloWorld, please define the main method as:
   public static void main(String[] args)
or a JavaFX application class must extend javafx.application.Application
```
for String:
```
HelloWorld.java:2: error: cannot find symbol
	public static void main(Sring[] args) {
	                        ^
  symbol:   class Sring
  location: class HelloWorld
1 error
```
for HelloWorld:
```
HelloWorld.java:1: error: class HlloWorld is public, should be declared in a file named HlloWorld.java
public class HlloWorld {
       ^
1 error
```
for System.out:
```
HelloWorld.java:3: error: package Sstem does not exist
		Sstem.out.println("Hello, World!");
		     ^
1 error
```
for println:
```
HelloWorld.java:3: error: cannot find symbol
		System.out.pintln("Hello, World!");
		          ^
  symbol:   method pintln(String)
  location: variable out of type PrintStream
1 error
```
