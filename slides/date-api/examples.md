#### Example
```java
// Java 7
Calendar cal = Calendar.getInstance();
cal.add(Calendar.HOUR, 8);
Date eightHoursAfter = cal.getTime();
```

```java
// Java 8
LocalTime now = LocalTime.now();
LocalTime eightHoursAfter = now.plus(8, HOURS);
```

```java
LocalDate today = LocalDate.now();

// Well-named methods
// Each method returns a different instance of LocalDate, 'today' is immutable
LocalDate thirtyDaysFromNow = today.plusDays(30);
LocalDate nextMonth = today.plusMonths(1);
LocalDate aMonthAgo = today.minusMonths(1);
```
