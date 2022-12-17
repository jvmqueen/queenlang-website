---
layout: default
title: Queen's Protocol
nav_order: 2
---

# Queen's Protocol

In the effort of implementing real object-oriented applications, the Queen programming language comes with a strict set of rules.

1. Any public instance methods should be declared in an interface.
2. A class is either abstract or final, no in-between.
3. Immutable-first: all instance fields and method parameters are final by default.
4. Fields of a class cannot be public (except static constants).
5. No static void methods (with the exception of the main method).
6. Null-safety.
7. No Enums allowed. Enums are actually good in very few cases, yet they encourage shallow and meaningless abstractions.