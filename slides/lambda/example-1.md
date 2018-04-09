```java
// Function that prefixes a name with @
Function<String, String> atr = (name) -> {return "@" + name;};

// Function that returns length of a String
Function<String, Integer> leng = (name) -> name.length();
Function<String, Integer> leng2 = String::length;
```