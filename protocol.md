---
layout: default
title: Queen's Protocol
nav_order: 2
---

# Queen's Protocol

In the effort of implementing real object-oriented applications, the Queen programming language comes with a strict set of rules.

1. Any public methods of a class should be declared in an interface.
2. A class is either abstract or final, no in-between.
3. Attributes of a class cannot be public.
4. No static attributes or static void methods (with the exception of the main method).
5. Immutable-first: all variables (class variables, method variables or parameters) are final by default.
6. Null-safety.
7. No Enums allowed. Enums are actually good in very few cases, yet they encourage shallow and meaningless abstractions.