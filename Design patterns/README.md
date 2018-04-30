### Design Patterns

#### Singleton vs Dependency Injection (http://enterprisecraftsmanship.com/2016/05/03/singleton-vs-dependency-injection/)

Singleton classes are the ones which have only one instance of of that class for the whole application lifetime.

Dependency Injection is used for passing instances of objects to the other dependent objects.

Ambient dependencies are the ones which span accross multiple classes and often multiple layers.

* If a dependency is ambient, use singletons.
* Otherwise, inject it to the dependent classes using the dependency injection pattern.

#### Singleton Design Pattern (https://www.journaldev.com/1377/java-singleton-design-pattern-best-practices-examples)
