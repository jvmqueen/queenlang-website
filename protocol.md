---
title: Queen's Protocol
#has_children: true
nav_order: 2
---

# Queen's Protocol

In the effort of implementing real object-oriented applications, the Queen programming language comes with a strict set of rules.

1. Any public method of a class should be declared in an interface.
2. A class is either abstract or final.
3. Attributes of a class cannot be public.
4. No static attributes or static void methods.
5. No null! Queen does not have the concept of null. Instead, in Queen, we say that an object is **missing** (there's more to this than just a name change). 
6. All variables (class variables, method variables or parameters) are final -- they can be attributed only once.
7. Naming restrictions. For instance, variables must have at least 3 characters in their name.
