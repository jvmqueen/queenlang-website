---
layout: default
title: Home
nav_order: 1
---

## The Queen programming language (Queenlang)

Queen is an object-oriented JVM language very similar to Java. In fact, you can think of it as Java with a strict protocol. Queen takes Java and tries to remove everything that goes against the pinciples of Object-Oriented Programming.

### Hello World

Similarly to Java, the entry point of a Queen application is the *main* method. However, the class implementing this method must implement the ``org.queenlang.api.Main`` interface.

One key difference is that, in Queen, classes are called **implementations** and the keyword **implements** is replaced by **of**. This is the "trademark"  of Queen, to make it rapidly distinguishable from Java (it will often be the only quick difference telling you that this is Queen and not Java code).

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

    public static void main(final String[] args) {
        println("Hello world!");
    }
}
```

### Development of Queenlang

The Queen programming language is developed and maintained on Github, under the [jvmqueen](https://github.com/jvmqueen) Organization. Feel free to contribute or open any Issues you might have. We will help you with any question or problem.
