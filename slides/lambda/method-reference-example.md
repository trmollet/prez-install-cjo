#### Example

```java
Arrays.sort(populationArray,
    (Person a, Person b) -> {
        return a.getBirthday().compareTo(b.getBirthday());
    }
);
Arrays.sort(populationArray,
    (a, b) -> Person.compareByAge(a, b)
);
Arrays.sort(populationArray, Person::compareByAge);
```