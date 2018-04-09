### Practice

Rewrite following method using `Optional`:

```java
public String getNickname(Person person) {
    if (person != null) {
        return person.getNickname();
    }
    return Person.defaultNickname();
}
```