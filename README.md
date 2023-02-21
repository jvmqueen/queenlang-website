## The Queen programming language (Queenlang)

Queen is an object-oriented JVM language very similar to Java. Queen's syntax started from and remains quite similar to Java 8. However, there are three main architectural differences:

- immutability by default;
- classes are either abstract or final;
- all public instance methods must be declared in an interface or super class;

Read more in Queen's [protocol](/protocol.html).

### Hello World

Similarly to Java, the entry point of a Queen application is the *main* method.

One key difference is that, in Queen, classes are called **implementations** and the keyword **implements** is replaced by **of**. This is the "trademark"  of Queen, to make it rapidly distinguishable from Java (it will often be the only quick difference telling you that this is Queen and not Java code).

Also note that the extension of any Queen file is ``.queen``.

``EntryPoint.queen``:
```java
package org.queenlang.helloworld;

/**
 * Entry point of our Queen application.
 * @author amihaiemil (amihaiemil@gmail.com)
 * @version $Id$
 * @since 0.0.1
 */
public final implementation EntryPoint {

    public static void main(final String[] args) {
        System.out.println("Hello world!");
    }
}
```

### Development of Queenlang

The Queen programming language is developed and maintained on Github, under the [jvmqueen](https://github.com/jvmqueen) Organization. Feel free to contribute or open any Issues you might have. We will help you with any question or problem.
