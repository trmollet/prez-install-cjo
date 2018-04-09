### Create date and time

```java
// Now
LocalDateTime now = LocalTime.now();
```

```java
// new LocalDate for March 15, 2014 is as simple as:
LocalDate date = LocalDate.of(2014, 3, 15);
System.out.println(date.getMonth());
// or
date = LocalDate.of(2014, Month.MARCH, 15);
System.out.println(date.getMonth());

// add time to date
LocalTime time = LocalTime.of(12, 15, 0);
LocalDateTime datetime = date.atTime(time);
```