#### Collect multiple statistics about a collection

```java
// Compute the count of people, as well as the minimum, maximum, sum, and average of their number of dependents
IntSummaryStatistics stats = people.stream()
                                   .collect(Collectors.summarizingInt(Person::getDependents));
System.out.println(stats.getAverage());
System.out.println("count = " + stats.getCount());
System.out.println("max = " + stats.getMax());
System.out.println("min = " + stats.getMin());
```