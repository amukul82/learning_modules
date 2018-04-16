#### JAVA Static kweyword

* Java static variable: A class level variable, deosn't belong to instances of the class but class only.
* Java static method: A class level method, doesn't belong to instances of the class but class only. Usually used for utility methods. Can access static variables only. Can invoke static methods only.
* Java static block: Group of statements that gets executed when the class is loaded into the memory by Java ClassLoader. Mostly used to create or initialize static resources whe the class is loaded. Can ony access static variables in static block.
* Java static class: use static keyword with nested classes. Generally used with nested classes for packaging convenience.
* Java static import: Normally we access static members using class reference. We can use static import to avoid class reference.
  Eg. 
  ```import static com.temp.example.ClassName.VARAIBLE_NAME```
