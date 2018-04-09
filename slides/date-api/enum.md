### New Enum's

* `java.time.temporal.ChronoUnit`
* `java.time.DayOfWeek`
* `java.time.Month`

```java
LocalDate today = LocalDate.now();
LocalDate nextWeek = today.plus(1, ChronoUnit.WEEKS);
LocalDate nextMonth = today.plus(1, ChronoUnit.MONTHS);
LocalDate nextYear = today.plus(1, ChronoUnit.YEARS);
```