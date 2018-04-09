### Infinite streams

Use the **generate** or **iterate** static methods on Stream:

````java
Stream.generate(() -> Math.random())
      .forEach(System.out::print);
````

```java
Stream.iterate(1, i -> i+1)
      .forEach(System.out::print);
```
