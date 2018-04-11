### Clean Code
#### By Robert C. Martin

#### Intro

* Specifying requirements in such detail that a machine can execute then is <i>programming</i>. Such a specification is <i>code</i>.
* The only way to make the deadline, the only way to go fast, is to keep the code as clean as possible at times.
* Clean code is <i>focused</i>. Each function, each class, each module exposes a single-minded attitude that remains entirely undistracted, and unpolluted, by the surrounding details.
* It is not the language that makes programs appear simple. It is the programmer that makes the language appear simple.
* The Boy Scout Rule - <i>Leave the campground cleaner than you found it</i>.

#### Meaningful names

* Use intention-revealing names : The name of a variable, function or class should tell you why it exists, what it does, and how it is used.

| Bad Code | Good Code |
| :---: | :---: |
| ```int d; //elapsed time in days``` | ```int elapsedTimeInDays;``` |
| ```public List<int[]> getThem(){
        return null;
     }
  ``` |  |