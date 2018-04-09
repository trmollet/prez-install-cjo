Sorting a list of String :

```java
// Java 7
Collections.sort(list, new Comparator<String>() {
    @Override
    public int compare(String s1, String s2) {
        return s1.length() - s2.length();
    }
});
// Java 8
Collections.sort(list, (s1, s2) -> s1.length() - s2.length());
// or
list.sort(Comparator.comparingInt(String::length));
```