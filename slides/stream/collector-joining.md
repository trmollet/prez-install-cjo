#### Joining (similar to Apache Commons’ **StringUtil.join**)

```java
String names = persons.stream()
        .map(Person::getName)
        .collect(Collectors.joining(", "));
```