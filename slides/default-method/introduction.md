## Default methods
* Put code in interfaces
* Add methods in existing interfaces without breaking existing implementations

```java
public interface Stream {
  ...

  default public Stream stream() {
    return StreamSupport.stream(spliterator());
  }
}
```