# Ruby Bug: Unexpected Behavior from Direct Instance Variable Manipulation

This repository demonstrates a common, yet subtle, bug in Ruby related to directly manipulating instance variables using `instance_variable_set`. While technically functional, it violates good object-oriented principles and can make code less maintainable and prone to errors.

The `bug.rb` file shows the buggy code. The `bugSolution.rb` demonstrates a more robust and idiomatic solution.

**Problem:** Direct manipulation of instance variables using methods like `instance_variable_set` bypasses the intended encapsulation provided by accessor methods (`attr_accessor`, `attr_reader`, `attr_writer`). This can lead to inconsistencies and difficulties in debugging.

**Solution:**  Prefer using accessor methods or defining appropriate methods to interact with instance variables. This promotes better code structure, maintainability, and predictability.