#### Java Static Keyword [https://www.journaldev.com/996/java-inner-class]

* Java static variable: A class level variable, deosn't belong to instances of the class but class only.
* Java static method: A class level method, doesn't belong to instances of the class but class only. Usually used for utility methods. Can access static variables only. Can invoke static methods only.
* Java static block: Group of statements that gets executed when the class is loaded into the memory by Java ClassLoader. Mostly used to create or initialize static resources whe the class is loaded. Can ony access static variables in static block.
* Java static class: use static keyword with nested classes. Generally used with nested classes for packaging convenience.
* Java static import: Normally we access static members using class reference. We can use static import to avoid class reference.
  Eg. 
  ```import static com.temp.example.ClassName.VARAIBLE_NAME```

#### Java Inner Class [https://www.journaldev.com/996/java-inner-class]

It is defined inside the body of another class.

Java nested classes are divided into two types:
  * Static nested class: If nested class is static, can only access static members of outer class
  * Java inner class: Any non-static nested class

Java Inner class is associated with instance of the class and is able to access all variable and methods of the outer class. Object of inner class is part of object of outer class, so to create an instance of inner class we first need to create and instance of outer class.

There are two special kinds of java inner classes:
  * Local inner class 
    * A class is defined in a method body. 
    * Local inner class is not associated with object, so we can't use private, public or protected modifiers with it. Only allowed modifiers are abstract and final.
    * Local inner class can access all members of enclosing class and local final variables in the scope it's defined.
  * Anonymous inner class
    * A local inner class without a name.
    * It's defined and instantiated in a single statement.
    * Anonymous inner class always extend or implement an interface.
    * It is not possible to define a constructor for an anonymous class as it has no name.
    * Anonymous inner class is accessible only at the point where it is defined.
    
Benefits of Java inner class:
  * If a class is useful to only one class, it makes sense to keep it nested and together. It helps in packaging of the classes.
  * Java inner classes implement encapsulation. Note that inner classes can access outer class private members and at the same time we can hide inner class from outer world.
  * Keeping the small class within top-level classes places the code closer to where it is used and makes code more readable and maintainable.
