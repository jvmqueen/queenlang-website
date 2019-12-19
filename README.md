## The Queen programming language (Queenlang)

Queen is an object-oriented JVM language very similar to Java. In fact, you can think of it as Java with a **very strict** protocol. Queen takes Java and tries to remove everything that goes against the pinciples of Object-Oriented Programming.

### Hello World

Similarly to Java, the entry point of a Queen application is the *main* method. However, this method is not static and the class implementing this method actually implements the ``org.queenlang.qdk.Main`` interface (there can be only one implementation of ``Main`` per application).

```java
package org.queenlang.helloworld;
import org.queenlang.qdk.Main;

/**
 * Entry point of our Queen application.
 * @author amihaiemil (amihaiemil@gmail.com)
 * @version $Id$
 * @since 0.0.1
 */
public final EntryPoint implements Main {

    @Override
    public void main(String[] args) {
        println("Hello world, I am your queen!");
    }
}
```

### Development of Queenlang

The Queen programming language is developed and maintained on Github, under the [jvmqueen](https://github.com/jvmqueen) Organization. Feel free to contribute or open any Issues you might have. We will help you with any question or problem.
