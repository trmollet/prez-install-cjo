#### Simple Collectors

```java
// Accumulate names into a List
List<String> list = persons.stream()
        .map(Person::getName)
        .collect(Collectors::toList);

// Accumulate names into a TreeSet
Set<String> set = persons.stream()
        .map(Person::getName)
        .collect(Collectors.toCollection(TreeSet::new));
```