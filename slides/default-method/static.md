### Not only default methods

* **Static** method is allowed in interface too in Java 8

```java
public interface Stream {
  ...

  /**
   * Returns a sequential ordered stream whose elements are the specified values.
   *
   * @param <T> the type of stream elements
   * @param values the elements of the new stream
   * @return the new stream
   */
  public static<T> Stream<T> of(T... values) {
    return Arrays.stream(values);
  }
}
```