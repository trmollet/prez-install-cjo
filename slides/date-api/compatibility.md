### Backwards Compatibility

* **toInstant()** method to convert existing **Date** and **Calendar** to the new Date-Time API
* Then use **ofInstant(Insant, ZoneId)** to get a **LocalDateTime**

```java
// original Date object
Date date = new Date();

// convert to new API
Instant now = date.toInstant();

// then use new objects
LocalDateTime dateTime = LocalDateTime.ofInstant(now, ZoneId.systemDefault());
```