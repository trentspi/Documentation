# Code Standards
This is an extremely broad topic and there are many concerns when writing code for a shared project.  We will not be enforcing extreme coding standards.  That being said there will be a handful of requirements that collaborators will have to adhere too.

## Indention
All collaborators must use 2 space tabs.

## Code Blocks (not the ide)
Code segments will look as follows:
```JavaScript
for (var i = 0; i < 5; i++) {
  // do stuff
}
```

## Variable Names
All variable names must be clear and all variable names must be in Camel Case.
```JavaScript
var packageManager = new uPackage();
```

## Documentation
All collaborators will provide clear comments on non-trivial sections of their code.
```JavaScript
var values = [5, 7, 9, 2, 4];
var temp;

// Bubble Sort Algorithm
// For each element in the array, compare that value with every other value
// if the value on the left is greater than the value on the right
// than it should be swapped closer to the end of the array
for (var i = 0; i < values.length; i++) {
  for (var j = 0; j < values.length - 1; j++) {
    if (values[j] > values[j+1]) {
      temp = values[j];
      values[j] = values[j+1];
      values[j+1] = temp;
    }
  }
}
```

