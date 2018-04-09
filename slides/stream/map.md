#### Map

Apply a function to the elements of the stream

```java
List<String> nameList = persons.stream()
                .map(p -> p.getFirstname() + " " + p.getLastname())
                .collect(Collectors::toList);
```
