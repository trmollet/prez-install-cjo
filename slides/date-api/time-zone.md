### Time zones

* Represented by `java.time.ZoneId`

```java
// Print out all available time-zone IDs
System.out.println(ZoneId.getAvailableZoneIds());

// Several ways to get an instance of a ZoneId
ZoneId mountainTime = ZoneId.of("America/Denver");
ZoneId myZone = ZoneId.systemDefault();

// Create a ZonedDateTime
LocalDateTime now = LocalDateTime.now();
ZonedDateTime zdt = now.atZone(myZone);
```