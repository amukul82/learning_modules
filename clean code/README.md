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
