### So when should one use Optional ? &rarr; Method result

* Use Optional as return type when value can be null

```java
public Optional<Address> getAddress() {
    AddressDto address = PersonDao.findAddress(this.id);
    return Optional.ofNullable(address);
}
```