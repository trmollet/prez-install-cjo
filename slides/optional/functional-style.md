Work with Optional's using functional style methods:
```java
// Executes the given Consumer only if there is a value present (no return value)
ifPresent(Consumer<? super T> consumer)
// If the wrapped value matches the predicate then return an Optional with the value otherwise return an empty Optional
filter(Predicate<? super T> predicate)

// Applies the given mapping Function and returns a new Optional
map(Function<? super T,? extends U> mapper)
// Applies the given mapping Function, unwrap the resulting value and returns a new Optional
flatMap(Function<? super T,Optional<U>> mapper)
```