#### Grouping

```java
// Group by first letter of name
Map<Character,List<Developer>> map = developers.stream()
        .collect(Collectors.groupingBy(dev -> dev.getName().charAt(0)));
map.forEach((k,v) ->
            System.out.println(k + " " + v.stream()
                               .map(Developer::getName)
                               .collect(Collectors.joining(", "))));
```