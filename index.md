---
layout: default
title: Home
nav_order: 1
---

## The Queen programming language (Queenlang)

Queen is an object-oriented JVM language similar to Java. Queen's syntax started from and remains quite close to Java 8. However, there are three main architectural differences:

- immutability by default (instance fields and method parameters are final by default);
- classes are either abstract or final;
- all public instance methods must be declared in an interface or super class;

Read more in Queen's [protocol](/protocol.html).

## Download

The CLI Transpiler can be downloaded from our Github Packages page. More [here](https://github.com/jvmqueen/queen-of-java).

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

    public static void main(String[] args) {
        System.out.println("Hello world!");
    }
}
```
Execute the file like this:

```bash
$ java -jar queenc.jar -f EntryPoint.queen && java ./org/queenlang/helloworld/EntryPoint.java
$ Queen says Hello World!
```
The first command transpiles the Queen file into a Java file, while the second command simply executes it.

### Development of Queenlang

The Queen programming language is developed and maintained on Github, under the [jvmqueen](https://github.com/jvmqueen) Organization. Feel free to contribute or open any Issues you might have. We will help you with any question or problem.

### Roadmap

Queen's roadmap is described [here](/roadmap.html).
