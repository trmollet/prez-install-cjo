#### Do not use in POJO fields and getters

* Optional deliberately [doesn’t implement the Serializable interface](http://mail.openjdk.java.net/pipermail/jdk8-dev/2013-September/003274.html)
* If your POJO accessors are using Optional it will be more complicated for a library or framework to use reflection to manipulate them
* However some people would like to use Optional this way (like [Stephen Colebourne](http://blog.joda.org/2015/08/java-se-8-optional-pragmatic-approach.html), contributor of Joda-Time)