for main:
```
HelloWorld.java:2: error: <identifier> expected
	public static void (String[] args) {
	                  ^
1 error
```
for String:
```
 HelloWorld.java:2: error: illegal start of type
	public static void main([] args) {
	                        ^
HelloWorld.java:2: error: ')' expected
	public static void main([] args) {
	                         ^
HelloWorld.java:2: error: ';' expected
	public static void main([] args) {
	                          ^
HelloWorld.java:2: error: illegal start of type
	public static void main([] args) {
	                               ^
HelloWorld.java:2: error: <identifier> expected
	public static void main([] args) {
	                                ^
HelloWorld.java:2: error: ';' expected
	public static void main([] args) {
	                                  ^
HelloWorld.java:3: error: illegal start of type
		System.out.println("Hello, World!");
		      ^
HelloWorld.java:3: error: ';' expected
		System.out.println("Hello, World!");
		          ^
HelloWorld.java:3: error: invalid method declaration; return type required
		System.out.println("Hello, World!");
		           ^
HelloWorld.java:3: error: illegal start of type
		System.out.println("Hello, World!");
		                   ^
HelloWorld.java:6: error: class, interface, or enum expected
}
^
11 errors
```
for HelloWorld:
```
HelloWorld.java:1: error: <identifier> expected
public class {
            ^
1 error
```
for System.out:
```
HelloWorld.java:3: error: illegal start of expression
		.println("Hello, World!");
		^
1 error
```
for println:
```
HelloWorld.java:3: error: <identifier> expected
		System.out.("Hello, World!");
		           ^
1 error
```
