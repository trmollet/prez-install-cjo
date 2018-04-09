#### FlatMap

```java
Stream.of(new Developer("polyglot").knows("scala").knows("groovy"),
		  new Developer("pragmatic").knows("java").knows("javascript"))
      .map(d -> d.getLanguages())
      .flatMap(l -> l.stream())
      .forEach(System.out::println);
```
