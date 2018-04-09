#### Partitioning

```java
// Group by whether or not the developer knows Java
Map<Boolean,List<Developer>> map = developers.stream()
        .collect(Collectors.partitioningBy(Developer::knowsJava));
```