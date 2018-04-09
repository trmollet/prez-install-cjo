* An interface can have **one or more** default methods and still be functional

```java
@FunctionalInterface
public interface Iterable {

	Iterator iterator();

    default void forEach(Consumer<? super T> action) {
		Objects.requireNonNull(action);
		for (T t : this) {
			action.accept(t);
		}
	}
}
```