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

The CLI Transpiler can be downloaded from our Github Packages page. More [here](https://github.com/jvmqueen/queen-of-java/tree/master#how-to-use-it).

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
Execute the ~~file~~ project like this:

```bash
$ java -jar queenc.jar --project . --output . && java ./org/queenlang/helloworld/EntryPoint.java
$ ... logging from queenc ... 
$ Queen says Hello World!
```

The first command transpiles the Queen project (in this case, only the file EntryPoint.queen) from the current directory into the same directory, while the second command simply executes the created Java class which is created in a directory structure respecting the declared package (org.queenlang.helloworld).

### Generate Maven Project Scaffold

``queenc`` can generate a Queen-compliant Maven structure which you can use as starting point for your Queen project. By default,
it will just say "Hello World", by using Java, as well as Queen - the two are interoperable, there is a Java class implementing a Queen interface.

In order for this to work, you have to set the ``$QUEEN_PATH`` environment variable, pointing to your ``queenc.jar`` file.
You can also define the queenc alias: ``alias queenc='java -jar $QUEEN_PATH'``, so your command becomes easier to read:

```bash
$ queenc -cm /playground/my-queen-project \
  && cd ~/playground/my-queen-project \
  && mvn clean install \
  && java -jar ./target/my-queen-project.jar
$  
$ ... logging from queenc and maven ...
$
$ [INFO] ------------------------------------------------------------------------
$ [INFO] BUILD SUCCESS
$ [INFO] ------------------------------------------------------------------------
$
$ ...
$
$ Queen says Hello World!
$ In the name of Queen, Java also says Hello World!
```

### Development of Queenlang

The Queen programming language is developed and maintained on Github, under the [jvmqueen](https://github.com/jvmqueen) Organization, by [Silvia Maxima et Co.](https://silviamaxima.eu). Feel free to contribute or open any Issues you might have. We will help you with any question or problem.

### Roadmap

Queen's roadmap is described [here](/roadmap.html).
