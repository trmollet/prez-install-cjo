#### Filter

Return a stream consisting of the elements that match a given predicate

```java
List<Widget> redWidgets = widgets.stream()
                .filter(w -> w.getColor() == RED)
                .collect(Collectors::toList);
```
