### Files as Stream

Read a file as a Stream using `Files.lines(Path filePath)`:

```java
try (Stream st = Files.lines(Paths.get("/path/to/file"))) {
    st.forEach(System.out::println);
}
```
Navigate file trees using a Stream using static methods on the **Files** class:
```java
// Stream of files in the given directory
list(Path dir)
// Stream that traverses the file tree depth-first starting at the given directory
walk(Path dir)
// Same as walk(dir) but with a maximum depth
walk(Path dir, int maxDepth) 
```
note: Any `IOException` that is thrown while processing the file (after the file is opened) will get wrapped in an `UncheckedIOException` and thrown