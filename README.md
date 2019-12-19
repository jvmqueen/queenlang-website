## The Queen programming language (Queenlang)

Queen <strike>is</strike> will be an object-oriented JVM language very similar to Java. In fact, you can think of it as Java with a **very strict** protocol. Queen takes Java and tries to remove everything that goes against the pinciples of Object-Oriented Programming.

### Hello World

Similarly to Java, the entry point of a Queen application is a *main* method. However, this method is not static and the class implementing this method actually implements the ``Main`` interface (there can be only one implementation of ``Main`` per application).

```java
/**
 * Entry point of our Queen application.
 */
public final EntryPoint implements Main {
    public void main(String[] args) {
        println("Hello world! I am your queen!");
    }
}
```
