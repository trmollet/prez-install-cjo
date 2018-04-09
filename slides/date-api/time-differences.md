### Time differences

* Period - **date**-based amount of time (such as "2 years, 3 months and 4 days")
* Duration - **time**-based amount of time (such as "34.5 seconds")

```java
Period p = Period.between(date1, date2);
Duration d = Duration.between(time1, time2);
```

```java
// static methods
Duration twoHours = Duration.ofHours(2);
Duration tenMinutes = Duration.ofMinutes(10);
Duration thirtySecs = Duration.ofSeconds(30);

// add/substract period or duration from a date or time
LocalTime t2 = time.plus(twoHours);
```