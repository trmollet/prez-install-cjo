Example

```java
public boolean isLocatedNearSopra(Person person) {
     return Optional.ofNullable(person)
       .flatMap(Person::getAddress)
       .map(Address::getStreet)
       .filter(street -> street.contains("Pré Faucon"))
       .isPresent();
 }
```
