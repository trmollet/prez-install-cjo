Deal with missing values using:
```java
// return a default value if the Optional is empty
orElse(T);
// call a given Supplier to provide a value if the Optional is empty
orElseGet(Supplier<T>)
// call a given Supplier for an exception to throw if the Optional is empty
orElseThrow(Supplier<X extends Throwable>)
```