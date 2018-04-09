Printing out a list of String :

```java
// Java 7
for (String s : list) {
    System.out.println(s);
}
// Java 8
list.forEach(System.out::println);
```