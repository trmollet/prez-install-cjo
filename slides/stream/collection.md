### Collections as Stream

The Collection interface has two default methods on it for creating streams:

- stream(): Returns a sequential Stream with the collection as its source
- parallelStream(): Returns a possibly parallel Stream with the collection as its source