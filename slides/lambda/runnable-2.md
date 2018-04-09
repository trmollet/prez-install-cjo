```java
import static java.lang.System.out;

public class Hello {
  Runnable r1 = () -> out.println(this);
  Runnable r2 = () -> out.println(toString());

  public String toString() {
    return "Hello, world!";
  }

  public static void main(String... args) {
    new Hello().r1.run(); //Hello, world!
    new Hello().r2.run(); //Hello, world!
  }
}
```

note: Have a look at the same implementation in Java 7. Reference to _this_ and _toString()_ are way more complicated.
