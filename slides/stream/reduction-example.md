Calculate the sum of the members age in a collection :

```java
Integer totalAgeReduce = population.stream()
   .map(Person::getAge)
   .reduce(0, (a, b) -> a + b);
```

```java
Integer totalAge = population.stream()
   .mapToInt(Person::getAge)
   .sum();
```