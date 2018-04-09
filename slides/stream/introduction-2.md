* Supports the filter / map / reduce pattern
* Elements in a stream are **lazily** evaluated

```java
List<String> list = persons.stream()
        .filter(person -> person.getAge() < 40)
        .map(Person::getName)
        .collect(Collectors::toList);
```

Stream + lambdas = basis of functional-style programming in Java 8