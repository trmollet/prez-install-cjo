### Temporal Adjusters

* Useful methods to adjust date or time:

  * firstInMonth(DayOfWeek)
  * next(DayOfWeek)
  * previous(DayOfWeek)
  * ...

```java
LocalDate today = LocalDate.now();
LocalDate nextTuesday = today.with(TemporalAdjusters.next(DayOfWeek.TUESDAY));
```