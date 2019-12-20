## The Queen programming language (Queenlang)

Queen is an object-oriented JVM language very similar to Java. In fact, you can think of it as Java with a strict protocol. Queen takes Java and tries to remove everything that goes against the pinciples of Object-Oriented Programming.

### Hello World

Similarly to Java, the entry point of a Queen application is the *main* method. However, this method is not static and the class implementing this method actually implements the ``org.queenlang.api.Main`` interface (there can be only one implementation of ``Main`` per application). One key difference is that, in Queen, classes are named **implementations** and the keyword **implements** is replaced by **of**.

``EntryPoint.queen``:
```java
package org.queenlang.helloworld;
import org.queenlang.api.Main;

/**
 * Entry point of our Queen application.
 * @author amihaiemil (amihaiemil@gmail.com)
 * @version $Id$
 * @since 0.0.1
 */
public final implementation EntryPoint of Main {

    @Override
    public void main(final String[] args) {
        println("Hello world!");
    }
}
```

### Development of Queenlang

The Queen programming language is developed and maintained on Github, under the [jvmqueen](https://github.com/jvmqueen) Organization. Feel free to contribute or open any Issues you might have. We will help you with any question or problem.
