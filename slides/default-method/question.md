### Question
What if a class implements two interfaces and both interfaces define a default method with the same signature ?
```java
interface Foo {
	default void talk() {
		out.println("Foo!");
	}
}
interface Bar {
	default void talk() {
		out.println("Bar!");
	}
}
class FooBar implements Foo, Bar {
	@Override
	void talk() { Foo.super.talk(); }
}
```