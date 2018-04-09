Imagine `getCurrentServiceContext(...)` returns an `Optional<ServiceContext>`.  

Rewrite following method using `Optional`:

```java
public String getSessionId(String subSettingPrefix) {
    String result;
    ServiceContext current = getCurrentServiceContext(subSettingPrefix);
    if (current != null) {
        result = current.getSessionId();
    } else {
        // Else take the current session id
        BusinessSessionManagementDelegate delegate = new BusinessSessionManagementDelegate();
        result = delegate.getSessionId();
    }
    return result;
}
```
