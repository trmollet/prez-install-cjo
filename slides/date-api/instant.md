### Instant

* **Instant** measures time starting from the “epoch” (Jan. 1, 1970)
* Time-zone ignorant
* Basis of time measurements in the Java 8

```java
Instant instant = Instant.now();
Instant instant2 = Instant.now();

System.out.println(instant.isBefore(instance2));
```