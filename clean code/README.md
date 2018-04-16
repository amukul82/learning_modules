### Clean Code
#### By Robert C. Martin

#### Intro

* Specifying requirements in such detail that a machine can execute then is <i>programming</i>. Such a specification is <i>code</i>.
* The only way to make the deadline, the only way to go fast, is to keep the code as clean as possible at times.
* Clean code is <i>focused</i>. Each function, each class, each module exposes a single-minded attitude that remains entirely undistracted, and unpolluted, by the surrounding details.
* It is not the language that makes programs appear simple. It is the programmer that makes the language appear simple.
* The Boy Scout Rule - <i>Leave the campground cleaner than you found it</i>.

#### Meaningful names

* Use intention-revealing names
  * The name of a variable, function or class should tell you why it exists, what it does, and how it is used.

  Examples:

  Bad Code:
  ```int d; //elapsed time in days```

  Good Code:
  ```int elapsedTimeInDays;```

  Bad Code:
  ```
  public List<int[]> getThem() {
    List<int[]> list1 = new ArrayList<int[]>();
    for(int[] x : theList11)
      if(x[0] == 4)
        lsit1.add(x);
    return list1;
  }
  ```

  Good Code:
  ```
  public List<int[]> getFlaggedCells() {
    List<int[]> flaggedCells = new ArrayList<int[]>();
    for(int[] cell : gameBoard)
      if(cel[STATUS_VALUE] == FLAGGED)
        flaggedCells.add(cell);
    return flaggedCells;
  }
  ```
* Avoid disinformation
  * Avoid words whose entrenched meaning vary from our intended meaning.
  * Avoid using names which vary in small ways.
  * Spell similar concepts similarly.
* Make meaningful distinctions
  * Avoid adding number series or noise words for distinctions. If names must be different, then they should mean something different.
* Use pronounceable names 
  * Avoid <i>DtaRecrd</i>, use <i>DataRecord</i>.
* Use searchable names
  * Avoid single letter names and numeric constants as they are not east to locate in a body of text.
  * The length of a variable should correspond to the size of its scope.
* Class names and Method names
  * Class and objects should have noun or noun phrase names (eg. Customer, Account). A class name should not be a verb.
  * Methods should have verb or verb phrase names. 
  Note: In java, accessors , mutators and predicates should be named for their value and prefixed with <i>get</i>, <i>set</i> and <i>is</i> according to javabean standard.
  * Add meaningful context to variable, method and class names. Avoid using prefixes for context(Eg. customerFirstName).

#### Functions

* Functions should be small.
  * Blocks within <i>if</i>, <i>else</i>, <i>while</i>  and so on statements should be one line long. Probably that line should be a function call. It keeps the function small and function called within the block can have a descriptive name.
  * Functions should not be large enough to hold nested structures. Therefore, indent level of a function should not be greater than one or two.
* Function should do <i>one thing</i>. They should do it <i>well</i>. They should do it <i>only</i>.
* One level of abstraction per function - statements within our function should all be at same level of abstraction.
* Switch statements
  * Switch statements always do N things, so it's important to take care of these.
  * Try to avoid switch statements, if not possible then make sure each switch statement is buried in a low-level class and is never repeated. This can be achieved using polymorphism.
  * General rule: switch statements should appear only once, are used to create polymorphic objects, and are hidden behind an inheritance relationship so that rest of the system can't see them.
* Use descriptive names
  * The smaller and more focused the function is, the easier it is to choose a descriptive name.
  * A long descriptive name is better than a short enigmatic name.
  * A long descriptive name is better than a long descriptive comment.
  * Choosing descriptive names wil clarify the design of the module in your mind.
  * Be consistent in your names. Use the same phrases, nouns, and verbs in the function names you choose for your module.
